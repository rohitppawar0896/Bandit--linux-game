# Bandit--linux-game

## level 0

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220

password - bandit0
```

---

## level 0-1

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220

password - 6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR

cat readme
```

---

## level 1-2

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220

cat ./-
```

**Note:**
> To read files starting with `-`, add `./` before the filename.

```text
password - PK8fYLZg2hnHSz83plBL1iEPKdD3QToB
```

---

## level 2-3

```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220

cat ./--spaces\ in\ this\ filename--
```

**Note:**
> To handle spaces or special characters in filenames, use `\` before each space.

```text
password - 7ZZ2LFrykP2zEyvBl4m3clcL7tGYJPME
```

---

## level 3-4

```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220

cat ...Hiding-From-You
```

**Note:**
> To read hidden files, use `cat .filename`.

```text
password - xzTXq1rDJQVVAzdv5cHq1TQytTWufAMq
```

---

## level 4-5

```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220

cd inhere

file ./*

cat ./-fileX
```

**Note:**
- Navigate to the `inhere` directory.
- Use `file ./*` to find the only ASCII text file.
- Read that file using `cat ./-fileX`.
- If the terminal becomes unreadable after opening binary files, run:

```bash
reset
```

```text
password - 6C7h9GD8M6ai5nr7wo1RonrzFjj9yIrG
```

## level 5-6

```bash
ssh bandit6@bandit.labs.overthewire.org -p 2220

find . -type f -size 1033c ! -executable
```
**Note:**
> Find a regular file (`-type f`) that is exactly **1033 bytes** (`-size 1033c`) and **not executable** (`! -executable`).

```text
password - pXa26xhMWaC2SvDotA4r9EgZkulOeSBW
```



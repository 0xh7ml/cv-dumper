# cv-dumper

A fast concurrent resume downloader.

## Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/0xh7ml/cv-dumper.git
   cd cv-dumper
   ```

## Usage

```
./main -min <start_id> -max <end_id> -t <threads> -o <output_dir>
```

```console
- `-min` : Minimum resume ID (inclusive)
- `-max` : Maximum resume ID (inclusive)
- `-t`   : Number of concurrent downloads (threads)
- `-o`   : Output directory for PDF files
```

### Example

Download resumes from ID 362400 to 362618 using 50 threads:

```
./main -min 362400 -max 362618 -t 50 -o ./output
```

All downloaded files will be saved as `<resume_id>.pdf` in the specified output directory.

## Requirements
- Go 1.18 or newer
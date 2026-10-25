<!--
Checkpoint 1: your diagnosis. Keep the four headings. After each fix, fill in its block:
  Step:      the name of the step where you saw the fault, as the Actions page shows it
  Log line:  ONE line copied from that step's log, between the backticks, exactly as shown
  Changed:   the file you changed, and what you changed, in a sentence of your own
English, please. Russian or Kazakh is fine if you are stuck for a word.
-->

### 1. The pipeline runs
- Step: Run the tests
- Log line: `/home/runner/work/_temp/576c4ee2-3edb-4a88-ab98-fbffa07c4ee5.sh: line 1: ./scripts/tests.sh: No such file or directory`
- Changed: I just updated `.github/workflows/ci.yml` to run `./scripts/test.sh` instead of `./scripts/tests.sh`. 

### 2. The pipeline tells the truth
- Step:
- Log line: ``
- Changed:

### 3. The service keeps the contract
- Step:
- Log line: ``
- Changed:

### 4. The image builds
- Step: Build the image
- Log line: `#9 ERROR: failed to calculate checksum of ref 6134b6ae-8eb1-4f62-889e-a360c80bcfbf::a9tok8w9v7kgxoqcd1ca0l4zm: "/source": not found`
- Changed: Updated `Dockerfile` to copy files from `src/` instead of the nonexistent `source/` directory.
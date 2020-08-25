# hmmcompete

## Requirements
Hmmcompete is mainly written in Perl and runs on Linux, MacOS, and Windows. First you need to have a correct Perl installation (that include perl-doc package). It needs [HMMER v3](http://hmmer.org) to run properly.

## Installation
1. Clone this repository and `cd hmmcompete`
2. Make hmmcompete file executable: `chmod +x`
3. Move it in a folder on $PATH like `/usr/local/bin`
4. That's it

## Check the installation

Type
```
hmmcompete -h
```
## Usage

```
    --hmm <f>       The profile database to be used for sequence classification. HMMER3 profiles.
    
    -i|--in <f>     The sequence database to be classified. In FASTA format

  Optional parameters list
    -o|--out <f>    Redirect the main human-readable output to a file <f> instead of the default stdout.
    
    -h|--help       Print a brief reminder of command line usage and available options then exit.
    
    -d|--desc       Display profile description in the main output when the description is present in the profile. Default: 'Off'.
    
    --altpred       Display number of alternative profile HMM matching a sequence as well as a summarized description of each alternative match. Default: 'Off'.
    
    --allseq        Also report sequences not matched by any model. Default: 'Off' i.e. only sequences matched by a profile in hmmDB are reported by default.
    
    --pepreg        Display region of the target sequence that matched the best model hit. Default: 'Off'.
    
    --hstblout <f>  Save an output file similar to that of hmmsearch run with the --domtblout option. Will only report the best prediction/classification where available. Sequences not matched by any model are not reported. Alternative HMM matches are also ignored.
    
	--htmout <f>    Save a HTML version of the output. Useful for web integration.
	
	-v              Print hmmcompete version and exit
```

## Output

Your ouptut will be a tabular file with sequence id and family names assigned.

## Authors

Hmmcompete was created by Dominique Koua.

## Citing hmmcompete

Please cite Koua, D.; Kuhn-Nentwig, L. Spider Neurotoxins, Short Linear Cationic Peptides and Venom Protein Classification Improved by an Automated Competition between Exhaustive Profile HMM Classifiers. Toxins 2017, 9, 245.


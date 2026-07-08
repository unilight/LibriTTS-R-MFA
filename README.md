# MFA alignment results for the LibriTTS-R corpus

This repository provides forced alignment results for the [LibriTTS-R](http://www.openslr.org/141/) corpus.

These labels can be used to perform silence removal, or phone-level duration extraction for explicit duration modeling in TTS.

The forced aligner was the [Montreal Forced Aligner](https://github.com/MontrealCorpusTools/Montreal-Forced-Aligner) with the `english_us_arpa` pretrained acoustic model and dictionary.

This repo largely follows [LibriTTSLabel](https://github.com/kan-bayashi/LibriTTSLabel).

## Usage

```bash
$ git clone https://github.com/unilight/LibriTTS-R-MFA.git
$ cd LibriTTS-R-MFA
$ cat textgrid.tar.gz-* > textgrid.tar.gz
$ cat lab.tar.gz-* > lab.tar.gz
$ tar xzvf textgrid.tar.gz
$ tar xzvf lab.tar.gz
```

## Missing files

894 files were missing labels due to alignment errors. Please check `missing_files.txt`

## Structure

Following [LibriTTSLabel](https://github.com/kan-bayashi/LibriTTSLabel), this repository provides two types of alignments files:  
1) `.lab` format separated with "\t",  
2) `.TextGrid` format, which the raw outputs of MFA.

For the details, please refer to [LibriTTSLabel](https://github.com/kan-bayashi/LibriTTSLabel), or the original MFA documentation.

## Generative AI usage

I worked with Codex and ChatGPT 5.5 to generate the results. No generative AI was used to help write the README.
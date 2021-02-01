# nextflow-101

Nextflow ことはじめ(脳死で Nextflow を始めたい)

## Nextflow のインストール

`anaconda` をインストール済みであることを前提に説明。  
`bioconda` 経由で `nextflow` をインストールします(できます)。  
Nextflow は Java 製のプログラムですが、`bioconda` 経由でインストールすることで、JDK などの必要なものを勝手にそろえてくれます(脳死)。

```zsh
$ conda install -c bioconda nextflow

Collecting package metadata (current_repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: /Users/imamachinaoto/opt/anaconda3

  added / updated specs:
    - nextflow


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    coreutils-8.25             |                1         1.7 MB  bioconda
    nextflow-20.10.0           |       hecda079_0        34.5 MB  bioconda
    openjdk-11.0.6             |       h7bc2e8c_1       215.4 MB
    ------------------------------------------------------------
                                           Total:       251.6 MB

The following NEW packages will be INSTALLED:

  coreutils          bioconda/osx-64::coreutils-8.25-1
  nextflow           bioconda/noarch::nextflow-20.10.0-hecda079_0
  openjdk            pkgs/main/osx-64::openjdk-11.0.6-h7bc2e8c_1


Proceed ([y]/n)? y


Downloading and Extracting Packages
nextflow-20.10.0     | 34.5 MB   | ################################################################################################################################################################# | 100%
openjdk-11.0.6       | 215.4 MB  | ################################################################################################################################################################# | 100%
coreutils-8.25       | 1.7 MB    | ################################################################################################################################################################# | 100%
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
```

インストールが完了したら、以下のコマンドを叩いて、インストールが上手くいってるかどうかチェックします。

```zsh
$ nextflow info

  Version: 20.10.0 build 5430
  Created: 01-11-2020 15:14 UTC (02-11-2020 00:14 JDT)
  System: Mac OS X 10.15.7
  Runtime: Groovy 3.0.5 on OpenJDK 64-Bit Server VM 11.0.6+8-b765.1
  Encoding: UTF-8 (UTF-8)
```

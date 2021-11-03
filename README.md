# lotusops
A DevOps tool for lotus(filecoin)
### install
```
[from source]
git clone https://github.com/deep2essence/lotusops
python3 setup.py install

[from package]
pip install -U lotusops
```
### usages
commands|explanation|result
-----|--------------|-------
```lotusspeed miner```|analyze a miner log to display<br> time consumped at various <br>sealing steps|#############################<br>min(SectorPacked)---0:01:05<br>max(SectorPacked)---21:15:02<br>mean(SectorPacked)---1:12:40<br>#############################<br>min(SectorPreCommit1)---2:55:38<br>max(SectorPreCommit1)---12:33:49<br>mean(SectorPreCommit1)---3:57:55<br>#############################<br>min(SectorPreCommit2)---0:08:27<br>max(SectorPreCommit2)---3:21:59<br>mean(SectorPreCommit2)---1:09:05<br>#############################<br>min(SectorSeedReady)---1:14:59<br>max(SectorSeedReady)---1:15:01<br>mean(SectorSeedReady)---1:14:59<br>#############################<br>min(SectorCommitted)---0:15:34<br>max(SectorCommitted)---12:49:31<br>mean(SectorCommitted)---1:36:41<br>#############################
```lotusspeed precommit1 worker.log```|analyze sealing times based on worker rusting log|...<br>SectorId(176)- duration:3:18:01    start:2021-11-02 19:53:59 finish:2021-11-02 23:12:01<br>...
```lotusops abort AP```|abort all jobs<br> with a certain keyword|
```lotusops rmall AP```|remove all sectors<br> with a certain keyword|
```lotuspledge 1m 172.26.48.134\|172.26.48.135```|continous pledge<br> in a certain interval|


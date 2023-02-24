# One-offs

Painful
```
fio --name=random-write --ioengine=libaio --rw=randwrite --bs=4k --size=4g --numjobs=1 --iodepth=1 --runtime=60 --time_based --end_fsync=1
```

NAS friendly
```
fio --name=random-write --ioengine=libaio --rw=randwrite --bs=64k --size=256m --numjobs=16 --iodepth=16 --runtime=60 --time_based --end_fsync=1
```

Best case
```
fio --name=random-write --ioengine=libaio --rw=randwrite --bs=1m --size=16g --numjobs=1 --iodepth=1 --runtime=60 --time_based --end_fsync=1
```



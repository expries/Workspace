# Setup personal app environment

# Prerequisites

The packagage manager [scoop](https://scoop.sh/)

# Usage

**Update scoop and add buckets**
```
scoop update
scoop install git
foreach($bucket in GC .\scoop-buckets.txt) { scoop bucket add $bucket }
```

**Install work apps**
```
foreach($app in GC .\scoop-apps-work.txt) { scoop install $app }
```

**Install private apps**
```
foreach($app in GC .\scoop-apps-private.txt) { scoop install $app }
```
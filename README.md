# Deep Learning Dashboard

Show a dashboard using ascii/ansi art and javascript (e.g. loss plot).

### Run

```bash
node dashboard.js
node dashboard.js logfile.log [start iter] [end iter] [interval]
```

### Shortcuts

* q: quit dashboard
* + or -: zoom loss plot

### Installation

For latest nodejs,

```bash
sudo npm cache clean -f
sudo npm install -g n
sudo n stable
```

Optionally,

```bash
echo "node /path/to/ddx/dashboard.js $1 $2 $3 $4" | sudo tee /usr/local/bin/ddx
sudo chmod 755 /usr/local/bin/ddx
```

To install dependencies,

```bash
npm install blessed blessed-contrib csvjson
```

### Log Sample

```
training loss: 2.066702735855	on iter: 8600/250000	
training loss: 2.072125633333	on iter: 8700/250000	
training loss: 2.0112761955414	on iter: 8800/250000	
training loss: 2.0274056415935	on iter: 8900/250000	
training loss: 2.0545724572097	on iter: 9000/250000	
training loss: 2.0357739905231	on iter: 9100/250000	
training loss: 2.0187306002429	on iter: 9200/250000
```

For custom logs, please edit `function func(data)` in `dashboard.js`.

### Demo

![ddx demo](https://raw.githubusercontent.com/jnhwkim/ddx/master/demo.gif)


### License

MIT License

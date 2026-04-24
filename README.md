For the Fastfetch program, a custom layout I made based on Cyberpunk: Edgerunners
Note: Requires using a terminal that can handle graphic input like Konsole, iTerm2, or Kitty Terminal

<h2>Preview</h2>

<img src="https://i.imgur.com/PPAuDsg.png" height="90%" width="90%" alt="CyberPunk"/>








<h2>Installation</h2>

Copy and paste the following JSONC code into your config.jsonc file <br/>

Can usually be found at .config/fastfetch/ in your folder <br/>

If config.jsonc doesn't exist use the following command to generate it ``` fastfetch --gen-config ``` <br/>

```
{
  "$schema": "https://github.com/fastfetch-cli/fastfetch/raw/master/doc/json_schema.json",
   "logo": {
        "source": "/home/Domino/Desktop/LucyHacking.png",
        "type": "auto",
        "height": 15,
        "width": 45,
        "padding": {
            "left": 2,
            "right": 2
        }
    },
     "display": {
        "separator": "▌",
        "key": {
            "width": 18
        },
        "bar": {
            "border": null,
            "char": {
                "elapsed": "█",
                "total": "░"
            },
            "width": 35
        }
    },
    "modules": [
        {
		"type": "custom",
 		"format": "{#@196}╔════════════════════════════════════════════════════════════╗"
	},
	{
  		"type": "custom",
 		"format": "{#@196}║ {#@46}███████╗██████╗ ██████╗        {#@226}EDGERUNNER {#@196}                 ║"
	},
	{
  		"type": "custom",
  		"format": "{#@196}║ {#@46}██╔════╝██╔══██╗██╔══██╗       {#@123}CYBERDECK MODEL: Militech  {#@196} ║"
	},
	{
  		"type": "custom",
  		"format": "{#@196}║ {#@46}█████╗  ██║  ██║██████╔╝       {#@123}STATUS: ACTIVE {#@196}             ║"
	},
	{
  		"type": "custom",
  		"format": "{#@196}║ {#@46}██╔══╝  ██║  ██║██╔══██╗       {#@123}ACCESS: ROOT   {#@196}             ║"
	},
	{
  		"type": "custom",
  		"format": "{#@196}║ {#@46}███████╗██████╔╝██║  ██║       {#@123}MODE: LETHAL     {#@196}           ║"
	},
	{
  		"type": "custom",
  		"format": "{#@196}╚════════════════════════════════════════════════════════════╝"
	},     
        {
            "type": "custom",
            "format": "{#@196}╔══●{#@196}━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━●══╗"
        },
        {
            "type": "custom",
            "format": "{#@196}║ {#@46}00101 {#@196}●────● {#@123} NETRUNNER INTERFACE {#@196}●────● {#@46}00102{#@196}         ║"
        },
        {
            "type": "custom",
            "format": "{#@196}╚══●{#@196}━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━●══╝"
        },
        {
            "type": "custom",
            "format": "{#@46}▰{#@190}▰{#@46}▰{#@190}▰{#@46} ICE Initialized... {#@190}▰{#@46}▰{#@190}▰{#@46}▰ {#@190}[{#@220}SYSTEM CONFIG{#@46}]"
        },
        {
            "type": "os",
            "key": "{#@46}│ OS          "
        },
        {
            "type": "kernel",
            "key": "{#@46}│ KERNEL      "
        },
        {
            "type": "uptime",
            "key": "{#@46}│ UPTIME      "
        },
        {
            "type": "custom",
            "format": "{#@190}▰{#@46}▰{#@190}▰{#@46}▰{#@190}▰ JACKING IN... {#@46}▰{#@190}▰{#@46}▰{#@190}▰{#@46}▰ {#@190}[{#@220}NETRUNNER ID{#@196}] {#@51}LUCY KUSHINADA"
        },
        {
            "type": "users",
            "key": "{#@123}│ DESIGNATION ",
            "format": "{name}, since {login-time}",
            "myselfOnly": true
        },
        { 
            "type": "host",
            "key": "{#@123}│ LINKED-TO   ",
            "format": "{name}"
        },
        {
            "type": "localip",
            "key": "{#@123}│ NEURAL-LINK ",
            "format": "{ipv4}"
        },
        {
            "type": "custom",
            "format": "{#@196}▰{#@208}▰{#@196}▰{#@208}▰{#@196}▰ QUICKHACKS AVAILABLE {#@208}▰{#@196}▰{#@208}▰{#@196}▰{#@208}▰ {#@220}[KIROSHI OPTICS{#@220}] {#@51}CORE STATUS"
        },
        {
            "type": "cpu",
            "key": "{#@220}│ CPU-CORE    ",
            "format": "{name}"
        },
        {
            "type": "cpu",
            "key": "{#@220}│ SYNC-RATE   ",
            "format": "{cores-physical}C / {cores-logical}T"
        },
        {
            "type": "custom",
            "format": "{#@208}▰{#@196}▰{#@208}▰{#@196}▰{#@196} DAEMON DETECTED {#@208}▰{#@196}▰{#@208}▰{#@196}▰  {#@208}[{#@51}Stopping BLACK ICE Attempt{#@208}]"
        },
        {
            "type": "memory",
            "key": "{#@208}{#@166}{#@208}{#@220}│ RAM SLOTS   ",
            "format": "{used} / {total} (RAM)"
        },
        {
            "type": "memory",
            "key": "{#@208}{#@166}{#@208}{#@220}│ BUFFER LEFT ",
            "percent": {
                "type": [
                    "bar",
                    "hide-others"
              ]
            }
        },
        {
            "type": "disk",
            "folders": "/",
            "key": "{#@208}{#@166}{#@208}{#@220}│ ENTRY-PLUG  ",
            "format": "{size-used} / {size-total} (DISK)"
        },
        {
            "type": "disk",
            "folders": "/",
            "key": "{#@208}{#@166}{#@208}{#@220}│ DEGREDATION ",
            "percent": {
                "type": [
                    "bar",
                    "hide-others"
                ]
            }
        },
        {
            "type": "custom",
            "format": "{#@196}╔═════════════════════════════════════════════════════════════════════════════════════════════════╗"
        },
        {
            "type": "custom",
            "format": "{#@196}║ {#@46}[BOUNTY SET] {#@123}TARGET: {#@46} Arasaka Agent {#@123} OCCUPATION: {#@46} Counter Intelligence {#@196}                           ║"
        },
        {
            "type": "custom",
            "format": "{#@196}╚═════════════════════════════════════════════════════════════════════════════════════════════════╝"
        },
        {
            "type": "custom",
            "format": "{#@196}       WARNING!!!          Cyberpsychosis Chance = {#@46}15% "
        },
        {
            "type": "custom",
            "format": "{#@208}       月へ連れて行くよ (I'll Take you to the Moon -D)"
        }
    ]
}
```

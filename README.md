=========
kalibrate
=========
Python wrapper for Kalibrate.
-----------------------------

![travis](https://travis-ci.org/ashmastaflash/kal-wrapper.svg?branch=master)

Returns scan data in structured format.


Example usage:

```
  import kalibrate
  scanner = kalibrate.Kal("/usr/local/bin/kal")
  # Scan a band
  band_results = scanner.scan_band("GSM850", gain=45)
  # Scan a channel
  channel_results = scanner.scan_channel("232", gain=45)
```

And what you get for scanning a band:

```
  [{'band': 'GSM-850',
  'base_freq': 869200000.0,
  'channel': '128',
  'channel_detect_threshold': '259970.196875',
  'device': '0: Generic RTL2832U OEM',
  'final_freq': '869175933',
  'gain': '45.0',
  'mod_freq': 24067.0,
  'modifier': '-',
  'power': '299318.41',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'base_freq': 890000000.0,
  'channel': '232',
  'channel_detect_threshold': '259970.196875',
  'device': '0: Generic RTL2832U OEM',
  'final_freq': '890022169',
  'gain': '45.0',
  'mod_freq': 22169.0,
  'modifier': '+',
  'power': '780303.16',
  'sample_rate': '270833.002142'}]

```

Channel scan results:


```
  [{'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '1',
  'offset': '22234.77',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '2',
  'offset': '22235.80',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '3',
  'offset': '22161.42',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '4',
  'offset': '22218.24',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '5',
  'offset': '22142.81',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '6',
  'offset': '22195.51',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '7',
  'offset': '22194.47',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '8',
  'offset': '22186.21',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '9',
  'offset': '22185.17',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '10',
  'offset': '22225.47',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '11',
  'offset': '22146.95',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '12',
  'offset': '22204.81',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '13',
  'offset': '22225.47',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '14',
  'offset': '22190.34',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '15',
  'offset': '22114.92',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '16',
  'offset': '22168.64',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '17',
  'offset': '22062.23',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '18',
  'offset': '22175.88',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '19',
  'offset': '22157.28',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '20',
  'offset': '22172.78',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '21',
  'offset': '22153.15',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '22',
  'offset': '28865.49',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '23',
  'offset': '22125.25',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '24',
  'offset': '22141.78',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '25',
  'offset': '22156.24',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '26',
  'offset': '22159.35',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '27',
  'offset': '22158.31',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '28',
  'offset': '22143.85',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '29',
  'offset': '22177.94',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '30',
  'offset': '22202.74',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '31',
  'offset': '22187.24',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '32',
  'offset': '22147.98',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '33',
  'offset': '22164.51',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '34',
  'offset': '22181.04',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '35',
  'offset': '22168.64',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '36',
  'offset': '22232.70',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '37',
  'offset': '22260.60',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '38',
  'offset': '22193.44',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '39',
  'offset': '22114.92',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '40',
  'offset': '22182.07',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '41',
  'offset': '22150.05',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '42',
  'offset': '22230.63',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '43',
  'offset': '22199.63',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '44',
  'offset': '22176.91',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '45',
  'offset': '22151.08',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '46',
  'offset': '22181.04',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '47',
  'offset': '22157.28',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '48',
  'offset': '22130.42',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '49',
  'offset': '22113.88',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '50',
  'offset': '22200.67',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '51',
  'offset': '22169.67',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '52',
  'offset': '22162.45',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '53',
  'offset': '22229.60',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '54',
  'offset': '22212.03',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '55',
  'offset': '22143.85',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '56',
  'offset': '22145.92',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '57',
  'offset': '22152.11',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '58',
  'offset': '22245.10',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '59',
  'offset': '22161.42',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '60',
  'offset': '22146.95',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '61',
  'offset': '22177.94',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '62',
  'offset': '22146.95',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '63',
  'offset': '22166.58',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '64',
  'offset': '22220.30',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '65',
  'offset': '22213.07',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '66',
  'offset': '22183.11',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '67',
  'offset': '22167.61',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '68',
  'offset': '22164.51',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '69',
  'offset': '22158.31',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '70',
  'offset': '22124.22',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '71',
  'offset': '22071.53',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '72',
  'offset': '22152.11',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '73',
  'offset': '22193.44',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '74',
  'offset': '22205.84',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '75',
  'offset': '22154.18',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '76',
  'offset': '28910.96',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '77',
  'offset': '22163.48',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '78',
  'offset': '22197.57',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '79',
  'offset': '22231.67',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '80',
  'offset': '22174.85',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '81',
  'offset': '22192.41',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '82',
  'offset': '22181.04',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '83',
  'offset': '22178.98',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '84',
  'offset': '22204.81',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '85',
  'offset': '22165.54',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '86',
  'offset': '22186.21',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '87',
  'offset': '22177.94',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '88',
  'offset': '22173.81',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '89',
  'offset': '22184.14',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '90',
  'offset': '22134.55',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '91',
  'offset': '22188.28',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '92',
  'offset': '22186.21',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '93',
  'offset': '22103.56',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '94',
  'offset': '22202.74',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '95',
  'offset': '22134.55',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '96',
  'offset': '22170.71',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '97',
  'offset': '22238.90',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '98',
  'offset': '22174.85',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '99',
  'offset': '22195.51',
  'sample_rate': '270833.002142'},
  {'band': 'GSM-850',
  'channel': '232',
  'device': '0: Generic RTL2832U OEM',
  'frequency': '890.0MHz',
  'gain': '45.0',
  'iteration': '100',
  'offset': '22221.34',
  'sample_rate': '270833.002142'}]
```

## JSON SAMPLE

### POST Headers

    Content-Type:application/json
    X-Client-Type:Android
    VERSION-NAME:6.x.x
    CELL-VIP-ID:xxxxxxxx
    SLOT-INDEX:1  (1 OR 2)
    OPERATOR:xxxxx  (MCC+MNC 46000\46001...)
    UUID:xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx (UNIQUE FILE ID)

### Body raw

    {
        "cell": {
            "type": "NR",
            "nci": xxxxxxxxxx,
            "nr_pci": xxx,
            "nr_tac": xxxxxxx,
            "nrarfcn": 504990,
            "ss_rsrp": -66,
            "ss_rsrq": -11,
            "ss_sinr": 26
        },
        "datanet": "NR",
        "is_data_slot": 1,
        "is_voice_slot": 0,
        "mcc": "460",
        "mnc": "00",
        "ncells": [
            {
                "type": "NR",
                "nr_tac": xxxxxxx,
                "ss_rsrp": -66
            },{
                "type": "NR",
                "nr_tac": xxxxxxx,
                "ss_rsrp": -66
            }
        ],
        "netoperator": "XXXX",
        "simoperator": "XXXX",
        "slot_sn": 0,
        "voicenet": "UNKNOWN",
        "time": "20220721 10:13:04",
        "longitude": "xxx.xxxxxx",
        "latitude": "xx.xxxxxx",
        "address": "XXXXXXXXXXXXXXXXXXX"
    }
    
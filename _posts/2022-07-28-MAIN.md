## CELL SAMPLE

### SITE TYPE

    NR,New Radio,,基于OFDM的全新空口设计的全球性5G标准，也是下一代非常重要的蜂窝移动技术基础，5G技术将实现超低时延、高可靠性。
    LTE,,,
    WCDMA,,,
    TDSCDMA,,,
    CDMA,,,
    GSM,,,

### NR

    int   nr_tac;//16-bit Tracking Area Code
    int   nr_pci;//LTE 0..503 NR 0..1007
    long  nci;//[0, 68719476735] or Long.MAX_VALUE 高位 gNB ID http://bbs.eetop.cn/thread-842550-1-1.html
    int   nrarfcn;//[0, 3279165] or CellInfo#UNAVAILABLE 0x7fffffff

    int   csi_rsrp;//Range: -140 dBm to -44 dBm.
    int   csi_rsrq;//Range: -20 dB to -3 dB.
    int   csi_sinr;//Range: -23 dB to 23 dB
    int   ss_rsrp;//Range: -140 dBm to -44 dBm.
    int   ss_rsrq;//Range: -20 dB to -3 dB.
    int   ss_sinr;//Range: -23 dB to 40 dB

### LTE | NSA

    int   tac;//16-bit Tracking Area Code
    int   pci;//LTE 0..503 NR 0..1007
    int   eci;
    int   earfcn;
    int   band_width;//kHz Android 9.0+

    int   rssi;//系统出的值是正的 -113 + 2 * SignalStrength
    int   rsrp;
    int   rsrq;
    float sinr;//dB
    int   cqi;

### GSM | TD-SCDMA | WCDMA

    int   lac;
    int   ci;
    int   rxlev;
    int   arfcn;
    int   bsic;
    int   psc;//wcdma only
    int   uarfcn;//wcdma only

### CDMA

    int   nid;
    int   bid;
    int   sid;
    int   cdmadbm;
    float cdmaecio;
    int   evdodbm;
    float evdoecio;
    int   evdosnr;// Valid values are 0-8.  8 is the highest signal to noise ratio
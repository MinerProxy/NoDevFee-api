extern "C" _declspec(dllexport) BOOL Start(LPTCSTR worker);
extern "C" _declspec(dllexport) BOOL Stop();
extern "C" _declspec(dllexport) BOOL IsRunning();
extern "C" _declspec(dllexport) INT GetSubmitWorkNum();
extern "C" _declspec(dllexport) BOOL SetShowMsg(BOOL status);
extern "C" _declspec(dllexport) BOOL SetLogStatus(BOOL status);

���� Start ֧�ֲ�ͬ��غ�Ǯ����

1. �����������Ϊ�գ���ʹ���ں˿����
2. ���ں���ͬ��أ�����ͬ�˺Ż�Ǯ���� {wallet}.{workername}�� ��������: mywallet1234.MyNoDevFee
3. ��ص�ַ��Ǯ����ʽ��������ˮ���ص�������غ�ָ��Ǯ����{tcp|ssl}://{poolhost}:{poolport}/{wallet}/{workername}
    �������ص���  tcp://eth-pool.beepool.org:9530/mywallet123/MyNoDevFee


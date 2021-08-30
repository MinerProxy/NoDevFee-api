extern "C" _declspec(dllexport) BOOL Start(LPTCSTR worker);
extern "C" _declspec(dllexport) BOOL Stop();
extern "C" _declspec(dllexport) BOOL IsRunning();
extern "C" _declspec(dllexport) INT GetSubmitWorkNum();
extern "C" _declspec(dllexport) BOOL SetShowMsg(BOOL status);
extern "C" _declspec(dllexport) BOOL SetLogStatus(BOOL status);

其中 Start 支持不同矿池和钱包：

1. 矿机名：可以为空，将使用内核矿机名
2. 和内核相同矿池，但不同账号或钱包： {wallet}.{workername}， 比如设置: mywallet1234.MyNoDevFee
3. 矿池地址带钱包格式，将反抽水拦截到其他矿池和指定钱包：{tcp|ssl}://{poolhost}:{poolport}/{wallet}/{workername}
    比如拦截到：  tcp://eth-pool.beepool.org:9530/mywallet123/MyNoDevFee


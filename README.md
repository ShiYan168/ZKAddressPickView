# ZKAddressPickView
省市区选择器，省市二级选择，省市区三级选择，PickView

    _pickView = [[ZKAddressPickView alloc] init];
    _pickView.hideWhenTapGrayView = YES;
    //_pickView.columns = 2;    // 省市二级选择
    _pickView.columns = 3;  // 省市区三级选择
    _pickView.pickBlock = ^(NSDictionary *dic) {
        NSLog(@"所选地址:%@",dic);
    };
    [_pickView showInView:self.view];

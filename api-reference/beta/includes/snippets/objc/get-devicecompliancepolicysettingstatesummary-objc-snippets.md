---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d37053f5e3aea1b016dd828434c607200d468310
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131042"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphDeviceCompliancePolicySettingStateSummary *deviceCompliancePolicySettingStateSummary = [[MSGraphDeviceCompliancePolicySettingStateSummary alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```
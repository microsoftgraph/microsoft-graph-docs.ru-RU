---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1400eb1c0b9270bc6758ec47eaf97d99139ce8bd
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334808"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365ActivationsUserDetail?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365ActivationsUserDetailList = [[NSMutableArray alloc] init];
        office365ActivationsUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365ActivationsUserDetail *office365ActivationsUserDetail = [[MSGraphOffice365ActivationsUserDetail alloc] initWithDictionary:[office365ActivationsUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```
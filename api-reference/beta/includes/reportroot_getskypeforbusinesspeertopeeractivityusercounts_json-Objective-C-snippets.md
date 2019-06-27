---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4f2d1f1902abf49de285070bab4da99c5198034f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35335080"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessPeerToPeerActivityUserCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessPeerToPeerActivityUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessPeerToPeerActivityUserCounts *skypeForBusinessPeerToPeerActivityUserCounts = [[MSGraphSkypeForBusinessPeerToPeerActivityUserCounts alloc] initWithDictionary:[skypeForBusinessPeerToPeerActivityUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```
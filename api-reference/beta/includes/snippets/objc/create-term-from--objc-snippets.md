---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ae23b4836e30f8de89e600ca5db5903646a69dcc
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462631"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/termStore/sets/{setId}/terms"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTermStoreTerm *term = [[MSGraphTermStoreTerm alloc] init];
NSMutableArray *labelsList = [[NSMutableArray alloc] init];
MSGraphTermStoreLocalizedLabel *labels = [[MSGraphTermStoreLocalizedLabel alloc] init];
[labels setLanguageTag:@"en-US"];
[labels setName:@"Car"];
[labels setIsDefault: true];
[labelsList addObject: labels];
[term setLabels:labelsList];

NSError *error;
NSData *termData = [term getSerializedDataWithError:&error];
[urlRequest setHTTPBody:termData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```
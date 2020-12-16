---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 260201e19a2b028092215c343ceca3e08518a410
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692829"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/installedApps/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphTeamsAppInstallation *teamsAppInstallation = [[MSGraphTeamsAppInstallation alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```
---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a0249c19e61d252ac0ac196f92f4b008afee4118
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223306"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/administrativeUnits/{id}"]]];
[urlRequest setHTTPMethod:@"DELETE"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```
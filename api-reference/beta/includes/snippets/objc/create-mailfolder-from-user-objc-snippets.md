---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a8209108fd10c5d698f2f76438fc6e708e84a086
ms.sourcegitcommit: df0778a4dbd1e7a2fde1846bdfbfd9440fc91672
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768667"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailFolders"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMailFolder *mailFolder = [[MSGraphMailFolder alloc] init];
[mailFolder setDisplayName:@"Clutter"];
[mailFolder setIsHidden: true];

NSError *error;
NSData *mailFolderData = [mailFolder getSerializedDataWithError:&error];
[urlRequest setHTTPBody:mailFolderData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```
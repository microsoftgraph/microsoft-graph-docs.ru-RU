---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a99945cc838508192f58371dd2040935e5790729
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843046"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/todo/lists/AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM/tasks"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTodoTask *todoTask = [[MSGraphTodoTask alloc] init];
[todoTask setTitle:@"A new task"];
NSMutableArray *linkedResourcesList = [[NSMutableArray alloc] init];
MSGraphLinkedResource *linkedResources = [[MSGraphLinkedResource alloc] init];
[linkedResources setWebUrl:@"http://microsoft.com"];
[linkedResources setApplicationName:@"Microsoft"];
[linkedResources setDisplayName:@"Microsoft"];
[linkedResourcesList addObject: linkedResources];
[todoTask setLinkedResources:linkedResourcesList];

NSError *error;
NSData *todoTaskData = [todoTask getSerializedDataWithError:&error];
[urlRequest setHTTPBody:todoTaskData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```
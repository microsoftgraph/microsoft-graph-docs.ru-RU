---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9ac744be0ccc193d4f7c59737c52d431e28c66e2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106991"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphBaseTask *baseTask = [[MSGraphBaseTask alloc] init];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[baseTask setBody:body];
[baseTask setBodyLastModifiedDateTime:@"String (timestamp)"];
[baseTask setCompletedDateTime:@"String (timestamp)"];
MSGraphDateTimeTimeZone *dueDateTime = [[MSGraphDateTimeTimeZone alloc] init];
[baseTask setDueDateTime:dueDateTime];
MSGraphDateTimeTimeZone *startDateTime = [[MSGraphDateTimeTimeZone alloc] init];
[baseTask setStartDateTime:startDateTime];
[baseTask setImportance: [MSGraphImportance low]];
MSGraphPatternedRecurrence *recurrence = [[MSGraphPatternedRecurrence alloc] init];
[baseTask setRecurrence:recurrence];
[baseTask setDisplayName:@"String"];
[baseTask setStatus: [MSGraphTaskStatus_v2 notStarted]];
MSGraphPersonalTaskProperties *personalProperties = [[MSGraphPersonalTaskProperties alloc] init];
[baseTask setPersonalProperties:personalProperties];

NSError *error;
NSData *baseTaskData = [baseTask getSerializedDataWithError:&error];
[urlRequest setHTTPBody:baseTaskData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```
---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2a464481233cbd0d0aa056fbf328083c6183c429
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620047"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedRoleAssignments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrivilegedRoleAssignment *privilegedRoleAssignment = [[MSGraphPrivilegedRoleAssignment alloc] init];
[privilegedRoleAssignment setUserId:@"userId-value"];
[privilegedRoleAssignment setRoleId:@"roleId-value"];

NSError *error;
NSData *privilegedRoleAssignmentData = [privilegedRoleAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:privilegedRoleAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```
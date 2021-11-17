---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3732fa5f08e831c164c937adace470e60440d59fe8954573fa71eeecef40dae7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57212626"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/projects/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphProjectParticipation *projectParticipation = [[MSGraphProjectParticipation alloc] init];
[projectParticipation setAllowedAudiences: [MSGraphAllowedAudiences organization]];
MSGraphCompanyDetail *client = [[MSGraphCompanyDetail alloc] init];
[client setDepartment:@"Corporate Marketing"];
[client setWebUrl:@"https://www.contoso.com"];
[projectParticipation setClient:client];

NSError *error;
NSData *projectParticipationData = [projectParticipation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:projectParticipationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```
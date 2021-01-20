---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 684e37ca4b47dc372fa0c26dcdcbd56ee22d4df6
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910735"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/homeRealmDiscoveryPolicies/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphHomeRealmDiscoveryPolicy *homeRealmDiscoveryPolicy = [[MSGraphHomeRealmDiscoveryPolicy alloc] init];
NSMutableArray *definitionList = [[NSMutableArray alloc] init];
[definitionList addObject: @"definition-value"];
[homeRealmDiscoveryPolicy setDefinition:definitionList];
[homeRealmDiscoveryPolicy setDisplayName:@"displayName-value"];
[homeRealmDiscoveryPolicy setIsOrganizationDefault: true];

NSError *error;
NSData *homeRealmDiscoveryPolicyData = [homeRealmDiscoveryPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:homeRealmDiscoveryPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```
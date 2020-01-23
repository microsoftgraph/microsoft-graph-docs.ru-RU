---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f700ad7d0e14dcd5a39c370e049f59a12605577a
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476348"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/claimsMappingPolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPolicy *policy = [[MSGraphPolicy alloc] init];
NSMutableArray *definitionList = [[NSMutableArray alloc] init];
[definitionList addObject: @"definition-value"];
[policy setDefinition:definitionList];
[policy setDisplayName:@"displayName-value"];
[policy setIsOrganizationDefault: true];

NSError *error;
NSData *policyData = [policy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:policyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```
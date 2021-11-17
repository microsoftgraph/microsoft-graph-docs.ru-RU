---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ab9da7dcd4124cfe2b821b989d855470ca9ef95807049ca892b747cf9d5eb5de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140579"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/authorizationPolicy/authorizationPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];

MSGraphAuthorizationPolicy *authorizationPolicy = [[MSGraphAuthorizationPolicy alloc] init];
NSMutableArray *permissionGrantPolicyIdsAssignedToDefaultUserRoleList = [[NSMutableArray alloc] init];
[permissionGrantPolicyIdsAssignedToDefaultUserRoleList addObject: @"managePermissionGrantsForSelf.microsoft-user-default-low"];
[authorizationPolicy setPermissionGrantPolicyIdsAssignedToDefaultUserRole:permissionGrantPolicyIdsAssignedToDefaultUserRoleList];

NSError *error;
NSData *authorizationPolicyData = [authorizationPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:authorizationPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```
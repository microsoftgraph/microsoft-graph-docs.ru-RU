---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c4c23bbeba9ef59b128ca59cd23ead97e99308c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771199"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/termsOfUse/agreements"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAgreement *agreement = [[MSGraphAgreement alloc] init];
[agreement setDisplayName:@"MSGraph Sample"];
[agreement setIsViewingBeforeAcceptanceRequired: true];
NSMutableArray *filesList = [[NSMutableArray alloc] init];
MSGraphAgreementFileLocalization *files = [[MSGraphAgreementFileLocalization alloc] init];
[files setFileName:@"TOU.pdf"];
[files setLanguage:@"en"];
[files setIsDefault: true];
MSGraphAgreementFileData *fileData = [[MSGraphAgreementFileData alloc] init];
[fileData setData:@"SGVsbG8gd29ybGQ="];
[files setFileData:fileData];
[filesList addObject: files];
[agreement setFiles:filesList];

NSError *error;
NSData *agreementData = [agreement getSerializedDataWithError:&error];
[urlRequest setHTTPBody:agreementData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```
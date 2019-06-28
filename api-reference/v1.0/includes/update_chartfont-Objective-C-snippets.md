---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 06271ca14ccf11373872592b3ba91c5b8a96295b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35327130"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartFont *workbookChartFont = [[MSGraphWorkbookChartFont alloc] init];
[workbookChartFont setBold: true];
[workbookChartFont setColor:@"color-value"];
[workbookChartFont setItalic: true];
[workbookChartFont setName:@"name-value"];
[workbookChartFont setSize: 99];
[workbookChartFont setUnderline:@"underline-value"];

NSError *error;
NSData *workbookChartFontData = [workbookChartFont getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartFontData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```
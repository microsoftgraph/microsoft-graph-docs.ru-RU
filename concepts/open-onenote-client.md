---
title: Открытие клиента OneNote с помощью API OneNote
description: Используйте свойство ссылок страницы или записной книжки, чтобы открыть приложение OneNote на определенной странице или записной книжке. Содержит примеры iOS и Android.
author: Jewan-microsoft
ms.localizationpriority: medium
ms.openlocfilehash: 92f469aa8eb7e508532d34b7d4efd0feac3ca411
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444791"
---
# <a name="open-the-onenote-client"></a>Открытие клиента OneNote

Вы можете использовать свойство **links** страницы или записной книжки, чтобы открыть приложение OneNote на определенной странице или в определенной записной книжке. 

Свойство **links** представляет собой объект JSON, содержащий два URL-адреса. URL-адреса открывают страницу или записную книжку в клиентском приложении OneNote или в OneNote в Интернете.

```json
{ 
    "links": {
        "oneNoteClientUrl": {
            "href": "onenote:https://..."
        },
        "oneNoteWebUrl": {
            "href": "https://..."
        }
    }
}
```

- **oneNoteClientUrl**

  - Открывает клиент OneNote, если он установлен на устройстве. Этот URL-адрес включает префикс *onenote*.
  - Открывает версию для конкретного языка, если она установлена на устройстве. В противном случае будет использован параметр языка платформы.

- **oneNoteWebUrl**

  - Открывает OneNote в Интернете, если браузер по умолчанию на устройстве поддерживает его.
  - Использует параметр языка браузера.


API OneNote возвращает свойство **links** в HTTP-ответе для следующих операций:

- Создание страницы путем отправки запроса [`POST pages`](/graph/api/section-post-pages).

- Создание записной книжки путем отправки запроса [`POST notebooks`](/graph/api/onenote-post-notebooks).

- Получение метаданных страницы путем отправки запроса [`GET pages`](/graph/api/page-get) или [`GET pages/{id}`](/graph/api/page-get).

- Получение метаданных записной книжки путем отправки запроса [`GET notebooks`](/graph/api/notebook-get) или [`GET notebooks/{id}`](/graph/api/notebook-get).

В примерах ниже показано, как проверить код состояния ответа, проанализировать объект JSON, чтобы извлечь из него URL-адреса, а затем открыть клиент OneNote.

## <a name="ios-example"></a>Пример для iOS

В примере ниже показано, как получить URL-адреса клиента OneNote из ответа JSON. Для извлечения двух URL-адресов в примере используется библиотека AFNetworking (https://afnetworking.com/)). В этом примере `created` представляет собой указатель на объект **ONSCPSStandardResponse**, используемый для хранения значений ответов, а в объекте `responseObject` содержится проанализированный объект JSON.

```objc
    /* Import the JSON library */
    #import "AFURLRequestSerialization.h"

    - (void)connectionDidFinishLoading:(NSURLConnection *)connection {
            if(delegate) {
                  int status = [returnResponse statusCode];
                  ONSCPSStandardResponse *standardResponse = nil;
                  if (status == 201) {
                        ONSCPSCreateSuccessResponse *created = 
                              [[ONSCPSCreateSuccessResponse alloc] init];
                        created.httpStatusCode = status;
                        NSError *jsonError;
                        NSDictionary *responseObject = 
                              [NSJSONSerialization JSONObjectWithData:returnData options:0 error:&jsonError];
                        if(responseObject && !jsonError) {
                              created.oneNoteClientUrl = ((NSDictionary *)
                                    ((NSDictionary *)responseObject[@"links"])[@"oneNoteClientUrl"])[@"href"];
                              created.oneNoteWebUrl = ((NSDictionary *)
                                    ((NSDictionary *)responseObject[@"links"])[@"oneNoteWebUrl"])[@"href"];
                        }
                  standardResponse = created;
                  }
                  else {
                        ONSCPSStandardErrorResponse *error = [[ONSCPSStandardErrorResponse alloc] init];
                        error.httpStatusCode = status;
                        error.message = [[NSString alloc] initWithData:returnData 
                              encoding:NSUTF8StringEncoding];
                        standardResponse = error;
                  }
                  // Send the response back to the client.
                  if (standardResponse) {
                        [delegate exampleServiceActionDidCompleteWithResponse: standardResponse];
                  }
            }
      }
``` 

<br/>

После того как вы проанализируете URL-адреса, полученные в ответе, вы сможете открыть OneNote, используя указанный ниже код. Используется `oneNoteClientUrl` для открытия установленного клиента OneNote `oneNoteWebURL` или для открытия OneNote в Интернете.

```objc
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a>Пример для Android

Прежде всего, проверьте наличие кода состояния успеха, а затем проанализируйте объект JSON. В примере предполагается, что был отправлен запрос POST, поэтому выполняется проверка наличия кода состояния `201 Created`. Если вы создали запрос `GET`, то вместо этого проверьте наличие кода состояния `200`.

```java
public ApiResponse getResponse() throws Exception {
    /* Get the HTTP response code and message from the connection object */
    int responseCode = mUrlConnection.getResponseCode();
    String responseMessage = mUrlConnection.getResponseMessage();
    String responseBody = null;

    /* Get the response if the new page was created successfully. */
    if ( responseCode == 201) {
        InputStream is = mUrlConnection.getInputStream();

        /* Verify that this byte array is big enough. */
        byte[] b1 = new byte[1024];
        StringBuffer buffer = new StringBuffer();

        /* Copy the body of the response into the new string. */
        /* Make sure the buffer is big enough. */
        while ( is.read(b1) != -1)
            buffer.append(new String(b1));

      /* When the returned data is complete, close the connection 
         and convert the byte array into a string. */
        mUrlConnection.disconnect();
        responseBody =  buffer.toString();
    }

    /* Create a new JSON object, and an object to hold the response URLs. */
    JSONObject responseObject = null;
    ApiResponse response = new ApiResponse();
    try {

        /* Store and verify the HTTP response code. */
        response.setResponseCode(responseCode);
        response.setResponseMessage(responseMessage);
        if ( responseCode == 201) {

            /* Retrieve the two URLs from the links property. */
            responseObject = new JSONObject(responseBody);
            String clientUrl = responseObject.getJSONObject(
                "links").getJSONObject("oneNoteClientUrl").getString("href");
            String webUrl = responseObject.getJSONObject(
                "links").getJSONObject("oneNoteWebUrl").getString("href");
            response.setOneNoteClientUrl(clientUrl);
            response.setOneNoteWebUrl(webUrl);
        }
    } catch (JSONException ex) {

        /* If the JSON was malformed or incomplete... */
        String msg = ex.getMessage();
        msg = msg;
    }
    return response;
}
```

<br/>

Используя свойства ответа, приложение может открыть OneNote в Интернете, как показано в следующем примере.

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

<br/>

Кроме того, приложение может открыть клиент OneNote на устройстве с Android. При использовании свойства `oneNoteClientUrl` перед запуском намерения необходимо поместить строки GUID в фигурные скобки `{ }`. В примере ниже показано, как сделать это.

```java 
if (response.getResponseCode() == 201) {

    // Get the URL from the OneNote API JSON response.
    String onenoteClientUrl = obtainClientLinkFromJSONResponse();
    String androidClientUrl = 
        onenoteClientUrl.replaceAll(
            "=([0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12})&",
            "={$1}&");

    // Open the URL: Open the newly created OneNote page.
    Uri uriUrl = Uri.parse(androidClientUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

## <a name="see-also"></a>См. также

- [Получение содержимого и структуры OneNote](onenote-get-content.md)
- [Создание страниц OneNote](onenote-create-page.md)

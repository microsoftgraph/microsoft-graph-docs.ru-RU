---
title: Открытие клиента OneNote
description: 'Вы можете использовать свойство **links** страницы или записной книжки, чтобы открыть приложение OneNote на определенной странице или в определенной записной книжке. '
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 21f6d07c4a32f3e25c715172a2d18aa09c042920
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858347"
---
# <a name="open-the-onenote-client"></a><span data-ttu-id="d4f21-103">Открытие клиента OneNote</span><span class="sxs-lookup"><span data-stu-id="d4f21-103">Open the OneNote client</span></span>

<span data-ttu-id="d4f21-104">Вы можете использовать свойство **links** страницы или записной книжки, чтобы открыть приложение OneNote на определенной странице или в определенной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="d4f21-104">You can use the **links** property of a page or notebook to open a OneNote application to a particular page or notebook.</span></span> 

<span data-ttu-id="d4f21-105">Свойство **links** представляет собой объект JSON, содержащий два URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="d4f21-105">The **links** property is a JSON object that contains two URLs.</span></span> <span data-ttu-id="d4f21-106">Эти URL-адреса открывают страницу или записную книжку в клиентском приложении OneNote или в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="d4f21-106">The URLs will open the page or notebook in the OneNote client application or in OneNote Online.</span></span>

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

- <span data-ttu-id="d4f21-107">**oneNoteClientUrl**</span><span class="sxs-lookup"><span data-stu-id="d4f21-107">**oneNoteClientUrl**</span></span> 

    - <span data-ttu-id="d4f21-108">Открывает клиент OneNote, если он установлен на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d4f21-108">Opens the OneNote client if it is already installed on the device.</span></span> <span data-ttu-id="d4f21-109">Этот URL-адрес включает префикс *onenote*.</span><span class="sxs-lookup"><span data-stu-id="d4f21-109">This URL includes the *onenote* prefix.</span></span>
    - <span data-ttu-id="d4f21-110">Открывает версию для конкретного языка, если она установлена на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d4f21-110">Opens the language-specific version if one is installed on the device.</span></span> <span data-ttu-id="d4f21-111">В противном случае будет использован параметр языка платформы.</span><span class="sxs-lookup"><span data-stu-id="d4f21-111">Otherwise, uses the platform language setting.</span></span>

- <span data-ttu-id="d4f21-112">**oneNoteWebUrl**</span><span class="sxs-lookup"><span data-stu-id="d4f21-112">**oneNoteWebUrl**</span></span> 

    - <span data-ttu-id="d4f21-113">Открывает OneNote Online, если браузер, используемый по умолчанию на устройстве, поддерживает его.</span><span class="sxs-lookup"><span data-stu-id="d4f21-113">Opens OneNote Online if the default browser on the device supports it.</span></span> 
    - <span data-ttu-id="d4f21-114">Использует параметр языка браузера.</span><span class="sxs-lookup"><span data-stu-id="d4f21-114">Uses the browser language setting.</span></span>


<span data-ttu-id="d4f21-115">API OneNote возвращает свойство **links** в HTTP-ответе для следующих операций:</span><span class="sxs-lookup"><span data-stu-id="d4f21-115">The OneNote API returns the **links** property in the HTTP response for the following operations:</span></span>

- <span data-ttu-id="d4f21-116">Создание страницы путем отправки запроса [`POST pages`](/graph/api/section-post-pages?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="d4f21-116">Create a page by sending a [`POST pages`](/graph/api/section-post-pages?view=graph-rest-1.0) request.</span></span>

- <span data-ttu-id="d4f21-117">Создание записной книжки путем отправки запроса [`POST notebooks`](/graph/api/onenote-post-notebooks?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="d4f21-117">Create a notebook by sending a [`POST notebooks`](/graph/api/onenote-post-notebooks?view=graph-rest-1.0) request.</span></span>

- <span data-ttu-id="d4f21-118">Получение метаданных страницы путем отправки запроса [`GET pages`](/graph/api/page-get?view=graph-rest-1.0) или [`GET pages/{id}`](/graph/api/page-get?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="d4f21-118">Get page metadata by sending a [`GET pages`](/graph/api/page-get?view=graph-rest-1.0) or [`GET pages/{id}`](/graph/api/page-get?view=graph-rest-1.0) request.</span></span>

- <span data-ttu-id="d4f21-119">Получение метаданных записной книжки путем отправки запроса [`GET notebooks`](/graph/api/notebook-get?view=graph-rest-1.0) или [`GET notebooks/{id}`](/graph/api/notebook-get?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="d4f21-119">Get notebook metadata by sending a [`GET notebooks`](/graph/api/notebook-get?view=graph-rest-1.0) or [`GET notebooks/{id}`](/graph/api/notebook-get?view=graph-rest-1.0) request.</span></span>

<span data-ttu-id="d4f21-120">В примерах ниже показано, как проверить код состояния ответа, проанализировать объект JSON, чтобы извлечь из него URL-адреса, а затем открыть клиент OneNote.</span><span class="sxs-lookup"><span data-stu-id="d4f21-120">The following examples show how to check the status code of the response, parse the JSON to extract the URLs, and then open the OneNote client.</span></span>

## <a name="ios-example"></a><span data-ttu-id="d4f21-121">Пример для iOS</span><span class="sxs-lookup"><span data-stu-id="d4f21-121">iOS example</span></span>

<span data-ttu-id="d4f21-122">В примере ниже показано, как получить URL-адреса клиента OneNote из ответа JSON.</span><span class="sxs-lookup"><span data-stu-id="d4f21-122">The following example gets the OneNote client URLs from the JSON response.</span></span> <span data-ttu-id="d4f21-123">Для извлечения двух URL-адресов в примере используется библиотека AFNetworking (https://afnetworking.com/)).</span><span class="sxs-lookup"><span data-stu-id="d4f21-123">It uses the AFNetworking library (https://afnetworking.com/) to extract the two URLs.</span></span> <span data-ttu-id="d4f21-124">В этом примере `created` представляет собой указатель на объект **ONSCPSStandardResponse**, используемый для хранения значений ответов, а в объекте `responseObject` содержится проанализированный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="d4f21-124">In the example, `created` is a pointer to the **ONSCPSStandardResponse** object used to store the response values, and `responseObject` holds the parsed JSON.</span></span>

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

<span data-ttu-id="d4f21-125">После того как вы проанализируете URL-адреса, полученные в ответе, вы сможете открыть OneNote, используя указанный ниже код.</span><span class="sxs-lookup"><span data-stu-id="d4f21-125">After you parse the URLs from the response, you can open OneNote by using the following code.</span></span> <span data-ttu-id="d4f21-126">Используйте `oneNoteClientUrl`, чтобы открыть установленный клиент OneNote, или `oneNoteWebURL`, чтобы открыть OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="d4f21-126">Use `oneNoteClientUrl` to open the installed OneNote client or `oneNoteWebURL` to open OneNote Online.</span></span>

```objc
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a><span data-ttu-id="d4f21-127">Пример для Android</span><span class="sxs-lookup"><span data-stu-id="d4f21-127">Android example</span></span>

<span data-ttu-id="d4f21-128">Прежде всего, проверьте наличие кода состояния успеха, а затем проанализируйте объект JSON.</span><span class="sxs-lookup"><span data-stu-id="d4f21-128">First, check for the success status code, and then parse the JSON.</span></span> <span data-ttu-id="d4f21-129">В примере предполагается, что был отправлен запрос POST, поэтому выполняется проверка наличия кода состояния `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="d4f21-129">The example assumes a POST request was sent, so it checks for a `201 Created` status code.</span></span> <span data-ttu-id="d4f21-130">Если вы создали запрос `GET`, то вместо этого проверьте наличие кода состояния `200`.</span><span class="sxs-lookup"><span data-stu-id="d4f21-130">If you made a `GET` request, check for a `200` status code instead.</span></span>

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

<span data-ttu-id="d4f21-131">С помощью свойств ответа ваше приложение может открыть OneNote Online, как показано в примере ниже.</span><span class="sxs-lookup"><span data-stu-id="d4f21-131">Using the response properties, your app can open OneNote Online, as shown in the following example.</span></span>

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

<br/>

<span data-ttu-id="d4f21-132">Кроме того, приложение может открыть клиент OneNote на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="d4f21-132">Or your app can open the OneNote client on an Android device.</span></span> <span data-ttu-id="d4f21-133">При использовании свойства `oneNoteClientUrl` перед запуском намерения необходимо поместить строки GUID в фигурные скобки `{ }`.</span><span class="sxs-lookup"><span data-stu-id="d4f21-133">When using the `oneNoteClientUrl` property, you must surround the GUID strings with braces `{ }` before starting the Intent.</span></span> <span data-ttu-id="d4f21-134">В примере ниже показано, как сделать это.</span><span class="sxs-lookup"><span data-stu-id="d4f21-134">The following example shows how to do that.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="d4f21-135">См. также</span><span class="sxs-lookup"><span data-stu-id="d4f21-135">See also</span></span>

- [<span data-ttu-id="d4f21-136">Получение содержимого и структуры OneNote</span><span class="sxs-lookup"><span data-stu-id="d4f21-136">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="d4f21-137">Создание страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="d4f21-137">Create OneNote pages</span></span>](onenote-create-page.md)

# <a name="open-the-onenote-client"></a><span data-ttu-id="fec83-101">Открытие клиента OneNote</span><span class="sxs-lookup"><span data-stu-id="fec83-101">Open the Postman client.</span></span>

<span data-ttu-id="fec83-102">Вы можете использовать свойство **links** страницы или записной книжки, чтобы открыть приложение OneNote на определенной странице или в определенной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="fec83-102">You can use the **links** property of a page or notebook to open a OneNote application to a particular page or notebook.</span></span> 

<span data-ttu-id="fec83-103">Свойство **links** представляет собой объект JSON, содержащий два URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="fec83-103">The **links** property is a JSON object that contains two URLs.</span></span> <span data-ttu-id="fec83-104">Эти URL-адреса открывают страницу или записную книжку в клиентском приложении OneNote или в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="fec83-104">The URLs will open the page or notebook in the OneNote client application or in OneNote Online.</span></span>

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

- <span data-ttu-id="fec83-105">**oneNoteClientUrl**: открывает клиент OneNote, если он установлен на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fec83-105">**oneNoteClientUrl** - Opens the OneNote client if it is already installed on the device.</span></span> <span data-ttu-id="fec83-106">Этот URL-адрес включает префикс *onenote*.</span><span class="sxs-lookup"><span data-stu-id="fec83-106">This URL includes the *onenote* prefix.</span></span>
<span data-ttu-id="fec83-107">Открывает версию для конкретного языка, если она установлена на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fec83-107">Opens the language-specific version if one is installed on the device.</span></span> <span data-ttu-id="fec83-108">В противном случае будет использован параметр языка платформы.</span><span class="sxs-lookup"><span data-stu-id="fec83-108">Otherwise, uses the platform language setting.</span></span>
- <span data-ttu-id="fec83-109">**oneNoteWebUrl**: открывает OneNote Online, если браузер, используемый по умолчанию на устройстве, поддерживает его.</span><span class="sxs-lookup"><span data-stu-id="fec83-109">**oneNoteWebUrl** - Opens OneNote Online if the default browser on the device supports it.</span></span> <span data-ttu-id="fec83-110">Использует параметр языка браузера.</span><span class="sxs-lookup"><span data-stu-id="fec83-110">Uses the browser language setting.</span></span>


<span data-ttu-id="fec83-111">API OneNote возвращает свойство **links** в HTTP-ответе для следующих операций:</span><span class="sxs-lookup"><span data-stu-id="fec83-111">The OneNote API returns the **links** property in the HTTP response for the following operations:</span></span>

- <span data-ttu-id="fec83-112">Создание страницы путем отправки запроса [`POST pages`](../api-reference/v1.0/api/section_post_pages.md).</span><span class="sxs-lookup"><span data-stu-id="fec83-112">Create a page by sending a [`POST pages`](../api-reference/v1.0/api/section_post_pages.md) request</span></span>
- <span data-ttu-id="fec83-113">Создание записной книжки путем отправки запроса [`POST notebooks`](../api-reference/v1.0/api/onenote_post_notebooks.md).</span><span class="sxs-lookup"><span data-stu-id="fec83-113">Create a notebook by sending a [`POST notebooks`](../api-reference/v1.0/api/onenote_post_notebooks.md) request</span></span>
- <span data-ttu-id="fec83-114">Получение метаданных страницы путем отправки запроса [`GET pages`](../api-reference/v1.0/api/page_get.md) или [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md).</span><span class="sxs-lookup"><span data-stu-id="fec83-114">Get page metadata by sending a [`GET pages`](../api-reference/v1.0/api/page_get.md) or [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md) request</span></span>
- <span data-ttu-id="fec83-115">Получение метаданных записной книжки путем отправки запроса [`GET notebooks`](../api-reference/v1.0/api/notebook_get.md) или [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md).</span><span class="sxs-lookup"><span data-stu-id="fec83-115">Get notebook metadata by sending a [`GET notebooks`](../api-reference/v1.0/api/notebook_get.md) or [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md) request</span></span>

<span data-ttu-id="fec83-116">В примерах ниже показано, как проверить код состояния ответа, проанализировать объект JSON, чтобы извлечь из него URL-адреса, а затем открыть клиент OneNote.</span><span class="sxs-lookup"><span data-stu-id="fec83-116">The following examples show how to check the status code of the response, parse the JSON to extract the URLs, and then open the OneNote client.</span></span>

## <a name="ios-example"></a><span data-ttu-id="fec83-117">Пример для iOS</span><span class="sxs-lookup"><span data-stu-id="fec83-117">iOS example</span></span>

<span data-ttu-id="fec83-118">В примере ниже показано, как получить URL-адреса клиента OneNote из ответа JSON.</span><span class="sxs-lookup"><span data-stu-id="fec83-118">The following example gets the OneNote client URLs from the JSON response.</span></span> <span data-ttu-id="fec83-119">Для извлечения двух URL-адресов в примере используется библиотека AFNetworking (http://afnetworking.com/).</span><span class="sxs-lookup"><span data-stu-id="fec83-119">It uses the AFNetworking library (http://afnetworking.com/) to extract the two URLs.</span></span> <span data-ttu-id="fec83-120">В этом примере `created` представляет собой указатель на объект ONSCPSStandardResponse, используемый для хранения значений ответов, а в объекте `responseObject` содержится проанализированный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="fec83-120">The following example gets the oncshort client URLs from the JSON response. It uses the AFNetworking library (http://afnetworking.com/http://afnetworking.com/) to extract the two URLs. In the example, created`created` is a pointer to the ONSCPSStandardResponse`responseObject` object used to store the response values, and responseObject holds the parsed JSON.</span></span>

```objectivec
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

<span data-ttu-id="fec83-121">После того как вы проанализируете URL-адреса, полученные в ответе, вы сможете открыть OneNote, используя указанный ниже код.</span><span class="sxs-lookup"><span data-stu-id="fec83-121">After you parse the URLs from the response, you can open OneNote by using the following code.</span></span> <span data-ttu-id="fec83-122">Используйте `oneNoteClientUrl`, чтобы открыть установленный клиент OneNote, или `oneNoteWebURL`, чтобы открыть OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="fec83-122">Use `oneNoteClientUrl` to open the installed OneNote client or `oneNoteWebURL` to open OneNote Online.</span></span>

```objectivec
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a><span data-ttu-id="fec83-123">Пример для Android</span><span class="sxs-lookup"><span data-stu-id="fec83-123">Android example</span></span>

<span data-ttu-id="fec83-124">Прежде всего, проверьте наличие кода состояния успеха, а затем проанализируйте объект JSON.</span><span class="sxs-lookup"><span data-stu-id="fec83-124">First, check for the success status code and then parse the JSON.</span></span> <span data-ttu-id="fec83-125">В примере предполагается, что был отправлен запрос POST, поэтому выполняется проверка наличия кода состояния `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="fec83-125">The example assumes a POST request was sent, so it checks for a `201 Created` status code.</span></span> <span data-ttu-id="fec83-126">Если вы создали запрос `GET`, то вместо этого проверьте наличие кода состояния `200`.</span><span class="sxs-lookup"><span data-stu-id="fec83-126">If you made a `GET` request, check for a `200` status code instead.</span></span>

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

<span data-ttu-id="fec83-127">С помощью свойств ответа ваше приложение может открыть OneNote Online, как показано в примере ниже.</span><span class="sxs-lookup"><span data-stu-id="fec83-127">Using the response properties, your app can open OneNote Online, as shown in the following example.</span></span>

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```
 
<span data-ttu-id="fec83-128">Кроме того, приложение может открыть клиент OneNote на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="fec83-128">Or your app can open the OneNote client on an Android device.</span></span> <span data-ttu-id="fec83-129">При использовании свойства `oneNoteClientUrl` перед запуском намерения необходимо поместить строки GUID в фигурные скобки `{ }`.</span><span class="sxs-lookup"><span data-stu-id="fec83-129">When using the `oneNoteClientUrl` property, you must surround the GUID strings with braces `{ }` before starting the Intent.</span></span> <span data-ttu-id="fec83-130">В примере ниже показано, как сделать это.</span><span class="sxs-lookup"><span data-stu-id="fec83-130">The following example shows how to:</span></span>

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

## <a name="see-also"></a><span data-ttu-id="fec83-131">См. также</span><span class="sxs-lookup"><span data-stu-id="fec83-131">See also</span></span>

- [<span data-ttu-id="fec83-132">Получение содержимого и структуры OneNote</span><span class="sxs-lookup"><span data-stu-id="fec83-132">Get OneNote content and structure</span></span>](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-get-content)
- [<span data-ttu-id="fec83-133">Создание страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="fec83-133">Create OneNote pages</span></span>](../api-reference/v1.0/api/section_post_pages.md)
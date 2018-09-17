# <a name="security-api-error-responses"></a><span data-ttu-id="a7468-101">Сообщения об ошибках безопасности API</span><span class="sxs-lookup"><span data-stu-id="a7468-101">Security API error responses</span></span>

<span data-ttu-id="a7468-102">Ошибки в API безопасности в Microsoft Graph выводятся с использованием стандартных кодов состояния HTTP и представлены в виде заголовка предупреждения.</span><span class="sxs-lookup"><span data-stu-id="a7468-102">Errors in the security API in Microsoft Graph are returned using standard HTTP status codes and are delivered by way of a warning header.</span></span>

<span data-ttu-id="a7468-103">API безопасности – это федеративная служба, в которую поступают ответы от всех поставщиков данных.</span><span class="sxs-lookup"><span data-stu-id="a7468-103">The security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="a7468-104">Если API безопасности получает ошибку HTTP, он отправляет заголовок предупреждение в следующем формате: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="a7468-104">When an HTTP error is received by the security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="a7468-105">Этот заголовок предупреждение отправляется клиентам, только если один из поставщиков данных выдает код ошибки, отличный от 2xx или 404.</span><span class="sxs-lookup"><span data-stu-id="a7468-105">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="a7468-106">Примеры:</span><span class="sxs-lookup"><span data-stu-id="a7468-106">For example:</span></span>

- <span data-ttu-id="a7468-107">Предупреждение HttpStatusCode.Forbidden (403) выводится, если не предоставляется доступ к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="a7468-107">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="a7468-108">Если истекает время ожидания поставщика, в заголовке предупреждения выводится HttpStatusCode.GatewayTimeout (504).</span><span class="sxs-lookup"><span data-stu-id="a7468-108">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="a7468-109">В случае внутренней ошибки поставщика в заголовке предупреждения используется HttpStatusCode.InternalServerError (500).</span><span class="sxs-lookup"><span data-stu-id="a7468-109">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="a7468-110">Если в ответе поставщика данных выводятся коды 2xx или 404, они не отображаются в заголовке предупреждения, так как они означают, что либо операция выполнена успешно, либо данные не найдены, соответственно.</span><span class="sxs-lookup"><span data-stu-id="a7468-110">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="a7468-111">В федеративной системе код "404 not found" встречается столько раз, сколько данные оказываются известны только одному или нескольким, но не всем поставщикам.</span><span class="sxs-lookup"><span data-stu-id="a7468-111">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="a7468-112">Пример</span><span class="sxs-lookup"><span data-stu-id="a7468-112">Example</span></span>

<span data-ttu-id="a7468-113">Пользователь запрашивает `security/alerts/{alert_id}`.</span><span class="sxs-lookup"><span data-stu-id="a7468-113">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="a7468-114">Так как коды 404 и 200 являются ожидаемыми условиями, заголовок предупреждения содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a7468-114">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span> 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/29000",    (usual timeout limit is set at 29 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="a7468-115">**Примечание.** Каждый заголовок HTTP — это набор элементов, так что пользователи могут просмотреть номер заголовка предупреждения и проверить все элементы.</span><span class="sxs-lookup"><span data-stu-id="a7468-115">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="see-also"></a><span data-ttu-id="a7468-116">См. также</span><span class="sxs-lookup"><span data-stu-id="a7468-116">See also</span></span>

<span data-ttu-id="a7468-117">Если у вас возникли сложности с авторизацией, см. запись в нашем [блоге](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span><span class="sxs-lookup"><span data-stu-id="a7468-117">If you’re having trouble with authorization, see our [blog post](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span></span>

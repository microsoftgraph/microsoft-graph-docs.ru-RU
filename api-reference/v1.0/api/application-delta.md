---
title: 'application: delta'
description: Создайте, обновим или удаляйте приложения, не выполняя полное чтение всей коллекции ресурсов.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8640221a136d6b19391e146b4d3d24a5a7daa974
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132523"
---
# <a name="application-delta"></a><span data-ttu-id="d469d-103">application: delta</span><span class="sxs-lookup"><span data-stu-id="d469d-103">application: delta</span></span>

<span data-ttu-id="d469d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d469d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d469d-105">Создавайте, обновляйте или удаляйте приложения без необходимости чтения всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d469d-105">Get newly created, updated, or deleted applications without performing a full read of the entire resource collection.</span></span> <span data-ttu-id="d469d-106">Подробные сведения см. [в под вопросе "Использование разнонали бытовего запроса".](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="d469d-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="d469d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d469d-107">Permissions</span></span>

<span data-ttu-id="d469d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d469d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d469d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d469d-110">Permission type</span></span>      | <span data-ttu-id="d469d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d469d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d469d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d469d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d469d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d469d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d469d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d469d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d469d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d469d-115">Not supported.</span></span>    |
|<span data-ttu-id="d469d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d469d-116">Application</span></span> | <span data-ttu-id="d469d-117">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d469d-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d469d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d469d-118">HTTP request</span></span>

<span data-ttu-id="d469d-119">Чтобы начать отслеживание изменений, необходимо внести запрос, включив функцию delta в **ресурсе** приложения.</span><span class="sxs-lookup"><span data-stu-id="d469d-119">To begin tracking changes, you make a request including the delta function on the **application** resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

## <a name="query-parameters"></a><span data-ttu-id="d469d-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="d469d-120">Query parameters</span></span>

<span data-ttu-id="d469d-121">Отслеживание изменений вызывает один или несколько вызовов **функции delta.**</span><span class="sxs-lookup"><span data-stu-id="d469d-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="d469d-122">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="d469d-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="d469d-123">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="d469d-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="d469d-124">Все параметры запроса необходимо указать только один раз за передним.</span><span class="sxs-lookup"><span data-stu-id="d469d-124">You only need to specify any query parameters once up front.</span></span> <span data-ttu-id="d469d-125">В последующих запросах скопируйте и примените `nextLink` `deltaLink` URL-адрес из предыдущего ответа.</span><span class="sxs-lookup"><span data-stu-id="d469d-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="d469d-126">Этот URL-адрес уже содержит закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="d469d-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="d469d-127">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="d469d-127">Query parameter</span></span>      | <span data-ttu-id="d469d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="d469d-128">Type</span></span>   |<span data-ttu-id="d469d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d469d-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d469d-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="d469d-130">$deltatoken</span></span> | <span data-ttu-id="d469d-131">string</span><span class="sxs-lookup"><span data-stu-id="d469d-131">string</span></span> | <span data-ttu-id="d469d-132">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адресе предыдущего вызова функции delta для той же коллекции ресурсов, что указывает на завершение этого круга `deltaLink` отслеживания  изменений.</span><span class="sxs-lookup"><span data-stu-id="d469d-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="d469d-133">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="d469d-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="d469d-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="d469d-134">$skiptoken</span></span> | <span data-ttu-id="d469d-135">string</span><span class="sxs-lookup"><span data-stu-id="d469d-135">string</span></span> | <span data-ttu-id="d469d-136">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адресе предыдущего вызова функции delta, указывающий на то, что в той же коллекции ресурсов отслеживаются `nextLink` дополнительные  изменения.</span><span class="sxs-lookup"><span data-stu-id="d469d-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="d469d-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d469d-137">Optional query parameters</span></span>

<span data-ttu-id="d469d-138">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d469d-138">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="d469d-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="d469d-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span>
- <span data-ttu-id="d469d-141">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="d469d-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="d469d-142">Единственное поддерживаемые выражения — отслеживание изменений для `$filter` определенных ресурсов по их ИД:  `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="d469d-142">The only supported `$filter` expression is for tracking changes for specific resources, by their ID:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="d469d-143">Количество указываемого количества ИД ограничено максимальной длиной URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="d469d-143">The number of IDs you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d469d-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d469d-144">Request headers</span></span>
| <span data-ttu-id="d469d-145">Имя</span><span class="sxs-lookup"><span data-stu-id="d469d-145">Name</span></span>       | <span data-ttu-id="d469d-146">Описание</span><span class="sxs-lookup"><span data-stu-id="d469d-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d469d-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="d469d-147">Authorization</span></span>  | <span data-ttu-id="d469d-148">Носитель &lt;токен&gt;.</span><span class="sxs-lookup"><span data-stu-id="d469d-148">Bearer &lt;token&gt;.</span></span> <span data-ttu-id="d469d-149">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d469d-149">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d469d-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d469d-150">Request body</span></span>
<span data-ttu-id="d469d-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d469d-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d469d-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d469d-152">Response</span></span>

<span data-ttu-id="d469d-153">В случае успеха этот метод возвращает код отклика и объект коллекции приложений `200 OK` в тексте [](../resources/application.md) отклика.</span><span class="sxs-lookup"><span data-stu-id="d469d-153">If successful, this method returns a `200 OK` response code and an [application](../resources/application.md) collection object in the response body.</span></span> <span data-ttu-id="d469d-154">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="d469d-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="d469d-155">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="d469d-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="d469d-156">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="d469d-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="d469d-157">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="d469d-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="d469d-158">Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях ресурса в будущем.</span><span class="sxs-lookup"><span data-stu-id="d469d-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="d469d-159">Подробные сведения см. [в под вопросе "Использование разнонали бытовего запроса".](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="d469d-159">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="d469d-160">Примеры запросов см. в подстановок ["Получить добавонные изменения для пользователей".](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="d469d-160">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="d469d-161">Пример</span><span class="sxs-lookup"><span data-stu-id="d469d-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="d469d-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="d469d-162">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d469d-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d469d-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/delta
```
# <a name="c"></a>[<span data-ttu-id="d469d-164">C#</span><span class="sxs-lookup"><span data-stu-id="d469d-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d469d-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d469d-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d469d-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d469d-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d469d-167">Java</span><span class="sxs-lookup"><span data-stu-id="d469d-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d469d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="d469d-168">Response</span></span>
><span data-ttu-id="d469d-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d469d-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


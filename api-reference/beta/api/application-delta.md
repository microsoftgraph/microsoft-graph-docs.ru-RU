---
title: 'Приложение: Delta'
description: Получите только что созданные, обновленные или удаленные приложения без полного считывания всей коллекции ресурсов. Сведения об использовании запроса изменений см.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 13b6f7809cf47edcc9de8c9ddfb052645b15f25a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459257"
---
# <a name="application-delta"></a><span data-ttu-id="12749-104">Приложение: Delta</span><span class="sxs-lookup"><span data-stu-id="12749-104">application: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12749-105">Получите только что созданные, обновленные или удаленные приложения без полного считывания всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="12749-105">Get newly created, updated, or deleted applications without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="12749-106">Сведения об [использовании запроса изменений](/graph/delta-query-overview) см.</span><span class="sxs-lookup"><span data-stu-id="12749-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="12749-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12749-107">Permissions</span></span>

<span data-ttu-id="12749-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12749-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="12749-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12749-110">Permission type</span></span>      | <span data-ttu-id="12749-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12749-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12749-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12749-112">Delegated (work or school account)</span></span> | <span data-ttu-id="12749-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12749-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12749-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12749-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12749-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12749-115">Not supported.</span></span>    |
|<span data-ttu-id="12749-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12749-116">Application</span></span> | <span data-ttu-id="12749-117">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="12749-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12749-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12749-118">HTTP request</span></span>

<span data-ttu-id="12749-119">Чтобы начать отслеживание изменений, необходимо создать запрос, включающий функцию Delta для ресурса Application.</span><span class="sxs-lookup"><span data-stu-id="12749-119">To begin tracking changes, you make a request including the delta function on the application resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

### <a name="query-parameters"></a><span data-ttu-id="12749-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="12749-120">Query parameters</span></span>

<span data-ttu-id="12749-121">Отслеживание изменений приводит к округлению одного или нескольких вызовов функции **Delta** .</span><span class="sxs-lookup"><span data-stu-id="12749-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="12749-122">Если вы используете любой параметр запроса (кроме `$deltatoken` и `$skiptoken`), необходимо указать его в исходном запросе **Delta** .</span><span class="sxs-lookup"><span data-stu-id="12749-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="12749-123">Microsoft Graph автоматически кодирует все заданные параметры в часть маркера или `nextLink` `deltaLink` URL-адрес, указанный в ответе.</span><span class="sxs-lookup"><span data-stu-id="12749-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="12749-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="12749-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="12749-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="12749-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="12749-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="12749-126">Query parameter</span></span>      | <span data-ttu-id="12749-127">Тип</span><span class="sxs-lookup"><span data-stu-id="12749-127">Type</span></span>   |<span data-ttu-id="12749-128">Описание</span><span class="sxs-lookup"><span data-stu-id="12749-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="12749-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="12749-129">$deltatoken</span></span> | <span data-ttu-id="12749-130">строка</span><span class="sxs-lookup"><span data-stu-id="12749-130">string</span></span> | <span data-ttu-id="12749-131">[Токен состояния](/graph/delta-query-overview) возвращается в `deltaLink` URL-адресе предыдущего вызова функции **Delta** для той же коллекции ресурсов, что указывает на завершение этого круга отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="12749-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="12749-132">Сохраните и примените весь `deltaLink` URL-адрес, включая этот маркер, в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="12749-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="12749-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="12749-133">$skiptoken</span></span> | <span data-ttu-id="12749-134">string</span><span class="sxs-lookup"><span data-stu-id="12749-134">string</span></span> | <span data-ttu-id="12749-135">[Токен состояния](/graph/delta-query-overview) возвращается в `nextLink` URL-адресе предыдущего вызова функции **Delta** , указывая, что в коллекции ресурсов отслеживаются другие изменения.</span><span class="sxs-lookup"><span data-stu-id="12749-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="12749-136">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="12749-136">Optional query parameters</span></span>

<span data-ttu-id="12749-137">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="12749-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="12749-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="12749-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="12749-140">Существует ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="12749-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="12749-141">Единственное поддерживаемое `$filter` выражение предназначено для отслеживания изменений для определенных ресурсов по их идентификаторам: `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="12749-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="12749-142">Количество идентификаторов, которые можно указать, ограничено максимальной длиной URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="12749-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="12749-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12749-143">Request headers</span></span>
| <span data-ttu-id="12749-144">Имя</span><span class="sxs-lookup"><span data-stu-id="12749-144">Name</span></span>       | <span data-ttu-id="12749-145">Описание</span><span class="sxs-lookup"><span data-stu-id="12749-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="12749-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12749-146">Authorization</span></span>  | <span data-ttu-id="12749-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="12749-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="12749-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12749-148">Content-Type</span></span>  | <span data-ttu-id="12749-149">application/json</span><span class="sxs-lookup"><span data-stu-id="12749-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="12749-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12749-150">Request body</span></span>
<span data-ttu-id="12749-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12749-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="12749-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="12749-152">Response</span></span>

<span data-ttu-id="12749-153">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект коллекции [приложения](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12749-153">If successful, this method returns `200 OK` response code and [application](../resources/application.md) collection object in the response body.</span></span> <span data-ttu-id="12749-154">Ответ также включает URL-адрес nextLink или URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="12749-154">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="12749-155">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="12749-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="12749-156">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="12749-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="12749-157">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="12749-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="12749-158">Следует оставить и использовать `deltaLink` URL-адрес для получения сведений об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="12749-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="12749-159">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="12749-159">See:</span></span></br>
- <span data-ttu-id="12749-160">[Дополнительные сведения](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="12749-160">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="12749-161">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="12749-161">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="12749-162">Пример</span><span class="sxs-lookup"><span data-stu-id="12749-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12749-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="12749-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```http
GET https://graph.microsoft.com/beta/applications/delta
```

##### <a name="response"></a><span data-ttu-id="12749-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="12749-164">Response</span></span>
<span data-ttu-id="12749-p111">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12749-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/beta/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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
    "Error: /api-reference/beta/api/application-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

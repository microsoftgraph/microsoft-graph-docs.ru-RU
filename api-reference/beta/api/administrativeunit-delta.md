---
title: 'administrativeUnit: Delta'
description: Получите только что созданные, обновленные или удаленные административные единицы, не требуя полного считывания всей коллекции ресурсов.
localization_priority: Normal
author: anandyadavMSFT
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3db487f3b8583c0fc25ab5ef834d1e10479c0d35
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43510617"
---
# <a name="administrativeunit-delta"></a><span data-ttu-id="5681e-103">administrativeUnit: Delta</span><span class="sxs-lookup"><span data-stu-id="5681e-103">administrativeUnit: delta</span></span>

<span data-ttu-id="5681e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5681e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5681e-105">Получите только что созданный, обновленный или удаленный **административеунитс** , не требуя полного считывания всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5681e-105">Get newly created, updated, or deleted **administrativeUnits** without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="5681e-106">Подробнее: [Использование запроса изменений](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="5681e-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="5681e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5681e-107">Permissions</span></span>

<span data-ttu-id="5681e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5681e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5681e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5681e-110">Permission type</span></span>      | <span data-ttu-id="5681e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5681e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5681e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5681e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5681e-113">AdministrativeUnit. Read. ALL, Directory. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="5681e-113">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5681e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5681e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5681e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5681e-115">Not supported.</span></span>    |
|<span data-ttu-id="5681e-116">administrativeunit</span><span class="sxs-lookup"><span data-stu-id="5681e-116">administrativeunit</span></span> | <span data-ttu-id="5681e-117">AdministrativeUnit. Read. ALL, Directory. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5681e-117">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5681e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5681e-118">HTTP request</span></span>

<span data-ttu-id="5681e-119">Чтобы начать отслеживание изменений, необходимо создать запрос, включающий функцию Delta в ресурсе **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="5681e-119">To begin tracking changes, you make a request that includes the delta function on the **administrativeUnit** resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /administrativeunits/delta
```

## <a name="query-parameters"></a><span data-ttu-id="5681e-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="5681e-120">Query parameters</span></span>

<span data-ttu-id="5681e-121">Отслеживание изменений приводит к округлению одного или нескольких вызовов функции **Delta** .</span><span class="sxs-lookup"><span data-stu-id="5681e-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="5681e-122">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="5681e-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="5681e-123">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="5681e-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="5681e-124">Необходимо указать только один из параметров запроса на передний план.</span><span class="sxs-lookup"><span data-stu-id="5681e-124">You only need to specify any query parameters once up front.</span></span> <span data-ttu-id="5681e-125">В последующих запросах скопируйте и примените `nextLink` `deltaLink` URL-адрес из предыдущего ответа.</span><span class="sxs-lookup"><span data-stu-id="5681e-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="5681e-126">Этот URL-адрес уже включает в себя зашифрованные параметры.</span><span class="sxs-lookup"><span data-stu-id="5681e-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="5681e-127">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="5681e-127">Query parameter</span></span>      | <span data-ttu-id="5681e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="5681e-128">Type</span></span>   |<span data-ttu-id="5681e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="5681e-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5681e-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="5681e-130">$deltatoken</span></span> | <span data-ttu-id="5681e-131">string</span><span class="sxs-lookup"><span data-stu-id="5681e-131">string</span></span> | <span data-ttu-id="5681e-132">[Токен состояния](/graph/delta-query-overview) возвращается в `deltaLink` URL-адресе предыдущего вызова функции **Delta** для той же коллекции ресурсов, что указывает на завершение этого круга отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="5681e-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="5681e-133">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="5681e-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="5681e-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="5681e-134">$skiptoken</span></span> | <span data-ttu-id="5681e-135">string</span><span class="sxs-lookup"><span data-stu-id="5681e-135">string</span></span> | <span data-ttu-id="5681e-136">[Токен состояния](/graph/delta-query-overview) возвращается в `nextLink` URL-адресе предыдущего вызова функции **Delta** , указывая, что в коллекции ресурсов отслеживаются другие изменения.</span><span class="sxs-lookup"><span data-stu-id="5681e-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="5681e-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5681e-137">Optional query parameters</span></span>

<span data-ttu-id="5681e-138">Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5681e-138">This method supports the following OData query parameters to help customize the response:</span></span>

- <span data-ttu-id="5681e-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="5681e-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span> 

- <span data-ttu-id="5681e-141">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="5681e-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="5681e-142">Единственное поддерживаемое `$filter` выражение предназначено для отслеживания изменений для определенных ресурсов по их идентификаторам: `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="5681e-142">The only supported `$filter` expression is for tracking changes for specific resources, by their ID:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="5681e-143">Количество идентификаторов, которые можно указать, ограничено максимальной длиной URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="5681e-143">The number of IDs you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="5681e-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5681e-144">Request headers</span></span>
| <span data-ttu-id="5681e-145">Имя</span><span class="sxs-lookup"><span data-stu-id="5681e-145">Name</span></span>       | <span data-ttu-id="5681e-146">Описание</span><span class="sxs-lookup"><span data-stu-id="5681e-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5681e-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="5681e-147">Authorization</span></span>  | <span data-ttu-id="5681e-148">Носитель &lt;токен&gt;.</span><span class="sxs-lookup"><span data-stu-id="5681e-148">Bearer &lt;token&gt;.</span></span> <span data-ttu-id="5681e-149">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="5681e-149">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5681e-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5681e-150">Request body</span></span>
<span data-ttu-id="5681e-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5681e-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5681e-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="5681e-152">Response</span></span>

<span data-ttu-id="5681e-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [administrativeUnit](../resources/administrativeunit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5681e-153">If successful, this method returns `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) collection object in the response body.</span></span> <span data-ttu-id="5681e-154">Оклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="5681e-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span> 

- <span data-ttu-id="5681e-155">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="5681e-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="5681e-156">**AdministrativeUnit** продолжает совершать запросы, используя `nextLink` URL-адрес, пока `deltaLink` в ответ не будет включен URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="5681e-156">The **administrativeUnit** continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="5681e-157">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="5681e-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="5681e-158">Следует оставить и использовать `deltaLink` URL-адрес для получения сведений об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="5681e-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="5681e-159">Для получения дополнительных сведений и примера обратитесь к разделу [Использование разностного запроса](/graph/delta-query-overview) и [получение добавочных изменений для пользователей](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="5681e-159">For details and an example, see [Using delta query](/graph/delta-query-overview) and [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="5681e-160">Пример</span><span class="sxs-lookup"><span data-stu-id="5681e-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="5681e-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="5681e-161">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5681e-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="5681e-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "administrativeunit_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeunits/delta
```
# <a name="c"></a>[<span data-ttu-id="5681e-163">C#</span><span class="sxs-lookup"><span data-stu-id="5681e-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/administrativeunit-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5681e-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5681e-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/administrativeunit-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5681e-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5681e-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/administrativeunit-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5681e-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="5681e-166">Response</span></span>
><span data-ttu-id="5681e-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5681e-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#administrativeunits",
  "@odata.nextLink":"https://graph.microsoft.com/beta/administrativeunits/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "Management Fast Track",
      "visibility": null,
      "extension_fe2174665583431c953114ff7268b7b3_Education_ObjectType": "School",
      "extension_fe2174665583431c953114ff7268b7b3_Education_StateId": "WA",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Address": "2 Microsoft Way",
      "extension_fe2174665583431c953114ff7268b7b3_Education_City": "Redmond",
      "extension_fe2174665583431c953114ff7268b7b3_Education_State": "WA",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Country": "US",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Zip": "98052",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Phone": "555-123-4567",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SyncSource": "SIS",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SyncSource_SchoolId": "10002",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalSyncSourceId": "14008",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalName": "Amy Roebuck",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalEmail": "aroebuck@principal.edu",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolZone": "1",
      "id": "8a07f5a8-edc9-4847-bbf2-dde106594bf4",
      "members@delta": [
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "b66ecf79-a093-4d51-86e0-efcc4531f37a"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "5bde3e51-d13b-4db1-9948-fe4b109d11a7"
        },
        {
            "@odata.type": "#microsoft.graph.group",
            "id": "801f2093-de7e-4883-a786-8a5f30874ff4"
        },
        {
            "@odata.type": "#microsoft.graph.group",
            "id": "7e4ec76c-8276-43ef-ba10-9aaa197cb212"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "f5289423-7233-4d60-831a-fe107a8551cc"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "48d31887-5fad-4d73-a9f5-3c356e68a038"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "c03e6eaa-b6ab-46d7-905b-73ec7ea1f755"
        }
      ]
  }
  ]
}
```

<!-- uuid: 69848a18-6b48-44fd-a398-4521803a0a00
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "administrativeunit: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

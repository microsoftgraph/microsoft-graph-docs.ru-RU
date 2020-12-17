---
title: Перечисление servicePrincipal memberOf
description: Список групп и ролей каталога, непосредственным участником которых является этот субъект-служба. Эта операция не является транзитивной.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: ff4e06c00870999b31aadd9c65d65cb53b30392d
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082267"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="da99e-104">Перечисление servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="da99e-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="da99e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da99e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da99e-106">Список групп и ролей каталога, непосредственным участником которых является этот [субъект-служба](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="da99e-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="da99e-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="da99e-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="da99e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da99e-108">Permissions</span></span>

<span data-ttu-id="da99e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da99e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da99e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da99e-111">Permission type</span></span>      | <span data-ttu-id="da99e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da99e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da99e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da99e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="da99e-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="da99e-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="da99e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da99e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da99e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da99e-116">Not supported.</span></span>    |
|<span data-ttu-id="da99e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da99e-117">Application</span></span> | <span data-ttu-id="da99e-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da99e-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="da99e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da99e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da99e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="da99e-120">Optional query parameters</span></span>

<span data-ttu-id="da99e-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="da99e-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="da99e-122">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="da99e-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="da99e-123">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="da99e-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="da99e-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="da99e-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="da99e-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="da99e-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da99e-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da99e-126">Request headers</span></span>
| <span data-ttu-id="da99e-127">Имя</span><span class="sxs-lookup"><span data-stu-id="da99e-127">Name</span></span>           | <span data-ttu-id="da99e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="da99e-128">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="da99e-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da99e-129">Authorization</span></span>  | <span data-ttu-id="da99e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da99e-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da99e-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="da99e-132">ConsistencyLevel</span></span> | <span data-ttu-id="da99e-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="da99e-133">eventual.</span></span> <span data-ttu-id="da99e-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="da99e-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="da99e-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="da99e-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da99e-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da99e-136">Request body</span></span>

<span data-ttu-id="da99e-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da99e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da99e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="da99e-138">Response</span></span>

<span data-ttu-id="da99e-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da99e-139">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da99e-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="da99e-140">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="da99e-141">Пример 1: Список групп и ролей каталога, непосредственным участником которых является этот субъект-служба</span><span class="sxs-lookup"><span data-stu-id="da99e-141">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="da99e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="da99e-142">Request</span></span>

<span data-ttu-id="da99e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da99e-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da99e-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="da99e-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="da99e-145">C#</span><span class="sxs-lookup"><span data-stu-id="da99e-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da99e-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da99e-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da99e-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da99e-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da99e-148">Java</span><span class="sxs-lookup"><span data-stu-id="da99e-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="da99e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="da99e-149">Response</span></span>

<span data-ttu-id="da99e-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da99e-150">The following is an example of the response.</span></span>

> <span data-ttu-id="da99e-151">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="da99e-151">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="da99e-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da99e-152">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="da99e-153">Пример 2: Получение только количества участников</span><span class="sxs-lookup"><span data-stu-id="da99e-153">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="da99e-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="da99e-154">Request</span></span>

<span data-ttu-id="da99e-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da99e-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="da99e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="da99e-156">Response</span></span>

<span data-ttu-id="da99e-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="da99e-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="da99e-158">Пример 3. Использование OData cast для получения только количества участия в группах</span><span class="sxs-lookup"><span data-stu-id="da99e-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="da99e-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="da99e-159">Request</span></span>

<span data-ttu-id="da99e-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da99e-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="da99e-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="da99e-161">Response</span></span>

<span data-ttu-id="da99e-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da99e-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="da99e-163">Пример 4: Использование параметра $search и OData cast для получения участия в группах с отображаемыми именами, содержащими буквы "Video", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="da99e-163">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="da99e-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="da99e-164">Request</span></span>

<span data-ttu-id="da99e-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da99e-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET iv. https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="da99e-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="da99e-166">Response</span></span>

<span data-ttu-id="da99e-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da99e-167">The following is an example of the response.</span></span>

><span data-ttu-id="da99e-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da99e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "@odata.count":1396,
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="da99e-170">Пример 5: Использование параметра $search и OData cast для получения участия в группах с отображаемым именем, которое начинается на «а», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="da99e-170">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="da99e-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="da99e-171">Request</span></span>

<span data-ttu-id="da99e-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da99e-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="da99e-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="da99e-173">Response</span></span>

<span data-ttu-id="da99e-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da99e-174">The following is an example of the response.</span></span>

><span data-ttu-id="da99e-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da99e-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "@odata.count":76,
  "value":[
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

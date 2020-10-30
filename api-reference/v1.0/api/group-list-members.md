---
title: Список участников
description: Получение списка непосредственных участников группы. Участниками группы могут быть пользователи, контакты организации, устройства, субъекты-службы и другие группы.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fce71e0caa13e5b1ba7ac4bf5aab41ecd2e96357
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782555"
---
# <a name="list-members"></a><span data-ttu-id="adeef-104">Список участников</span><span class="sxs-lookup"><span data-stu-id="adeef-104">List members</span></span>

<span data-ttu-id="adeef-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adeef-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="adeef-106">Получение списка непосредственных участников группы.</span><span class="sxs-lookup"><span data-stu-id="adeef-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="adeef-107">Участниками группы могут быть пользователи, контакты организации, устройства, субъекты-службы и другие группы.</span><span class="sxs-lookup"><span data-stu-id="adeef-107">A group can have users, organizational contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="adeef-108">В настоящее время субъекты-службы не указаны как участники группы благодаря поэтапному развертыванию субъектов-служб в конечной точке Microsoft Graph версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="adeef-108">Currently service principals are not listed as group members due to staged roll-out of service principals on Graph V1.0 endpoint.</span></span> <span data-ttu-id="adeef-109">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="adeef-109">This operation is not transitive.</span></span>

<span data-ttu-id="adeef-110">Если группа содержит более 100 участников, Microsoft Graph возвращает в отклике свойство `@odata.nextLink`, содержащее URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="adeef-110">When a group contains more than 100 members, Microsoft Graph returns a `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="adeef-111">При наличии этого свойства продолжайте выполнять дополнительные запросы с URL-адресом `@odata.nextLink` в каждом отклике, пока не будут возвращены все результаты, как описано в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="adeef-111">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="adeef-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="adeef-112">Permissions</span></span>
<span data-ttu-id="adeef-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adeef-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adeef-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adeef-115">Permission type</span></span>      | <span data-ttu-id="adeef-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="adeef-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adeef-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adeef-117">Delegated (work or school account)</span></span> | <span data-ttu-id="adeef-118">User.ReadBasic.All, User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="adeef-118">User.ReadBasic.All, User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="adeef-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adeef-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adeef-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adeef-120">Not supported.</span></span>    |
|<span data-ttu-id="adeef-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adeef-121">Application</span></span> | <span data-ttu-id="adeef-122">User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="adeef-122">User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="adeef-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adeef-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="adeef-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="adeef-124">Optional query parameters</span></span>
<span data-ttu-id="adeef-125">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="adeef-125">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="adeef-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="adeef-126">Request headers</span></span>
| <span data-ttu-id="adeef-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="adeef-127">Header</span></span>       | <span data-ttu-id="adeef-128">Значение</span><span class="sxs-lookup"><span data-stu-id="adeef-128">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="adeef-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="adeef-129">Authorization</span></span>  | <span data-ttu-id="adeef-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="adeef-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adeef-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="adeef-132">Request body</span></span>
<span data-ttu-id="adeef-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="adeef-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adeef-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="adeef-134">Response</span></span>
<span data-ttu-id="adeef-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="adeef-135">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adeef-136">Пример</span><span class="sxs-lookup"><span data-stu-id="adeef-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="adeef-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="adeef-137">Request</span></span>
<span data-ttu-id="adeef-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adeef-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="adeef-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="adeef-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="adeef-140">C#</span><span class="sxs-lookup"><span data-stu-id="adeef-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adeef-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adeef-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adeef-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adeef-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adeef-143">Java</span><span class="sxs-lookup"><span data-stu-id="adeef-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="adeef-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="adeef-144">Response</span></span>
<span data-ttu-id="adeef-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="adeef-145">The following is an example of the response.</span></span>
><span data-ttu-id="adeef-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="adeef-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


---
title: Список членов группы
description: Получение списка непосредственных участников группы. У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников. Эта операция не является транзитивной.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 25f2585647e81afdf4abb9a2257b9548f1847c37
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419431"
---
# <a name="list-group-members"></a><span data-ttu-id="d7884-105">Список членов группы</span><span class="sxs-lookup"><span data-stu-id="d7884-105">List group members</span></span>

<span data-ttu-id="d7884-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d7884-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7884-107">Получение списка непосредственных участников группы.</span><span class="sxs-lookup"><span data-stu-id="d7884-107">Get a list of the group's direct members.</span></span> <span data-ttu-id="d7884-108">У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="d7884-108">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="d7884-109">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="d7884-109">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7884-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7884-110">Permissions</span></span>

<span data-ttu-id="d7884-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7884-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7884-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7884-113">Permission type</span></span>      | <span data-ttu-id="d7884-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7884-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7884-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7884-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d7884-116">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7884-116">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="d7884-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7884-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7884-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7884-118">Not supported.</span></span>    |
|<span data-ttu-id="d7884-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7884-119">Application</span></span> | <span data-ttu-id="d7884-120">Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7884-120">Group.Read.All, Directory.Read.All</span></span> |

> <span data-ttu-id="d7884-121">Note: чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="d7884-121">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="d7884-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7884-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7884-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d7884-123">Optional query parameters</span></span>
<span data-ttu-id="d7884-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d7884-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7884-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7884-125">Request headers</span></span>
| <span data-ttu-id="d7884-126">Имя</span><span class="sxs-lookup"><span data-stu-id="d7884-126">Name</span></span>       | <span data-ttu-id="d7884-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d7884-127">Type</span></span> | <span data-ttu-id="d7884-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d7884-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d7884-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7884-129">Authorization</span></span>  | <span data-ttu-id="d7884-130">string</span><span class="sxs-lookup"><span data-stu-id="d7884-130">string</span></span>  | <span data-ttu-id="d7884-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7884-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7884-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7884-133">Request body</span></span>
<span data-ttu-id="d7884-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7884-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7884-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7884-135">Response</span></span>
<span data-ttu-id="d7884-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7884-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7884-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d7884-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d7884-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7884-138">Request</span></span>
<span data-ttu-id="d7884-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7884-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d7884-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7884-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="d7884-141">C#</span><span class="sxs-lookup"><span data-stu-id="d7884-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7884-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7884-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7884-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7884-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7884-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7884-144">Response</span></span>
<span data-ttu-id="d7884-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d7884-145">The following is an example of the response.</span></span>
><span data-ttu-id="d7884-146">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d7884-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d7884-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7884-147">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user",
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

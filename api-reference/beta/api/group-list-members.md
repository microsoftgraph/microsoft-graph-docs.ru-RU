---
title: Список членов группы
description: Получение списка непосредственных участников группы. У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников. Эта операция не является транзитивной.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4d74380ab35e90002af2919b67b63b4a50fb7dcd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869631"
---
# <a name="list-group-members"></a><span data-ttu-id="a0553-105">Список членов группы</span><span class="sxs-lookup"><span data-stu-id="a0553-105">List group members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0553-106">Получение списка непосредственных участников группы.</span><span class="sxs-lookup"><span data-stu-id="a0553-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="a0553-107">У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="a0553-107">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="a0553-108">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="a0553-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0553-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0553-109">Permissions</span></span>

<span data-ttu-id="a0553-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0553-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0553-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0553-112">Permission type</span></span>      | <span data-ttu-id="a0553-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0553-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0553-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0553-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a0553-115">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0553-115">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="a0553-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0553-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0553-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0553-117">Not supported.</span></span>    |
|<span data-ttu-id="a0553-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0553-118">Application</span></span> | <span data-ttu-id="a0553-119">Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0553-119">Group.Read.All, Directory.Read.All</span></span> |

> <span data-ttu-id="a0553-120">Note: чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="a0553-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="a0553-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0553-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0553-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a0553-122">Optional query parameters</span></span>
<span data-ttu-id="a0553-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a0553-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0553-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0553-124">Request headers</span></span>
| <span data-ttu-id="a0553-125">Имя</span><span class="sxs-lookup"><span data-stu-id="a0553-125">Name</span></span>       | <span data-ttu-id="a0553-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a0553-126">Type</span></span> | <span data-ttu-id="a0553-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a0553-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a0553-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0553-128">Authorization</span></span>  | <span data-ttu-id="a0553-129">string</span><span class="sxs-lookup"><span data-stu-id="a0553-129">string</span></span>  | <span data-ttu-id="a0553-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0553-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0553-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a0553-132">Request body</span></span>
<span data-ttu-id="a0553-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0553-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0553-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0553-134">Response</span></span>
<span data-ttu-id="a0553-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0553-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0553-136">Пример</span><span class="sxs-lookup"><span data-stu-id="a0553-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a0553-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0553-137">Request</span></span>
<span data-ttu-id="a0553-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0553-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a0553-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0553-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a0553-140">C#</span><span class="sxs-lookup"><span data-stu-id="a0553-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0553-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0553-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a0553-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0553-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a0553-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0553-143">Response</span></span>
<span data-ttu-id="a0553-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a0553-144">The following is an example of the response.</span></span>
><span data-ttu-id="a0553-145">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a0553-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a0553-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0553-146">All the properties will be returned from an actual call.</span></span>
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

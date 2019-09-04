---
title: Список членов группы
description: Получение списка непосредственных участников группы. У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников. Эта операция не является транзитивной.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 98b02ed4dfdc4d3cd6fbaf1a6447b39618aece54
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721592"
---
# <a name="list-group-members"></a><span data-ttu-id="585ae-105">Список членов группы</span><span class="sxs-lookup"><span data-stu-id="585ae-105">List group members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="585ae-106">Получение списка непосредственных участников группы.</span><span class="sxs-lookup"><span data-stu-id="585ae-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="585ae-107">У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="585ae-107">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="585ae-108">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="585ae-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="585ae-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="585ae-109">Permissions</span></span>

<span data-ttu-id="585ae-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="585ae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="585ae-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="585ae-112">Permission type</span></span>      | <span data-ttu-id="585ae-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="585ae-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="585ae-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="585ae-114">Delegated (work or school account)</span></span> | <span data-ttu-id="585ae-115">Directory. Read. ALL, Directory. AccessAsUser. ALL, User. ReadBasic. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="585ae-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="585ae-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="585ae-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="585ae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="585ae-117">Not supported.</span></span>    |
|<span data-ttu-id="585ae-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="585ae-118">Application</span></span> | <span data-ttu-id="585ae-119">Directory. Read. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="585ae-119">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="585ae-120">Note: чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="585ae-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>
 
## <a name="http-request"></a><span data-ttu-id="585ae-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="585ae-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="585ae-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="585ae-122">Optional query parameters</span></span>
<span data-ttu-id="585ae-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="585ae-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="585ae-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="585ae-124">Request headers</span></span>
| <span data-ttu-id="585ae-125">Имя</span><span class="sxs-lookup"><span data-stu-id="585ae-125">Name</span></span>       | <span data-ttu-id="585ae-126">Тип</span><span class="sxs-lookup"><span data-stu-id="585ae-126">Type</span></span> | <span data-ttu-id="585ae-127">Описание</span><span class="sxs-lookup"><span data-stu-id="585ae-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="585ae-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="585ae-128">Authorization</span></span>  | <span data-ttu-id="585ae-129">string</span><span class="sxs-lookup"><span data-stu-id="585ae-129">string</span></span>  | <span data-ttu-id="585ae-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="585ae-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="585ae-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="585ae-132">Request body</span></span>
<span data-ttu-id="585ae-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="585ae-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="585ae-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="585ae-134">Response</span></span>
<span data-ttu-id="585ae-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="585ae-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="585ae-136">Пример</span><span class="sxs-lookup"><span data-stu-id="585ae-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="585ae-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="585ae-137">Request</span></span>
<span data-ttu-id="585ae-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="585ae-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="585ae-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="585ae-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="585ae-140">C#</span><span class="sxs-lookup"><span data-stu-id="585ae-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="585ae-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="585ae-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="585ae-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="585ae-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="585ae-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="585ae-143">Response</span></span>
<span data-ttu-id="585ae-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="585ae-144">The following is an example of the response.</span></span>
><span data-ttu-id="585ae-145">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="585ae-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="585ae-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="585ae-146">All the properties will be returned from an actual call.</span></span>
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

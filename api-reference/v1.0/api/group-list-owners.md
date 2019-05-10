---
title: Список владельцев
description: 'Получение списка владельцев группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы. '
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ad2c5abbbfe7178386612ebb3980be36db690823
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614123"
---
# <a name="list-owners"></a><span data-ttu-id="4dba6-104">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="4dba6-104">List owners</span></span>
<span data-ttu-id="4dba6-p102">Получение списка владельцев группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="4dba6-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4dba6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4dba6-107">Permissions</span></span>
<span data-ttu-id="4dba6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dba6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dba6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dba6-110">Permission type</span></span>      | <span data-ttu-id="4dba6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dba6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dba6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dba6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4dba6-113">Group.Read.All и User.ReadBasic.All, Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dba6-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="4dba6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dba6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dba6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dba6-115">Not supported.</span></span>    |
|<span data-ttu-id="4dba6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4dba6-116">Application</span></span> | <span data-ttu-id="4dba6-117">Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dba6-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4dba6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dba6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4dba6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4dba6-119">Optional query parameters</span></span>
<span data-ttu-id="4dba6-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4dba6-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4dba6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4dba6-121">Request headers</span></span>
| <span data-ttu-id="4dba6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4dba6-122">Name</span></span>       | <span data-ttu-id="4dba6-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4dba6-123">Type</span></span> | <span data-ttu-id="4dba6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4dba6-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4dba6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dba6-125">Authorization</span></span>  | <span data-ttu-id="4dba6-126">string</span><span class="sxs-lookup"><span data-stu-id="4dba6-126">string</span></span>  | <span data-ttu-id="4dba6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4dba6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4dba6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4dba6-129">Request body</span></span>
<span data-ttu-id="4dba6-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4dba6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dba6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dba6-131">Response</span></span>
<span data-ttu-id="4dba6-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4dba6-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dba6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4dba6-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4dba6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dba6-134">Request</span></span>
<span data-ttu-id="4dba6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dba6-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="4dba6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dba6-136">Response</span></span>
<span data-ttu-id="4dba6-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4dba6-137">The following is an example of the response.</span></span>
><span data-ttu-id="4dba6-138">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4dba6-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4dba6-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4dba6-139">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4dba6-140">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="4dba6-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4dba6-141">C#</span><span class="sxs-lookup"><span data-stu-id="4dba6-141">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_owners-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4dba6-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="4dba6-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_owners-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-owners.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-owners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

---
title: Список владельцев
description: Получение списка владельцев группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2b8d2a8478d3b6b0c5ffbea13b4a59873cdc9f91
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701433"
---
# <a name="list-owners"></a><span data-ttu-id="8c6d2-103">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="8c6d2-103">List owners</span></span>

<span data-ttu-id="8c6d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c6d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c6d2-105">Получение списка владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="8c6d2-105">Retrieve a list of the group's owners.</span></span> <span data-ttu-id="8c6d2-106">Владельцы — это набор пользователей, которым разрешено изменять объект Group.</span><span class="sxs-lookup"><span data-stu-id="8c6d2-106">The owners are a set of users who are allowed to modify the group object.</span></span> <span data-ttu-id="8c6d2-107">В настоящее время владельцы не доступны в Microsoft Graph для групп, которые были созданы в Exchange или в группах, синхронизированных из локальной среды.</span><span class="sxs-lookup"><span data-stu-id="8c6d2-107">Owners are currently not available in Microsoft Graph for groups that were created in Exchange or groups that are synchronized from an on-premises environment.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8c6d2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c6d2-108">Permissions</span></span>
<span data-ttu-id="8c6d2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c6d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c6d2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c6d2-111">Permission type</span></span>      | <span data-ttu-id="8c6d2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c6d2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c6d2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c6d2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8c6d2-114">Group.Read.All и User.ReadBasic.All, Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All, Group.Read.All и User.Read.All и Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c6d2-114">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>  |
|<span data-ttu-id="8c6d2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c6d2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c6d2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c6d2-116">Not supported.</span></span>    |
|<span data-ttu-id="8c6d2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c6d2-117">Application</span></span> | <span data-ttu-id="8c6d2-118">Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All, Group.Read.All и User.Read.All и Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c6d2-118">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8c6d2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c6d2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c6d2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c6d2-120">Optional query parameters</span></span>
<span data-ttu-id="8c6d2-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8c6d2-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c6d2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c6d2-122">Request headers</span></span>
| <span data-ttu-id="8c6d2-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8c6d2-123">Name</span></span>       | <span data-ttu-id="8c6d2-124">Тип</span><span class="sxs-lookup"><span data-stu-id="8c6d2-124">Type</span></span> | <span data-ttu-id="8c6d2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8c6d2-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8c6d2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c6d2-126">Authorization</span></span>  | <span data-ttu-id="8c6d2-127">string</span><span class="sxs-lookup"><span data-stu-id="8c6d2-127">string</span></span>  | <span data-ttu-id="8c6d2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c6d2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c6d2-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c6d2-130">Request body</span></span>
<span data-ttu-id="8c6d2-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c6d2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c6d2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c6d2-132">Response</span></span>
<span data-ttu-id="8c6d2-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c6d2-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c6d2-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8c6d2-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8c6d2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c6d2-135">Request</span></span>
<span data-ttu-id="8c6d2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c6d2-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c6d2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c6d2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="8c6d2-138">C#</span><span class="sxs-lookup"><span data-stu-id="8c6d2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c6d2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c6d2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c6d2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c6d2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8c6d2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c6d2-141">Response</span></span>
<span data-ttu-id="8c6d2-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c6d2-142">The following is an example of the response.</span></span>
><span data-ttu-id="8c6d2-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c6d2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



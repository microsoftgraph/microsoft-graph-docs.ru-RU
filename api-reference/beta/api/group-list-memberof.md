---
title: Группа списка memberOf
description: Получение групп и административных единиц, непосредственным участником которых является группа.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f98e5d7f4a0bf1fcbc92a57467bdf009ab7b2698
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406609"
---
# <a name="list-group-memberof"></a><span data-ttu-id="229c2-103">Группа списка memberOf</span><span class="sxs-lookup"><span data-stu-id="229c2-103">List group memberOf</span></span>

<span data-ttu-id="229c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="229c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="229c2-105">Получение групп и административных единиц, непосредственным участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="229c2-105">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="229c2-p101">Эта операция не является транзитивным. В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="229c2-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="229c2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="229c2-108">Permissions</span></span>

<span data-ttu-id="229c2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="229c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="229c2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="229c2-111">Permission type</span></span>      | <span data-ttu-id="229c2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="229c2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="229c2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="229c2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="229c2-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="229c2-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="229c2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="229c2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="229c2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="229c2-116">Not supported.</span></span>    |
|<span data-ttu-id="229c2-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="229c2-117">Application</span></span> | <span data-ttu-id="229c2-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="229c2-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="229c2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="229c2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="229c2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="229c2-120">Optional query parameters</span></span>
<span data-ttu-id="229c2-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="229c2-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="229c2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="229c2-122">Request headers</span></span>
| <span data-ttu-id="229c2-123">Имя</span><span class="sxs-lookup"><span data-stu-id="229c2-123">Name</span></span>       | <span data-ttu-id="229c2-124">Тип</span><span class="sxs-lookup"><span data-stu-id="229c2-124">Type</span></span> | <span data-ttu-id="229c2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="229c2-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="229c2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="229c2-126">Authorization</span></span>  | <span data-ttu-id="229c2-127">string</span><span class="sxs-lookup"><span data-stu-id="229c2-127">string</span></span>  | <span data-ttu-id="229c2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="229c2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="229c2-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="229c2-130">Request body</span></span>
<span data-ttu-id="229c2-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="229c2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="229c2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="229c2-132">Response</span></span>
<span data-ttu-id="229c2-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="229c2-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="229c2-134">Пример</span><span class="sxs-lookup"><span data-stu-id="229c2-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="229c2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="229c2-135">Request</span></span>

<span data-ttu-id="229c2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="229c2-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="229c2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="229c2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="229c2-138">C#</span><span class="sxs-lookup"><span data-stu-id="229c2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="229c2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="229c2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="229c2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="229c2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="229c2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="229c2-141">Response</span></span>

<span data-ttu-id="229c2-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="229c2-142">The following is an example of the response.</span></span>
><span data-ttu-id="229c2-143">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="229c2-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="229c2-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="229c2-144">All the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

---
title: Получение команды
description: Получение свойств и связей указанной команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dc9a45e22022b6f95ab0e7dde4187bfe105af093
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845801"
---
# <a name="get-team"></a><span data-ttu-id="38990-103">Получение команды</span><span class="sxs-lookup"><span data-stu-id="38990-103">Get team</span></span>

<span data-ttu-id="38990-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38990-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="38990-105">Получение свойств и связей указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="38990-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="38990-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38990-106">Permissions</span></span>
<span data-ttu-id="38990-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="38990-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="38990-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38990-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38990-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38990-109">Permission type</span></span>      | <span data-ttu-id="38990-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38990-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38990-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38990-111">Delegated (work or school account)</span></span> | <span data-ttu-id="38990-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38990-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="38990-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38990-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38990-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38990-114">Not supported.</span></span>    |
|<span data-ttu-id="38990-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38990-115">Application</span></span> | <span data-ttu-id="38990-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38990-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="38990-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="38990-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="38990-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="38990-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="38990-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38990-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38990-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="38990-120">Optional query parameters</span></span>
<span data-ttu-id="38990-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="38990-121">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38990-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38990-122">Request headers</span></span>
| <span data-ttu-id="38990-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38990-123">Header</span></span>       | <span data-ttu-id="38990-124">Значение</span><span class="sxs-lookup"><span data-stu-id="38990-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="38990-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38990-125">Authorization</span></span>  | <span data-ttu-id="38990-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="38990-126">Bearer {token}.</span></span> <span data-ttu-id="38990-127">Required.</span><span class="sxs-lookup"><span data-stu-id="38990-127">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38990-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38990-128">Request body</span></span>
<span data-ttu-id="38990-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38990-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38990-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="38990-130">Response</span></span>

<span data-ttu-id="38990-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [team](../resources/team.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38990-131">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38990-132">Пример</span><span class="sxs-lookup"><span data-stu-id="38990-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="38990-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="38990-133">Request</span></span>
<span data-ttu-id="38990-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38990-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38990-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="38990-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}
```
# <a name="c"></a>[<span data-ttu-id="38990-136">C#</span><span class="sxs-lookup"><span data-stu-id="38990-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38990-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38990-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38990-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38990-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38990-139">Java</span><span class="sxs-lookup"><span data-stu-id="38990-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="38990-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="38990-140">Response</span></span>
<span data-ttu-id="38990-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="38990-141">The following is an example of the response.</span></span> 

><span data-ttu-id="38990-142">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="38990-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="38990-143">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="38990-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived": false,
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  },
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

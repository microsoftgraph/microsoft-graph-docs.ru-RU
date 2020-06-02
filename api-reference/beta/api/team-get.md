---
title: Получение команды
description: Получение свойств и связей указанной команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4df3c51a75bd20b024642f5eeba1bc28aa7d6cc7
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491667"
---
# <a name="get-team"></a><span data-ttu-id="bf3d9-103">Получение команды</span><span class="sxs-lookup"><span data-stu-id="bf3d9-103">Get team</span></span>

<span data-ttu-id="bf3d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf3d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf3d9-105">Получение свойств и связей указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="bf3d9-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf3d9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf3d9-106">Permissions</span></span>
<span data-ttu-id="bf3d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf3d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf3d9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf3d9-109">Permission type</span></span>      | <span data-ttu-id="bf3d9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf3d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf3d9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf3d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf3d9-112">Team. ReadBasic. ALL, Теамсеттингс. Read. ALL, Теамсеттингс. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bf3d9-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="bf3d9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf3d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf3d9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf3d9-114">Not supported.</span></span>    |
|<span data-ttu-id="bf3d9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf3d9-115">Application</span></span> | <span data-ttu-id="bf3d9-116">Теамсеттингс. Read. Group *, Team. ReadBasic. ALL, теамсеттингс. Read. ALL, теамсеттингс. ReadWrite. ALL, теамсеттингс. Edit. Group*, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bf3d9-116">TeamSettings.Read.Group *, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, TeamSettings.Edit.Group*, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
> <span data-ttu-id="bf3d9-117">**Note**: разрешения, помеченные как \* использовать [согласие с определенным ресурсом](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="bf3d9-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="bf3d9-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="bf3d9-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bf3d9-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="bf3d9-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bf3d9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf3d9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf3d9-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bf3d9-121">Optional query parameters</span></span>
<span data-ttu-id="bf3d9-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bf3d9-122">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf3d9-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf3d9-123">Request headers</span></span>
| <span data-ttu-id="bf3d9-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf3d9-124">Header</span></span>       | <span data-ttu-id="bf3d9-125">Значение</span><span class="sxs-lookup"><span data-stu-id="bf3d9-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bf3d9-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf3d9-126">Authorization</span></span>  | <span data-ttu-id="bf3d9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf3d9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bf3d9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf3d9-129">Request body</span></span>
<span data-ttu-id="bf3d9-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf3d9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf3d9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf3d9-131">Response</span></span>

<span data-ttu-id="bf3d9-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [team](../resources/team.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf3d9-132">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bf3d9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bf3d9-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bf3d9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf3d9-134">Request</span></span>
<span data-ttu-id="bf3d9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf3d9-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf3d9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf3d9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}
```
# <a name="c"></a>[<span data-ttu-id="bf3d9-137">C#</span><span class="sxs-lookup"><span data-stu-id="bf3d9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf3d9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf3d9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf3d9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf3d9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="bf3d9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf3d9-140">Response</span></span>
<span data-ttu-id="bf3d9-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bf3d9-141">The following is an example of the response.</span></span> 

><span data-ttu-id="bf3d9-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf3d9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "isArchived" : false,
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
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

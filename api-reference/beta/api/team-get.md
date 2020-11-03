---
title: Получение команды
description: Получение свойств и связей указанной команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c4c351b67f58343342a42ee0652a992947a5be97
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848846"
---
# <a name="get-team"></a><span data-ttu-id="4d3be-103">Получение команды</span><span class="sxs-lookup"><span data-stu-id="4d3be-103">Get team</span></span>

<span data-ttu-id="4d3be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d3be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d3be-105">Получение свойств и связей указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4d3be-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4d3be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d3be-106">Permissions</span></span>
<span data-ttu-id="4d3be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d3be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d3be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d3be-109">Permission type</span></span>      | <span data-ttu-id="4d3be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d3be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d3be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d3be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4d3be-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d3be-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="4d3be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d3be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d3be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d3be-114">Not supported.</span></span>    |
|<span data-ttu-id="4d3be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d3be-115">Application</span></span> | <span data-ttu-id="4d3be-116">TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group* , Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d3be-116">TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group* , Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
> <span data-ttu-id="4d3be-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="4d3be-117">**Note** : Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="4d3be-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="4d3be-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="4d3be-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="4d3be-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4d3be-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d3be-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d3be-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4d3be-121">Optional query parameters</span></span>
<span data-ttu-id="4d3be-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4d3be-122">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d3be-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d3be-123">Request headers</span></span>
| <span data-ttu-id="4d3be-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d3be-124">Header</span></span>       | <span data-ttu-id="4d3be-125">Значение</span><span class="sxs-lookup"><span data-stu-id="4d3be-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4d3be-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d3be-126">Authorization</span></span>  | <span data-ttu-id="4d3be-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d3be-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d3be-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d3be-129">Request body</span></span>
<span data-ttu-id="4d3be-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d3be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d3be-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d3be-131">Response</span></span>

<span data-ttu-id="4d3be-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [team](../resources/team.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d3be-132">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d3be-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4d3be-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4d3be-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d3be-134">Request</span></span>
<span data-ttu-id="4d3be-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d3be-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d3be-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d3be-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}
```
# <a name="c"></a>[<span data-ttu-id="4d3be-137">C#</span><span class="sxs-lookup"><span data-stu-id="4d3be-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d3be-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d3be-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d3be-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d3be-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="4d3be-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d3be-140">Response</span></span>
<span data-ttu-id="4d3be-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d3be-141">The following is an example of the response.</span></span> 

><span data-ttu-id="4d3be-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d3be-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "isMembershipLimitedToOwners": true,
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



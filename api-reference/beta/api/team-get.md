---
title: Получение команды
description: Получение свойств и связей указанной команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c8d1129c57444d95a1a3a46ee58590e102056a98
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290099"
---
# <a name="get-team"></a><span data-ttu-id="10300-103">Получение команды</span><span class="sxs-lookup"><span data-stu-id="10300-103">Get team</span></span>

<span data-ttu-id="10300-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10300-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10300-105">Получение свойств и связей указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="10300-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="10300-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10300-106">Permissions</span></span>
<span data-ttu-id="10300-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10300-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10300-109">Permission type</span></span>      | <span data-ttu-id="10300-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10300-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10300-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10300-111">Delegated (work or school account)</span></span> | <span data-ttu-id="10300-112">Team. ReadBasic. ALL, Теамсеттингс. Read. ALL, Теамсеттингс. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="10300-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="10300-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10300-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10300-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10300-114">Not supported.</span></span>    |
|<span data-ttu-id="10300-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10300-115">Application</span></span> | <span data-ttu-id="10300-116">Теамсеттингс. Read. Group ([RSC](https://aka.ms/teams-rsc)), Team. ReadBasic. ALL, Теамсеттингс. Read. ALL, Теамсеттингс. ReadWrite. ALL, Теамсеттингс. Edit. Group ([RSC](https://aka.ms/teams-rsc)), Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="10300-116">TeamSettings.Read.Group ([RSC](https://aka.ms/teams-rsc)), Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, TeamSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="10300-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="10300-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="10300-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="10300-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="10300-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10300-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10300-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10300-120">Optional query parameters</span></span>
<span data-ttu-id="10300-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="10300-121">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10300-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10300-122">Request headers</span></span>
| <span data-ttu-id="10300-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10300-123">Header</span></span>       | <span data-ttu-id="10300-124">Значение</span><span class="sxs-lookup"><span data-stu-id="10300-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="10300-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10300-125">Authorization</span></span>  | <span data-ttu-id="10300-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10300-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="10300-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10300-128">Request body</span></span>
<span data-ttu-id="10300-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10300-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10300-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="10300-130">Response</span></span>

<span data-ttu-id="10300-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [team](../resources/team.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10300-131">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10300-132">Пример</span><span class="sxs-lookup"><span data-stu-id="10300-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="10300-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="10300-133">Request</span></span>
<span data-ttu-id="10300-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10300-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="10300-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="10300-135">Response</span></span>
<span data-ttu-id="10300-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10300-136">The following is an example of the response.</span></span> 

><span data-ttu-id="10300-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10300-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
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

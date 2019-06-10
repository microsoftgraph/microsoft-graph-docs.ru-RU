---
title: Получение команды
description: Получение свойств и связей указанной команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 4a82949f717fd815aadb6423a7885b3ebe1da769
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812735"
---
# <a name="get-team"></a><span data-ttu-id="34239-103">Получение команды</span><span class="sxs-lookup"><span data-stu-id="34239-103">Get team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34239-104">Получение свойств и связей указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="34239-104">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="34239-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34239-105">Permissions</span></span>
<span data-ttu-id="34239-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34239-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34239-108">Permission type</span></span>      | <span data-ttu-id="34239-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34239-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34239-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34239-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34239-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34239-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="34239-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34239-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34239-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34239-113">Not supported.</span></span>    |
|<span data-ttu-id="34239-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34239-114">Application</span></span> | <span data-ttu-id="34239-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34239-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="34239-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="34239-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="34239-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="34239-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="34239-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34239-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34239-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="34239-119">Optional query parameters</span></span>
<span data-ttu-id="34239-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="34239-120">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34239-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34239-121">Request headers</span></span>
| <span data-ttu-id="34239-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34239-122">Header</span></span>       | <span data-ttu-id="34239-123">Значение</span><span class="sxs-lookup"><span data-stu-id="34239-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="34239-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34239-124">Authorization</span></span>  | <span data-ttu-id="34239-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34239-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34239-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34239-127">Request body</span></span>
<span data-ttu-id="34239-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34239-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34239-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="34239-129">Response</span></span>

<span data-ttu-id="34239-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [team](../resources/team.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34239-130">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34239-131">Пример</span><span class="sxs-lookup"><span data-stu-id="34239-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="34239-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="34239-132">Request</span></span>
<span data-ttu-id="34239-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34239-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="34239-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="34239-134">Response</span></span>
<span data-ttu-id="34239-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="34239-135">The following is an example of the response.</span></span> 

><span data-ttu-id="34239-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34239-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

---
title: Получение команды
description: Получение свойств и связей указанной команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3f66f20dd41da6212cda37c9a3f45c9f9dc90b26
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452577"
---
# <a name="get-team"></a><span data-ttu-id="25e52-103">Получение команды</span><span class="sxs-lookup"><span data-stu-id="25e52-103">Get team</span></span>

<span data-ttu-id="25e52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25e52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25e52-105">Получение свойств и связей указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="25e52-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="25e52-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25e52-106">Permissions</span></span>
<span data-ttu-id="25e52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25e52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25e52-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25e52-109">Permission type</span></span>      | <span data-ttu-id="25e52-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25e52-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25e52-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25e52-111">Delegated (work or school account)</span></span> | <span data-ttu-id="25e52-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25e52-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="25e52-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25e52-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25e52-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25e52-114">Not supported.</span></span>    |
|<span data-ttu-id="25e52-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25e52-115">Application</span></span> | <span data-ttu-id="25e52-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25e52-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="25e52-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="25e52-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="25e52-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="25e52-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="25e52-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25e52-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25e52-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="25e52-120">Optional query parameters</span></span>
<span data-ttu-id="25e52-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="25e52-121">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25e52-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25e52-122">Request headers</span></span>
| <span data-ttu-id="25e52-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25e52-123">Header</span></span>       | <span data-ttu-id="25e52-124">Значение</span><span class="sxs-lookup"><span data-stu-id="25e52-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="25e52-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25e52-125">Authorization</span></span>  | <span data-ttu-id="25e52-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25e52-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25e52-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25e52-128">Request body</span></span>
<span data-ttu-id="25e52-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25e52-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25e52-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="25e52-130">Response</span></span>

<span data-ttu-id="25e52-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [team](../resources/team.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25e52-131">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25e52-132">Пример</span><span class="sxs-lookup"><span data-stu-id="25e52-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="25e52-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="25e52-133">Request</span></span>
<span data-ttu-id="25e52-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25e52-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="25e52-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="25e52-135">Response</span></span>
<span data-ttu-id="25e52-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25e52-136">The following is an example of the response.</span></span> 

><span data-ttu-id="25e52-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25e52-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

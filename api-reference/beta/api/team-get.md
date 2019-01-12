---
title: Получение группы
description: Извлечение свойств и связи из указанной группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 4ec9c53dbb474afabc3c2a67e480bf9972dfefc5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947710"
---
# <a name="get-team"></a><span data-ttu-id="e9500-103">Получение группы</span><span class="sxs-lookup"><span data-stu-id="e9500-103">Get team</span></span>

> <span data-ttu-id="e9500-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9500-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9500-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9500-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9500-106">Извлечение свойств и связи из указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="e9500-106">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9500-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9500-107">Permissions</span></span>
<span data-ttu-id="e9500-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9500-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9500-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9500-110">Permission type</span></span>      | <span data-ttu-id="e9500-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9500-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9500-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9500-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e9500-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9500-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e9500-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9500-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9500-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9500-115">Not supported.</span></span>    |
|<span data-ttu-id="e9500-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9500-116">Application</span></span> | <span data-ttu-id="e9500-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9500-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="e9500-118">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="e9500-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e9500-119">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="e9500-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e9500-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9500-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9500-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e9500-121">Optional query parameters</span></span>
<span data-ttu-id="e9500-122">Этот метод поддерживает $select и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e9500-122">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9500-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9500-123">Request headers</span></span>
| <span data-ttu-id="e9500-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9500-124">Header</span></span>       | <span data-ttu-id="e9500-125">Значение</span><span class="sxs-lookup"><span data-stu-id="e9500-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e9500-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9500-126">Authorization</span></span>  | <span data-ttu-id="e9500-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9500-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9500-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9500-129">Request body</span></span>
<span data-ttu-id="e9500-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9500-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9500-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9500-131">Response</span></span>

<span data-ttu-id="e9500-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и объекта [группы](../resources/team.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e9500-132">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9500-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e9500-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e9500-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9500-134">Request</span></span>
<span data-ttu-id="e9500-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9500-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="e9500-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9500-136">Response</span></span>
<span data-ttu-id="e9500-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9500-137">The following is an example of the response.</span></span> 

><span data-ttu-id="e9500-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9500-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

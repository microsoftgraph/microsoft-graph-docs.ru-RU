---
title: Получение группы
description: Извлечение свойств и связи из указанной группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 0221983538f14ef3f0c0439f8241974091e8dc0b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943139"
---
# <a name="get-team"></a><span data-ttu-id="4d81b-103">Получение группы</span><span class="sxs-lookup"><span data-stu-id="4d81b-103">Get team</span></span>



<span data-ttu-id="4d81b-104">Извлечение свойств и связи из указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4d81b-104">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4d81b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d81b-105">Permissions</span></span>
<span data-ttu-id="4d81b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d81b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d81b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d81b-108">Permission type</span></span>      | <span data-ttu-id="4d81b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d81b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d81b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d81b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d81b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d81b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d81b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d81b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d81b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d81b-113">Not supported.</span></span>    |
|<span data-ttu-id="4d81b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d81b-114">Application</span></span> | <span data-ttu-id="4d81b-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d81b-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="4d81b-116">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="4d81b-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4d81b-117">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="4d81b-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4d81b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d81b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d81b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4d81b-119">Optional query parameters</span></span>
<span data-ttu-id="4d81b-120">Этот метод поддерживает $select и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4d81b-120">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d81b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d81b-121">Request headers</span></span>
| <span data-ttu-id="4d81b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d81b-122">Header</span></span>       | <span data-ttu-id="4d81b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4d81b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4d81b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d81b-124">Authorization</span></span>  | <span data-ttu-id="4d81b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d81b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d81b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4d81b-127">Request body</span></span>
<span data-ttu-id="4d81b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d81b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d81b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d81b-129">Response</span></span>

<span data-ttu-id="4d81b-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объекта [группы](../resources/team.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4d81b-130">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d81b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4d81b-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4d81b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d81b-132">Request</span></span>
<span data-ttu-id="4d81b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d81b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="4d81b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d81b-134">Response</span></span>
<span data-ttu-id="4d81b-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d81b-135">The following is an example of the response.</span></span> 

><span data-ttu-id="4d81b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d81b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

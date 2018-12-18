---
title: Получение группы
description: Извлечение свойств и связи из указанной группы.
author: nkramer
ms.openlocfilehash: dfa59948a9bffce77c98a3462f919e75fe18042e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329234"
---
# <a name="get-team"></a><span data-ttu-id="aff64-103">Получение группы</span><span class="sxs-lookup"><span data-stu-id="aff64-103">Get team</span></span>

> <span data-ttu-id="aff64-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aff64-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aff64-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aff64-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aff64-106">Извлечение свойств и связи из указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="aff64-106">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aff64-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aff64-107">Permissions</span></span>
<span data-ttu-id="aff64-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aff64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aff64-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aff64-110">Permission type</span></span>      | <span data-ttu-id="aff64-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aff64-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aff64-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aff64-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aff64-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aff64-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="aff64-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aff64-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aff64-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aff64-115">Not supported.</span></span>    |
|<span data-ttu-id="aff64-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aff64-116">Application</span></span> | <span data-ttu-id="aff64-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aff64-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="aff64-118">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="aff64-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="aff64-119">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="aff64-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="aff64-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aff64-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aff64-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aff64-121">Optional query parameters</span></span>
<span data-ttu-id="aff64-122">Этот метод поддерживает $select и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aff64-122">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aff64-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aff64-123">Request headers</span></span>
| <span data-ttu-id="aff64-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aff64-124">Header</span></span>       | <span data-ttu-id="aff64-125">Значение</span><span class="sxs-lookup"><span data-stu-id="aff64-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aff64-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aff64-126">Authorization</span></span>  | <span data-ttu-id="aff64-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aff64-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aff64-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aff64-129">Request body</span></span>
<span data-ttu-id="aff64-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aff64-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aff64-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="aff64-131">Response</span></span>

<span data-ttu-id="aff64-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и объекта [группы](../resources/team.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="aff64-132">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aff64-133">Пример</span><span class="sxs-lookup"><span data-stu-id="aff64-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="aff64-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="aff64-134">Request</span></span>
<span data-ttu-id="aff64-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aff64-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="aff64-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="aff64-136">Response</span></span>
<span data-ttu-id="aff64-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aff64-137">The following is an example of the response.</span></span> 

><span data-ttu-id="aff64-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aff64-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

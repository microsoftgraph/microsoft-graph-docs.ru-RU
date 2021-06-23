---
title: Список teamworkTags
description: Получите список объектов teamworkTag и их свойств.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 0a5e008e32565675982ec7d120be3d6d3bad98ed
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060722"
---
# <a name="list-teamworktags"></a><span data-ttu-id="449d6-103">Список teamworkTags</span><span class="sxs-lookup"><span data-stu-id="449d6-103">List teamworkTags</span></span>
<span data-ttu-id="449d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="449d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="449d6-105">Получите список объектов [тегов](../resources/teamworktag.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="449d6-105">Get a list of the [tags](../resources/teamworktag.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="449d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="449d6-106">Permissions</span></span>
<span data-ttu-id="449d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="449d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="449d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="449d6-109">Permission type</span></span>|<span data-ttu-id="449d6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="449d6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="449d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="449d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="449d6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="449d6-112">Not supported.</span></span>|
|<span data-ttu-id="449d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="449d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="449d6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="449d6-114">Not supported.</span></span>|
|<span data-ttu-id="449d6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="449d6-115">Application</span></span>|<span data-ttu-id="449d6-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="449d6-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="relationships"></a><span data-ttu-id="449d6-117">Связи</span><span class="sxs-lookup"><span data-stu-id="449d6-117">Relationships</span></span>
|<span data-ttu-id="449d6-118">Связь</span><span class="sxs-lookup"><span data-stu-id="449d6-118">Relationship</span></span>|<span data-ttu-id="449d6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="449d6-119">Type</span></span>|<span data-ttu-id="449d6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="449d6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="449d6-121">members</span><span class="sxs-lookup"><span data-stu-id="449d6-121">members</span></span>|<span data-ttu-id="449d6-122">[коллекция teamworkTag](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="449d6-122">[teamworkTag](../resources/teamworktag.md) collection</span></span>|<span data-ttu-id="449d6-123">Теги, присвоенные команде.</span><span class="sxs-lookup"><span data-stu-id="449d6-123">Tags assigned to a team.</span></span>|

## <a name="http-request"></a><span data-ttu-id="449d6-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="449d6-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags
```

## <a name="optional-query-parameters"></a><span data-ttu-id="449d6-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="449d6-125">Optional query parameters</span></span>
<span data-ttu-id="449d6-126">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="449d6-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="449d6-127">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="449d6-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="449d6-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="449d6-128">Request headers</span></span>
|<span data-ttu-id="449d6-129">Имя</span><span class="sxs-lookup"><span data-stu-id="449d6-129">Name</span></span>|<span data-ttu-id="449d6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="449d6-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="449d6-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="449d6-131">Authorization</span></span>|<span data-ttu-id="449d6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="449d6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="449d6-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="449d6-134">Request body</span></span>
<span data-ttu-id="449d6-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="449d6-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="449d6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="449d6-136">Response</span></span>

<span data-ttu-id="449d6-137">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [teamworkTag](../resources/teamworktag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="449d6-137">If successful, this method returns a `200 OK` response code and a collection of [teamworkTag](../resources/teamworktag.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="449d6-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="449d6-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="449d6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="449d6-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_teamworktag"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags
```


### <a name="response"></a><span data-ttu-id="449d6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="449d6-140">Response</span></span>
><span data-ttu-id="449d6-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="449d6-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamworkTag)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "@odata.type": "#microsoft.graph.teamworkTag",
        "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
        "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
        "displayName": "Finance",
        "description": "Finance Team for Mach 8 Project",
        "memberCount": 2,
        "tagType": "standard"
    },
    {
        "@odata.type": "#microsoft.graph.teamworkTag",
        "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjIzk3ZjYyMzQ0LTU3ZGMtNDA5Yy04OGFkLWM0YWYxNDE1OGZmNQ==",
        "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
        "displayName": "Legal",
        "description": "Legal experts, ask us your legal questions",
        "memberCount": 4,
        "tagType": "standard"
    }
  ]
}
```


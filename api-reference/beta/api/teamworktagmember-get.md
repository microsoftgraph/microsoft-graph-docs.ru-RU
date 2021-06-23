---
title: Получить командную работуTagMember
description: Ознакомьтесь с свойствами и отношениями объекта teamworkTagMember.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8978cd5fe2ce6fc2ce806dc4093d50d86dc7c335
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060707"
---
# <a name="get-teamworktagmember"></a><span data-ttu-id="b8b6c-103">Получить командную работуTagMember</span><span class="sxs-lookup"><span data-stu-id="b8b6c-103">Get teamworkTagMember</span></span>
<span data-ttu-id="b8b6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8b6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8b6c-105">Получите свойства и отношения участника [стандартного](../resources/teamworktagmember.md) тега в команде.</span><span class="sxs-lookup"><span data-stu-id="b8b6c-105">Get the properties and relationships of a [member](../resources/teamworktagmember.md) of a standard tag in a team.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b8b6c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8b6c-106">Permissions</span></span>
<span data-ttu-id="b8b6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8b6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8b6c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8b6c-109">Permission type</span></span>|<span data-ttu-id="b8b6c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8b6c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8b6c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8b6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8b6c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8b6c-112">Not supported.</span></span>|
|<span data-ttu-id="b8b6c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8b6c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8b6c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8b6c-114">Not supported.</span></span>|
|<span data-ttu-id="b8b6c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b8b6c-115">Application</span></span>|<span data-ttu-id="b8b6c-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8b6c-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8b6c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8b6c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags/{teamworkTag-Id}/members/{teamworkTagMember-Id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8b6c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b8b6c-118">Optional query parameters</span></span>
<span data-ttu-id="b8b6c-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b8b6c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b8b6c-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b8b6c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8b6c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8b6c-121">Request headers</span></span>
|<span data-ttu-id="b8b6c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b8b6c-122">Name</span></span>|<span data-ttu-id="b8b6c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b8b6c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b8b6c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8b6c-124">Authorization</span></span>|<span data-ttu-id="b8b6c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8b6c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8b6c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8b6c-127">Request body</span></span>
<span data-ttu-id="b8b6c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8b6c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8b6c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8b6c-129">Response</span></span>

<span data-ttu-id="b8b6c-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект teamworkTagMember](../resources/teamworktagmember.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b8b6c-130">If successful, this method returns a `200 OK` response code and a [teamworkTagMember](../resources/teamworktagmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8b6c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b8b6c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b8b6c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8b6c-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teamworktagmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==
```


### <a name="response"></a><span data-ttu-id="b8b6c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8b6c-133">Response</span></span>
><span data-ttu-id="b8b6c-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b8b6c-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTagMember"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkTagMember",
    "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==",
    "displayName": "Alex Wilbur",
    "tenantId": "18be64a9-c73a-4862-bccc-76c31ef09b9d",
    "userId": "92f6952f-61ca-4a94-8910-508a240bc167"
  }
}
```

---
title: Командная работа
description: Ознакомьтесь с свойствами и отношениями объекта teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: aa99a204fac9dbc2417d0e30d548638e0b63ebd6
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060725"
---
# <a name="get-teamworktag"></a><span data-ttu-id="09594-103">Командная работа</span><span class="sxs-lookup"><span data-stu-id="09594-103">Get teamworkTag</span></span>
<span data-ttu-id="09594-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09594-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09594-105">Ознакомьтесь с свойствами и отношениями объекта [тегов.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="09594-105">Read the properties and relationships of a [tag](../resources/teamworktag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="09594-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09594-106">Permissions</span></span>
<span data-ttu-id="09594-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09594-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09594-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09594-109">Permission type</span></span>|<span data-ttu-id="09594-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09594-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09594-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09594-111">Delegated (work or school account)</span></span>|<span data-ttu-id="09594-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09594-112">Not supported.</span></span>|
|<span data-ttu-id="09594-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09594-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09594-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09594-114">Not supported.</span></span>|
|<span data-ttu-id="09594-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="09594-115">Application</span></span>|<span data-ttu-id="09594-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09594-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09594-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09594-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09594-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="09594-118">Optional query parameters</span></span>
<span data-ttu-id="09594-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="09594-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="09594-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="09594-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="09594-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09594-121">Request headers</span></span>
|<span data-ttu-id="09594-122">Имя</span><span class="sxs-lookup"><span data-stu-id="09594-122">Name</span></span>|<span data-ttu-id="09594-123">Описание</span><span class="sxs-lookup"><span data-stu-id="09594-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="09594-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09594-124">Authorization</span></span>|<span data-ttu-id="09594-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09594-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="09594-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09594-127">Request body</span></span>
<span data-ttu-id="09594-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09594-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09594-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="09594-129">Response</span></span>

<span data-ttu-id="09594-130">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [teamworkTag](../resources/teamworktag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="09594-130">If successful, this method returns a `200 OK` response code and a [teamworkTag](../resources/teamworktag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="09594-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="09594-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="09594-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="09594-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teamworktag"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
```


### <a name="response"></a><span data-ttu-id="09594-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="09594-133">Response</span></span>
><span data-ttu-id="09594-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="09594-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkTag",
    "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
    "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
    "displayName": "IT Admins",
    "description": "Team admins and IT support",
    "memberCount": "2",
    "tagType": "standard"
  }
}
```


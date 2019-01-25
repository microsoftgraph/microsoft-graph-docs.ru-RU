---
title: Обновление звука группы маршрутизации
description: Изменение источники и приемники audioRoutingGroup.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a6c8142ec36becd2a06a16d81bff7d1ceff75b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524676"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="8a7de-103">Обновление звука группы маршрутизации</span><span class="sxs-lookup"><span data-stu-id="8a7de-103">Update audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a7de-104">Изменение источники и приемники [audioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="8a7de-104">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8a7de-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a7de-105">Permissions</span></span>
<span data-ttu-id="8a7de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a7de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a7de-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a7de-108">Permission type</span></span> | <span data-ttu-id="8a7de-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a7de-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="8a7de-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a7de-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a7de-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8a7de-111">Not Supported</span></span>                       |
| <span data-ttu-id="8a7de-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a7de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a7de-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8a7de-113">Not Supported</span></span>                       |
| <span data-ttu-id="8a7de-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a7de-114">Application</span></span>     | <span data-ttu-id="8a7de-115">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="8a7de-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a7de-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a7de-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8a7de-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a7de-117">Request headers</span></span>
| <span data-ttu-id="8a7de-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8a7de-118">Name</span></span>          | <span data-ttu-id="8a7de-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8a7de-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8a7de-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a7de-120">Authorization</span></span> | <span data-ttu-id="8a7de-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a7de-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a7de-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a7de-123">Request body</span></span>
<span data-ttu-id="8a7de-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8a7de-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8a7de-125">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8a7de-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8a7de-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8a7de-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8a7de-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a7de-127">Property</span></span>       | <span data-ttu-id="8a7de-128">Тип</span><span class="sxs-lookup"><span data-stu-id="8a7de-128">Type</span></span>    |<span data-ttu-id="8a7de-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8a7de-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8a7de-130">Приемники</span><span class="sxs-lookup"><span data-stu-id="8a7de-130">receivers</span></span> | <span data-ttu-id="8a7de-131">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8a7de-131">String collection</span></span> | <span data-ttu-id="8a7de-132">Участники целевой в audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="8a7de-132">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="8a7de-133">routingMode</span><span class="sxs-lookup"><span data-stu-id="8a7de-133">routingMode</span></span> | <span data-ttu-id="8a7de-134">String</span><span class="sxs-lookup"><span data-stu-id="8a7de-134">String</span></span> | <span data-ttu-id="8a7de-135">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="8a7de-135">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="8a7de-136">sources</span><span class="sxs-lookup"><span data-stu-id="8a7de-136">sources</span></span> | <span data-ttu-id="8a7de-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8a7de-137">String collection</span></span> | <span data-ttu-id="8a7de-138">Участник источника в audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="8a7de-138">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="8a7de-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a7de-139">Response</span></span>
<span data-ttu-id="8a7de-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [audioRoutingGroup](../resources/audioroutinggroup.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8a7de-140">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a7de-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8a7de-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8a7de-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a7de-142">Request</span></span>
<span data-ttu-id="8a7de-143">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a7de-143">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update-audioRoutingGroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="8a7de-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a7de-144">Response</span></span>

> <span data-ttu-id="8a7de-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a7de-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/audioroutinggroup-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

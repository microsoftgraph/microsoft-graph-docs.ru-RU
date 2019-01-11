---
title: Обновление звука группы маршрутизации
description: Изменение источники и приемники audioRoutingGroup.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: b12d93d3cd8255cb735beaba7c78684a2b3b3a9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833840"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="68fd9-103">Обновление звука группы маршрутизации</span><span class="sxs-lookup"><span data-stu-id="68fd9-103">Update audio routing group</span></span>

> <span data-ttu-id="68fd9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="68fd9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68fd9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68fd9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="68fd9-106">Изменение источники и приемники [audioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="68fd9-106">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="68fd9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68fd9-107">Permissions</span></span>
<span data-ttu-id="68fd9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68fd9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68fd9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68fd9-110">Permission type</span></span> | <span data-ttu-id="68fd9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68fd9-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="68fd9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68fd9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="68fd9-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="68fd9-113">Not Supported</span></span>                       |
| <span data-ttu-id="68fd9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68fd9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68fd9-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="68fd9-115">Not Supported</span></span>                       |
| <span data-ttu-id="68fd9-116">Application</span><span class="sxs-lookup"><span data-stu-id="68fd9-116">Application</span></span>     | <span data-ttu-id="68fd9-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="68fd9-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68fd9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68fd9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="68fd9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68fd9-119">Request headers</span></span>
| <span data-ttu-id="68fd9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="68fd9-120">Name</span></span>          | <span data-ttu-id="68fd9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="68fd9-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="68fd9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68fd9-122">Authorization</span></span> | <span data-ttu-id="68fd9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68fd9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68fd9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68fd9-125">Request body</span></span>
<span data-ttu-id="68fd9-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="68fd9-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="68fd9-127">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="68fd9-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="68fd9-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="68fd9-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="68fd9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="68fd9-129">Property</span></span>       | <span data-ttu-id="68fd9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="68fd9-130">Type</span></span>    |<span data-ttu-id="68fd9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="68fd9-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="68fd9-132">Приемники</span><span class="sxs-lookup"><span data-stu-id="68fd9-132">receivers</span></span> | <span data-ttu-id="68fd9-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="68fd9-133">String collection</span></span> | <span data-ttu-id="68fd9-134">Участники целевой в audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="68fd9-134">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="68fd9-135">routingMode</span><span class="sxs-lookup"><span data-stu-id="68fd9-135">routingMode</span></span> | <span data-ttu-id="68fd9-136">String</span><span class="sxs-lookup"><span data-stu-id="68fd9-136">String</span></span> | <span data-ttu-id="68fd9-137">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="68fd9-137">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="68fd9-138">sources</span><span class="sxs-lookup"><span data-stu-id="68fd9-138">sources</span></span> | <span data-ttu-id="68fd9-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="68fd9-139">String collection</span></span> | <span data-ttu-id="68fd9-140">Участник источника в audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="68fd9-140">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="68fd9-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="68fd9-141">Response</span></span>
<span data-ttu-id="68fd9-142">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [audioRoutingGroup](../resources/audioroutinggroup.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="68fd9-142">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68fd9-143">Пример</span><span class="sxs-lookup"><span data-stu-id="68fd9-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="68fd9-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="68fd9-144">Request</span></span>
<span data-ttu-id="68fd9-145">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68fd9-145">The following example shows the request.</span></span>

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
##### <a name="response"></a><span data-ttu-id="68fd9-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="68fd9-146">Response</span></span>

> <span data-ttu-id="68fd9-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68fd9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

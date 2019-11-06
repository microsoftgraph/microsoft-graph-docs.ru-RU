---
title: Обновление группы маршрутизации звука
description: Изменение источников и приемников Аудиораутингграуп.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 993695ead1dc881a721ffc360cfb1e9abd75556d
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006377"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="3a3c8-103">Обновление группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="3a3c8-103">Update audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a3c8-104">Изменение источников и приемников [аудиораутингграуп](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="3a3c8-104">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3a3c8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a3c8-105">Permissions</span></span>
<span data-ttu-id="3a3c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a3c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a3c8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a3c8-108">Permission type</span></span> | <span data-ttu-id="3a3c8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a3c8-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="3a3c8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a3c8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a3c8-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3a3c8-111">Not Supported</span></span>                       |
| <span data-ttu-id="3a3c8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a3c8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a3c8-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3a3c8-113">Not Supported</span></span>                       |
| <span data-ttu-id="3a3c8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a3c8-114">Application</span></span>     | <span data-ttu-id="3a3c8-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="3a3c8-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a3c8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a3c8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="3a3c8-117">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="3a3c8-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="3a3c8-118">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="3a3c8-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a3c8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a3c8-119">Request headers</span></span>
| <span data-ttu-id="3a3c8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3a3c8-120">Name</span></span>          | <span data-ttu-id="3a3c8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3a3c8-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3a3c8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a3c8-122">Authorization</span></span> | <span data-ttu-id="3a3c8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a3c8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a3c8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a3c8-125">Request body</span></span>
<span data-ttu-id="3a3c8-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3a3c8-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3a3c8-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="3a3c8-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3a3c8-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3a3c8-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3a3c8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a3c8-129">Property</span></span>       | <span data-ttu-id="3a3c8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3a3c8-130">Type</span></span>    |<span data-ttu-id="3a3c8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3a3c8-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3a3c8-132">приемники</span><span class="sxs-lookup"><span data-stu-id="3a3c8-132">receivers</span></span> | <span data-ttu-id="3a3c8-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3a3c8-133">String collection</span></span> | <span data-ttu-id="3a3c8-134">Целевые участники в Аудиораутингграуп.</span><span class="sxs-lookup"><span data-stu-id="3a3c8-134">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="3a3c8-135">раутингмоде</span><span class="sxs-lookup"><span data-stu-id="3a3c8-135">routingMode</span></span> | <span data-ttu-id="3a3c8-136">String</span><span class="sxs-lookup"><span data-stu-id="3a3c8-136">String</span></span> | <span data-ttu-id="3a3c8-137">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="3a3c8-137">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="3a3c8-138">sources</span><span class="sxs-lookup"><span data-stu-id="3a3c8-138">sources</span></span> | <span data-ttu-id="3a3c8-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3a3c8-139">String collection</span></span> | <span data-ttu-id="3a3c8-140">Участник источника в Аудиораутингграуп.</span><span class="sxs-lookup"><span data-stu-id="3a3c8-140">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="3a3c8-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a3c8-141">Response</span></span>
<span data-ttu-id="3a3c8-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [аудиораутингграуп](../resources/audioroutinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a3c8-142">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a3c8-143">Пример</span><span class="sxs-lookup"><span data-stu-id="3a3c8-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3a3c8-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a3c8-144">Request</span></span>
<span data-ttu-id="3a3c8-145">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a3c8-145">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3a3c8-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a3c8-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update-audioRoutingGroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
Content-Type: application/json

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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3a3c8-147">C#</span><span class="sxs-lookup"><span data-stu-id="3a3c8-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a3c8-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a3c8-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3a3c8-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a3c8-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3a3c8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a3c8-150">Response</span></span>

> <span data-ttu-id="3a3c8-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a3c8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

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
  ]
}
-->

---
title: Обновление группы маршрутизации звука
description: Изменение источников и приемников audioRoutingGroup.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6e8bfe43529632988249206a0d84cc6e50e8324e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048010"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="ea1cb-103">Обновление группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="ea1cb-103">Update audio routing group</span></span>

<span data-ttu-id="ea1cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea1cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea1cb-105">Изменение источников и приемников [audioRoutingGroup.](../resources/audioroutinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="ea1cb-105">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea1cb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea1cb-106">Permissions</span></span>
<span data-ttu-id="ea1cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea1cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea1cb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea1cb-109">Permission type</span></span> | <span data-ttu-id="ea1cb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea1cb-110">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="ea1cb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea1cb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea1cb-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ea1cb-112">Not Supported</span></span>                       |
| <span data-ttu-id="ea1cb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea1cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea1cb-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ea1cb-114">Not Supported</span></span>                       |
| <span data-ttu-id="ea1cb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ea1cb-115">Application</span></span>     | <span data-ttu-id="ea1cb-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="ea1cb-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea1cb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea1cb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="ea1cb-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="ea1cb-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="ea1cb-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="ea1cb-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea1cb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea1cb-120">Request headers</span></span>
| <span data-ttu-id="ea1cb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ea1cb-121">Name</span></span>          | <span data-ttu-id="ea1cb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ea1cb-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ea1cb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea1cb-123">Authorization</span></span> | <span data-ttu-id="ea1cb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea1cb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea1cb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea1cb-126">Request body</span></span>
<span data-ttu-id="ea1cb-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="ea1cb-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ea1cb-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="ea1cb-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ea1cb-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ea1cb-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ea1cb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea1cb-130">Property</span></span>       | <span data-ttu-id="ea1cb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ea1cb-131">Type</span></span>    |<span data-ttu-id="ea1cb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ea1cb-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ea1cb-133">приемники</span><span class="sxs-lookup"><span data-stu-id="ea1cb-133">receivers</span></span> | <span data-ttu-id="ea1cb-134">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="ea1cb-134">String collection</span></span> | <span data-ttu-id="ea1cb-135">Целевые участники audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="ea1cb-135">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="ea1cb-136">routingMode</span><span class="sxs-lookup"><span data-stu-id="ea1cb-136">routingMode</span></span> | <span data-ttu-id="ea1cb-137">String</span><span class="sxs-lookup"><span data-stu-id="ea1cb-137">String</span></span> | <span data-ttu-id="ea1cb-138">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="ea1cb-138">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="ea1cb-139">sources</span><span class="sxs-lookup"><span data-stu-id="ea1cb-139">sources</span></span> | <span data-ttu-id="ea1cb-140">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="ea1cb-140">String collection</span></span> | <span data-ttu-id="ea1cb-141">Исходный участник в audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="ea1cb-141">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="ea1cb-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea1cb-142">Response</span></span>
<span data-ttu-id="ea1cb-143">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект audioRoutingGroup](../resources/audioroutinggroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ea1cb-143">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea1cb-144">Пример</span><span class="sxs-lookup"><span data-stu-id="ea1cb-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ea1cb-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea1cb-145">Request</span></span>
<span data-ttu-id="ea1cb-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea1cb-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ea1cb-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea1cb-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ea1cb-148">C#</span><span class="sxs-lookup"><span data-stu-id="ea1cb-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea1cb-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea1cb-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea1cb-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea1cb-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea1cb-151">Java</span><span class="sxs-lookup"><span data-stu-id="ea1cb-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-audioroutinggroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ea1cb-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea1cb-152">Response</span></span>

> <span data-ttu-id="ea1cb-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ea1cb-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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



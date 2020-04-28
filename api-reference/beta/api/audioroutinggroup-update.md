---
title: Обновление группы маршрутизации звука
description: Изменение источников и приемников Аудиораутингграуп.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 28cbf6662b09be81c6ffbafecbe1f888e596e3a8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441314"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="cc575-103">Обновление группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="cc575-103">Update audio routing group</span></span>

<span data-ttu-id="cc575-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc575-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc575-105">Изменение источников и приемников [аудиораутингграуп](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="cc575-105">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc575-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc575-106">Permissions</span></span>
<span data-ttu-id="cc575-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc575-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc575-109">Permission type</span></span> | <span data-ttu-id="cc575-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc575-110">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="cc575-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc575-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc575-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cc575-112">Not Supported</span></span>                       |
| <span data-ttu-id="cc575-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc575-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc575-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cc575-114">Not Supported</span></span>                       |
| <span data-ttu-id="cc575-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc575-115">Application</span></span>     | <span data-ttu-id="cc575-116">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="cc575-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc575-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc575-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="cc575-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="cc575-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="cc575-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="cc575-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc575-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc575-120">Request headers</span></span>
| <span data-ttu-id="cc575-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cc575-121">Name</span></span>          | <span data-ttu-id="cc575-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cc575-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cc575-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc575-123">Authorization</span></span> | <span data-ttu-id="cc575-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc575-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc575-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc575-126">Request body</span></span>
<span data-ttu-id="cc575-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="cc575-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="cc575-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="cc575-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cc575-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="cc575-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cc575-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc575-130">Property</span></span>       | <span data-ttu-id="cc575-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cc575-131">Type</span></span>    |<span data-ttu-id="cc575-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cc575-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cc575-133">приемники</span><span class="sxs-lookup"><span data-stu-id="cc575-133">receivers</span></span> | <span data-ttu-id="cc575-134">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="cc575-134">String collection</span></span> | <span data-ttu-id="cc575-135">Целевые участники в Аудиораутингграуп.</span><span class="sxs-lookup"><span data-stu-id="cc575-135">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="cc575-136">раутингмоде</span><span class="sxs-lookup"><span data-stu-id="cc575-136">routingMode</span></span> | <span data-ttu-id="cc575-137">String</span><span class="sxs-lookup"><span data-stu-id="cc575-137">String</span></span> | <span data-ttu-id="cc575-138">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="cc575-138">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="cc575-139">sources</span><span class="sxs-lookup"><span data-stu-id="cc575-139">sources</span></span> | <span data-ttu-id="cc575-140">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="cc575-140">String collection</span></span> | <span data-ttu-id="cc575-141">Участник источника в Аудиораутингграуп.</span><span class="sxs-lookup"><span data-stu-id="cc575-141">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="cc575-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc575-142">Response</span></span>
<span data-ttu-id="cc575-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [аудиораутингграуп](../resources/audioroutinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc575-143">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc575-144">Пример</span><span class="sxs-lookup"><span data-stu-id="cc575-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cc575-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc575-145">Request</span></span>
<span data-ttu-id="cc575-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc575-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc575-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc575-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cc575-148">C#</span><span class="sxs-lookup"><span data-stu-id="cc575-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc575-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc575-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc575-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc575-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cc575-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc575-151">Response</span></span>

> <span data-ttu-id="cc575-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc575-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

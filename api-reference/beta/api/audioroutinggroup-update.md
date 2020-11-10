---
title: Обновление группы маршрутизации звука
description: Изменение источников и приемников Аудиораутингграуп.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9ca123ad39a307a67c5a91b542eab368dc988b85
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961568"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="d7e73-103">Обновление группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="d7e73-103">Update audio routing group</span></span>

<span data-ttu-id="d7e73-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7e73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7e73-105">Изменение источников и приемников [аудиораутингграуп](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="d7e73-105">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d7e73-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7e73-106">Permissions</span></span>
<span data-ttu-id="d7e73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7e73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7e73-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7e73-109">Permission type</span></span> | <span data-ttu-id="d7e73-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7e73-110">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="d7e73-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7e73-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7e73-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d7e73-112">Not Supported</span></span>                       |
| <span data-ttu-id="d7e73-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7e73-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7e73-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d7e73-114">Not Supported</span></span>                       |
| <span data-ttu-id="d7e73-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7e73-115">Application</span></span>     | <span data-ttu-id="d7e73-116">Calls. Жоинграупкаллс. ALL, Calls.IniТиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="d7e73-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7e73-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7e73-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="d7e73-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="d7e73-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="d7e73-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="d7e73-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7e73-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7e73-120">Request headers</span></span>
| <span data-ttu-id="d7e73-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d7e73-121">Name</span></span>          | <span data-ttu-id="d7e73-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d7e73-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d7e73-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7e73-123">Authorization</span></span> | <span data-ttu-id="d7e73-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7e73-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7e73-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7e73-126">Request body</span></span>
<span data-ttu-id="d7e73-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d7e73-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d7e73-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="d7e73-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d7e73-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d7e73-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d7e73-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7e73-130">Property</span></span>       | <span data-ttu-id="d7e73-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d7e73-131">Type</span></span>    |<span data-ttu-id="d7e73-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d7e73-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d7e73-133">приемники</span><span class="sxs-lookup"><span data-stu-id="d7e73-133">receivers</span></span> | <span data-ttu-id="d7e73-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d7e73-134">String collection</span></span> | <span data-ttu-id="d7e73-135">Целевые участники в Аудиораутингграуп.</span><span class="sxs-lookup"><span data-stu-id="d7e73-135">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="d7e73-136">раутингмоде</span><span class="sxs-lookup"><span data-stu-id="d7e73-136">routingMode</span></span> | <span data-ttu-id="d7e73-137">String</span><span class="sxs-lookup"><span data-stu-id="d7e73-137">String</span></span> | <span data-ttu-id="d7e73-138">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="d7e73-138">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="d7e73-139">sources</span><span class="sxs-lookup"><span data-stu-id="d7e73-139">sources</span></span> | <span data-ttu-id="d7e73-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d7e73-140">String collection</span></span> | <span data-ttu-id="d7e73-141">Участник источника в Аудиораутингграуп.</span><span class="sxs-lookup"><span data-stu-id="d7e73-141">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="d7e73-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7e73-142">Response</span></span>
<span data-ttu-id="d7e73-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [аудиораутингграуп](../resources/audioroutinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7e73-143">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7e73-144">Пример</span><span class="sxs-lookup"><span data-stu-id="d7e73-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d7e73-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7e73-145">Request</span></span>
<span data-ttu-id="d7e73-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7e73-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7e73-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7e73-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d7e73-148">C#</span><span class="sxs-lookup"><span data-stu-id="d7e73-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7e73-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7e73-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7e73-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7e73-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7e73-151">Java</span><span class="sxs-lookup"><span data-stu-id="d7e73-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-audioroutinggroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d7e73-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7e73-152">Response</span></span>

> <span data-ttu-id="d7e73-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7e73-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



---
title: Создание группы маршрутизации звука
description: Создание нового **аудиораутингграуп**.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7b34bc058c116a9be78f491f8dc2e826ea09f0c6
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005980"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="8a7ee-103">Создание группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="8a7ee-103">Create audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a7ee-104">Создание нового **аудиораутингграуп**.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-104">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a7ee-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a7ee-105">Permissions</span></span>
<span data-ttu-id="8a7ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a7ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a7ee-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a7ee-108">Permission type</span></span>                        | <span data-ttu-id="8a7ee-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a7ee-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8a7ee-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a7ee-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a7ee-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-111">Not supported.</span></span>                               |
| <span data-ttu-id="8a7ee-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a7ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a7ee-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-113">Not supported.</span></span>                               |
| <span data-ttu-id="8a7ee-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a7ee-114">Application</span></span>                            | <span data-ttu-id="8a7ee-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="8a7ee-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a7ee-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a7ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /communications/calls/{id}/audioRoutingGroups
```
> <span data-ttu-id="8a7ee-117">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="8a7ee-118">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a7ee-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a7ee-119">Request headers</span></span>
| <span data-ttu-id="8a7ee-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8a7ee-120">Name</span></span>          | <span data-ttu-id="8a7ee-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8a7ee-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8a7ee-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a7ee-122">Authorization</span></span> | <span data-ttu-id="8a7ee-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a7ee-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a7ee-125">Request body</span></span>
<span data-ttu-id="8a7ee-126">В тексте запроса добавьте представление объекта [аудиораутингграуп](../resources/audioroutinggroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-126">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8a7ee-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a7ee-127">Response</span></span>
<span data-ttu-id="8a7ee-128">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [аудиораутингграуп](../resources/audioroutinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-128">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8a7ee-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="8a7ee-129">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="8a7ee-130">Пример 1: "одна к одной группе маршрутизации аудио"</span><span class="sxs-lookup"><span data-stu-id="8a7ee-130">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="8a7ee-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a7ee-131">Request</span></span>
<span data-ttu-id="8a7ee-132">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-132">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8a7ee-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a7ee-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-audioRoutingGroup-from-call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8a7ee-134">C#</span><span class="sxs-lookup"><span data-stu-id="8a7ee-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-audioroutinggroup-from-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8a7ee-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a7ee-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-audioroutinggroup-from-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8a7ee-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a7ee-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-audioroutinggroup-from-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="8a7ee-137">В тексте запроса добавьте представление объекта [аудиораутингграуп](../resources/audioroutinggroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-137">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="8a7ee-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a7ee-138">Response</span></span>

> <span data-ttu-id="8a7ee-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
}
```
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="8a7ee-141">Пример 2: multicast Аудиораутингграуп</span><span class="sxs-lookup"><span data-stu-id="8a7ee-141">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="8a7ee-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a7ee-142">Request</span></span>
<span data-ttu-id="8a7ee-143">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-143">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233
```

<!-- {
  "blockType": "example",
  "name": "create-audioRoutingGroup-from-call",
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->

```json
{
  "id": "multicast",
  "routingMode": "multicast",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<span data-ttu-id="8a7ee-144">В тексте запроса добавьте представление объекта [аудиораутингграуп](../resources/audioroutinggroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-144">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="8a7ee-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a7ee-145">Response</span></span>

> <span data-ttu-id="8a7ee-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a7ee-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233
```
<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->

```json
{
  "id": "multicast",
  "routingMode": "multicast",
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
  "description": "Create audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

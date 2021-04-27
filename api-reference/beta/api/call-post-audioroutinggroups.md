---
title: Создание группы маршрутизации звука
description: Создание новой **audioRoutingGroup**.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f4c7cbc969b676db6786bf0d708e92381fd4cecf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047632"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="b71d9-103">Создание группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="b71d9-103">Create audio routing group</span></span>

<span data-ttu-id="b71d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b71d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b71d9-105">Создание новой **audioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="b71d9-105">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="b71d9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b71d9-106">Permissions</span></span>
<span data-ttu-id="b71d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b71d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b71d9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b71d9-109">Permission type</span></span>                        | <span data-ttu-id="b71d9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b71d9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b71d9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b71d9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b71d9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b71d9-112">Not supported.</span></span>                               |
| <span data-ttu-id="b71d9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b71d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b71d9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b71d9-114">Not supported.</span></span>                               |
| <span data-ttu-id="b71d9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b71d9-115">Application</span></span>                            | <span data-ttu-id="b71d9-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="b71d9-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b71d9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b71d9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /communications/calls/{id}/audioRoutingGroups
```
> <span data-ttu-id="b71d9-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="b71d9-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="b71d9-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="b71d9-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b71d9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b71d9-120">Request headers</span></span>
| <span data-ttu-id="b71d9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b71d9-121">Name</span></span>          | <span data-ttu-id="b71d9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b71d9-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b71d9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b71d9-123">Authorization</span></span> | <span data-ttu-id="b71d9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b71d9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b71d9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b71d9-126">Request body</span></span>
<span data-ttu-id="b71d9-127">В корпусе запроса поставляем представление JSON объекта [audioRoutingGroup.](../resources/audioroutinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="b71d9-127">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b71d9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b71d9-128">Response</span></span>
<span data-ttu-id="b71d9-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект audioRoutingGroup](../resources/audioroutinggroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b71d9-129">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b71d9-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="b71d9-130">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="b71d9-131">Пример 1. Группа маршрутизания звука один к одному</span><span class="sxs-lookup"><span data-stu-id="b71d9-131">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="b71d9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b71d9-132">Request</span></span>
<span data-ttu-id="b71d9-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b71d9-133">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b71d9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b71d9-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b71d9-135">C#</span><span class="sxs-lookup"><span data-stu-id="b71d9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-audioroutinggroup-from-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b71d9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b71d9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-audioroutinggroup-from-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b71d9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b71d9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-audioroutinggroup-from-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b71d9-138">Java</span><span class="sxs-lookup"><span data-stu-id="b71d9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-audioroutinggroup-from-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="b71d9-139">В корпусе запроса поставляем представление JSON объекта [audioRoutingGroup.](../resources/audioroutinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="b71d9-139">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="b71d9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b71d9-140">Response</span></span>

> <span data-ttu-id="b71d9-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b71d9-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="b71d9-142">Пример 2. Многоуровневая аудионастройкаGroup</span><span class="sxs-lookup"><span data-stu-id="b71d9-142">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="b71d9-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="b71d9-143">Request</span></span>
<span data-ttu-id="b71d9-144">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b71d9-144">The following example shows the request.</span></span>

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

<span data-ttu-id="b71d9-145">В корпусе запроса поставляем представление JSON объекта [audioRoutingGroup.](../resources/audioroutinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="b71d9-145">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="b71d9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b71d9-146">Response</span></span>

> <span data-ttu-id="b71d9-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b71d9-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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



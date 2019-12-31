---
title: Создание группы маршрутизации звука
description: Создание нового **аудиораутингграуп**.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7a5c6f43183ffdb4f01df689bd3fe20cdf3688cd
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912827"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="a0d88-103">Создание группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="a0d88-103">Create audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0d88-104">Создание нового **аудиораутингграуп**.</span><span class="sxs-lookup"><span data-stu-id="a0d88-104">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0d88-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0d88-105">Permissions</span></span>
<span data-ttu-id="a0d88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0d88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0d88-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0d88-108">Permission type</span></span>                        | <span data-ttu-id="a0d88-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0d88-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a0d88-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0d88-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0d88-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0d88-111">Not supported.</span></span>                               |
| <span data-ttu-id="a0d88-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0d88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0d88-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0d88-113">Not supported.</span></span>                               |
| <span data-ttu-id="a0d88-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0d88-114">Application</span></span>                            | <span data-ttu-id="a0d88-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="a0d88-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0d88-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0d88-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /communications/calls/{id}/audioRoutingGroups
```
> <span data-ttu-id="a0d88-117">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="a0d88-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="a0d88-118">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="a0d88-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0d88-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0d88-119">Request headers</span></span>
| <span data-ttu-id="a0d88-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a0d88-120">Name</span></span>          | <span data-ttu-id="a0d88-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a0d88-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a0d88-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0d88-122">Authorization</span></span> | <span data-ttu-id="a0d88-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0d88-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0d88-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0d88-125">Request body</span></span>
<span data-ttu-id="a0d88-126">В тексте запроса добавьте представление объекта [аудиораутингграуп](../resources/audioroutinggroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0d88-126">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a0d88-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0d88-127">Response</span></span>
<span data-ttu-id="a0d88-128">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [аудиораутингграуп](../resources/audioroutinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0d88-128">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0d88-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="a0d88-129">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="a0d88-130">Пример 1: "одна к одной группе маршрутизации аудио"</span><span class="sxs-lookup"><span data-stu-id="a0d88-130">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="a0d88-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0d88-131">Request</span></span>
<span data-ttu-id="a0d88-132">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0d88-132">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a0d88-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0d88-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a0d88-134">C#</span><span class="sxs-lookup"><span data-stu-id="a0d88-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-audioroutinggroup-from-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0d88-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0d88-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-audioroutinggroup-from-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a0d88-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0d88-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-audioroutinggroup-from-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a0d88-137">В тексте запроса добавьте представление объекта [аудиораутингграуп](../resources/audioroutinggroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0d88-137">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="a0d88-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0d88-138">Response</span></span>

> <span data-ttu-id="a0d88-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0d88-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="a0d88-141">Пример 2: multicast Аудиораутингграуп</span><span class="sxs-lookup"><span data-stu-id="a0d88-141">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="a0d88-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0d88-142">Request</span></span>
<span data-ttu-id="a0d88-143">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0d88-143">The following example shows the request.</span></span>

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

<span data-ttu-id="a0d88-144">В тексте запроса добавьте представление объекта [аудиораутингграуп](../resources/audioroutinggroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0d88-144">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="a0d88-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0d88-145">Response</span></span>

> <span data-ttu-id="a0d88-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0d88-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

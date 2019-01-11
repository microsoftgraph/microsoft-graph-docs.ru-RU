---
title: Создание звуковых группы маршрутизации
description: Создание нового **audioRoutingGroup**.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 4f8a430e46137d54df5fc6d99a9676f4faa0d5ee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838481"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="df4a8-103">Создание звуковых группы маршрутизации</span><span class="sxs-lookup"><span data-stu-id="df4a8-103">Create audio routing group</span></span>

> <span data-ttu-id="df4a8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="df4a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df4a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df4a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df4a8-106">Создание нового **audioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="df4a8-106">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="df4a8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df4a8-107">Permissions</span></span>
<span data-ttu-id="df4a8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df4a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df4a8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df4a8-110">Permission type</span></span>                        | <span data-ttu-id="df4a8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df4a8-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="df4a8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df4a8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="df4a8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df4a8-113">Not supported.</span></span>                               |
| <span data-ttu-id="df4a8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df4a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df4a8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df4a8-115">Not supported.</span></span>                               |
| <span data-ttu-id="df4a8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df4a8-116">Application</span></span>                            | <span data-ttu-id="df4a8-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="df4a8-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df4a8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df4a8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="df4a8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df4a8-119">Request headers</span></span>
| <span data-ttu-id="df4a8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="df4a8-120">Name</span></span>          | <span data-ttu-id="df4a8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="df4a8-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="df4a8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df4a8-122">Authorization</span></span> | <span data-ttu-id="df4a8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df4a8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df4a8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="df4a8-125">Request body</span></span>
<span data-ttu-id="df4a8-126">В тексте запроса укажите представление JSON объекта [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="df4a8-126">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="df4a8-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="df4a8-127">Response</span></span>
<span data-ttu-id="df4a8-128">Успешно завершена, этот метод возвращает `200 OK` объект [audioRoutingGroup](../resources/audioroutinggroup.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="df4a8-128">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df4a8-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="df4a8-129">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="df4a8-130">В примере 1: Один к одному группу звука маршрутизации</span><span class="sxs-lookup"><span data-stu-id="df4a8-130">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="df4a8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="df4a8-131">Request</span></span>
<span data-ttu-id="df4a8-132">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df4a8-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-audioRoutingGroup-from-call"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
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

<span data-ttu-id="df4a8-133">В тексте запроса укажите представление JSON объекта [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="df4a8-133">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="df4a8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="df4a8-134">Response</span></span>

> <span data-ttu-id="df4a8-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df4a8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="df4a8-137">Пример 2: AudioRoutingGroup многоадресной рассылки</span><span class="sxs-lookup"><span data-stu-id="df4a8-137">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="df4a8-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="df4a8-138">Request</span></span>
<span data-ttu-id="df4a8-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df4a8-139">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
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

<span data-ttu-id="df4a8-140">В тексте запроса укажите представление JSON объекта [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="df4a8-140">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="df4a8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="df4a8-141">Response</span></span>

> <span data-ttu-id="df4a8-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df4a8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

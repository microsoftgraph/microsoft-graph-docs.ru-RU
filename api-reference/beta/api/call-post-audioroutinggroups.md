---
title: Создание звуковых группы маршрутизации
description: Создание нового **audioRoutingGroup**.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dc0e2a3463229762b3a641f33f77f2df8d506aa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522863"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="44165-103">Создание звуковых группы маршрутизации</span><span class="sxs-lookup"><span data-stu-id="44165-103">Create audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44165-104">Создание нового **audioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="44165-104">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="44165-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44165-105">Permissions</span></span>
<span data-ttu-id="44165-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44165-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44165-108">Permission type</span></span>                        | <span data-ttu-id="44165-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44165-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="44165-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44165-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="44165-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44165-111">Not supported.</span></span>                               |
| <span data-ttu-id="44165-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44165-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44165-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44165-113">Not supported.</span></span>                               |
| <span data-ttu-id="44165-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44165-114">Application</span></span>                            | <span data-ttu-id="44165-115">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="44165-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44165-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44165-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="44165-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44165-117">Request headers</span></span>
| <span data-ttu-id="44165-118">Имя</span><span class="sxs-lookup"><span data-stu-id="44165-118">Name</span></span>          | <span data-ttu-id="44165-119">Описание</span><span class="sxs-lookup"><span data-stu-id="44165-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="44165-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44165-120">Authorization</span></span> | <span data-ttu-id="44165-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44165-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44165-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44165-123">Request body</span></span>
<span data-ttu-id="44165-124">В тексте запроса укажите представление JSON объекта [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="44165-124">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="44165-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="44165-125">Response</span></span>
<span data-ttu-id="44165-126">Успешно завершена, этот метод возвращает `200 OK` объект [audioRoutingGroup](../resources/audioroutinggroup.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="44165-126">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44165-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="44165-127">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="44165-128">В примере 1: Один к одному группу звука маршрутизации</span><span class="sxs-lookup"><span data-stu-id="44165-128">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="44165-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="44165-129">Request</span></span>
<span data-ttu-id="44165-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44165-130">The following example shows the request.</span></span>

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

<span data-ttu-id="44165-131">В тексте запроса укажите представление JSON объекта [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="44165-131">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="44165-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="44165-132">Response</span></span>

> <span data-ttu-id="44165-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44165-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="44165-135">Пример 2: AudioRoutingGroup многоадресной рассылки</span><span class="sxs-lookup"><span data-stu-id="44165-135">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="44165-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="44165-136">Request</span></span>
<span data-ttu-id="44165-137">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44165-137">The following example shows the request.</span></span>

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

<span data-ttu-id="44165-138">В тексте запроса укажите представление JSON объекта [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="44165-138">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="44165-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="44165-139">Response</span></span>

> <span data-ttu-id="44165-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44165-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/call-post-audioroutinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

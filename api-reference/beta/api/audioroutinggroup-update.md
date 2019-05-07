---
title: Обновление группы маршрутизации звука
description: Изменение источников и приемников Аудиораутингграуп.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 835298804e2b409f75ef4d0e86786951f7ae0099
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636424"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="576fa-103">Обновление группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="576fa-103">Update audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="576fa-104">Изменение источников и приемников [аудиораутингграуп](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="576fa-104">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="576fa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="576fa-105">Permissions</span></span>
<span data-ttu-id="576fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="576fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="576fa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="576fa-108">Permission type</span></span> | <span data-ttu-id="576fa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="576fa-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="576fa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="576fa-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="576fa-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="576fa-111">Not Supported</span></span>                       |
| <span data-ttu-id="576fa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="576fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="576fa-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="576fa-113">Not Supported</span></span>                       |
| <span data-ttu-id="576fa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="576fa-114">Application</span></span>     | <span data-ttu-id="576fa-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="576fa-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="576fa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="576fa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="576fa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="576fa-117">Request headers</span></span>
| <span data-ttu-id="576fa-118">Имя</span><span class="sxs-lookup"><span data-stu-id="576fa-118">Name</span></span>          | <span data-ttu-id="576fa-119">Описание</span><span class="sxs-lookup"><span data-stu-id="576fa-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="576fa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="576fa-120">Authorization</span></span> | <span data-ttu-id="576fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="576fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="576fa-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="576fa-123">Request body</span></span>
<span data-ttu-id="576fa-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="576fa-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="576fa-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="576fa-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="576fa-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="576fa-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="576fa-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="576fa-127">Property</span></span>       | <span data-ttu-id="576fa-128">Тип</span><span class="sxs-lookup"><span data-stu-id="576fa-128">Type</span></span>    |<span data-ttu-id="576fa-129">Описание</span><span class="sxs-lookup"><span data-stu-id="576fa-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="576fa-130">приемники</span><span class="sxs-lookup"><span data-stu-id="576fa-130">receivers</span></span> | <span data-ttu-id="576fa-131">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="576fa-131">String collection</span></span> | <span data-ttu-id="576fa-132">Целевые участники в Аудиораутингграуп.</span><span class="sxs-lookup"><span data-stu-id="576fa-132">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="576fa-133">Раутингмоде</span><span class="sxs-lookup"><span data-stu-id="576fa-133">routingMode</span></span> | <span data-ttu-id="576fa-134">String</span><span class="sxs-lookup"><span data-stu-id="576fa-134">String</span></span> | <span data-ttu-id="576fa-135">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="576fa-135">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="576fa-136">sources</span><span class="sxs-lookup"><span data-stu-id="576fa-136">sources</span></span> | <span data-ttu-id="576fa-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="576fa-137">String collection</span></span> | <span data-ttu-id="576fa-138">Участник источника в Аудиораутингграуп.</span><span class="sxs-lookup"><span data-stu-id="576fa-138">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="576fa-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="576fa-139">Response</span></span>
<span data-ttu-id="576fa-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [аудиораутингграуп](../resources/audioroutinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="576fa-140">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="576fa-141">Пример</span><span class="sxs-lookup"><span data-stu-id="576fa-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="576fa-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="576fa-142">Request</span></span>
<span data-ttu-id="576fa-143">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="576fa-143">The following example shows the request.</span></span>

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
##### <a name="response"></a><span data-ttu-id="576fa-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="576fa-144">Response</span></span>

> <span data-ttu-id="576fa-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="576fa-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="576fa-147">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="576fa-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="576fa-148">Языках</span><span class="sxs-lookup"><span data-stu-id="576fa-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update-audioRoutingGroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="576fa-149">Язык</span><span class="sxs-lookup"><span data-stu-id="576fa-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update-audioRoutingGroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/audioroutinggroup-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/audioroutinggroup-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

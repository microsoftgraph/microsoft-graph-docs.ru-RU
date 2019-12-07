---
title: Обновление Свапшифтсчанжерекуест
description: Обновление свойств объекта Свапшифтсчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 141b011ab1dbca436c39e9e48f8312fea77ec6f0
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895819"
---
# <a name="update-swapshiftschangerequest"></a><span data-ttu-id="d403d-103">Обновление Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="d403d-103">Update swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d403d-104">Обновление свойств объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d403d-104">Update the properties of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d403d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d403d-105">Permissions</span></span>

<span data-ttu-id="d403d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d403d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d403d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d403d-108">Permission type</span></span>                        | <span data-ttu-id="d403d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d403d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d403d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d403d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d403d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d403d-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d403d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d403d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d403d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d403d-113">Not supported.</span></span> |
| <span data-ttu-id="d403d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d403d-114">Application</span></span>                            | <span data-ttu-id="d403d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d403d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d403d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d403d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="d403d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d403d-117">Request headers</span></span>

| <span data-ttu-id="d403d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d403d-118">Name</span></span>       | <span data-ttu-id="d403d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d403d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d403d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d403d-120">Authorization</span></span> | <span data-ttu-id="d403d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d403d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d403d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d403d-123">Content-type</span></span> | <span data-ttu-id="d403d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d403d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d403d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d403d-126">Request body</span></span>

<span data-ttu-id="d403d-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d403d-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d403d-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="d403d-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d403d-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d403d-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d403d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d403d-130">Property</span></span>     | <span data-ttu-id="d403d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d403d-131">Type</span></span>        | <span data-ttu-id="d403d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d403d-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d403d-133">реЦипиентшифтид</span><span class="sxs-lookup"><span data-stu-id="d403d-133">recipientShiftId</span></span>|<span data-ttu-id="d403d-134">String</span><span class="sxs-lookup"><span data-stu-id="d403d-134">String</span></span>|<span data-ttu-id="d403d-135">Идентификатор получателя запроса на замену.</span><span class="sxs-lookup"><span data-stu-id="d403d-135">The ID of the recipient of the swap request.</span></span> <span data-ttu-id="d403d-136">Это пользователь, который запрашивается для замены.</span><span class="sxs-lookup"><span data-stu-id="d403d-136">This is the user who is requested to swap with.</span></span>|

## <a name="response"></a><span data-ttu-id="d403d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d403d-137">Response</span></span>

<span data-ttu-id="d403d-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d403d-138">If successful, this method returns a `200 OK` response code and an updated [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d403d-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="d403d-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d403d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d403d-140">Request</span></span>

<span data-ttu-id="d403d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d403d-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_swapshiftschangerequest"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests
Content-type: application/json

{
  "recipientShiftId": "recipientShiftId-value"
}
```

### <a name="response"></a><span data-ttu-id="d403d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d403d-142">Response</span></span>

<span data-ttu-id="d403d-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d403d-143">The following is an example of the response.</span></span>

> <span data-ttu-id="d403d-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d403d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientShiftId": "recipientShiftId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update swapshiftschangerequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Обновление Свапшифтсчанжерекуест
description: Обновление свойств объекта Свапшифтсчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b0955428ce82f585bbdb085e0d6d2f2f6023f92f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870802"
---
# <a name="update-swapshiftschangerequest"></a><span data-ttu-id="e1c4b-103">Обновление Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="e1c4b-103">Update swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1c4b-104">Обновление свойств объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="e1c4b-104">Update the properties of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1c4b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1c4b-105">Permissions</span></span>

<span data-ttu-id="e1c4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1c4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1c4b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1c4b-108">Permission type</span></span>                        | <span data-ttu-id="e1c4b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1c4b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e1c4b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1c4b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1c4b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1c4b-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="e1c4b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1c4b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1c4b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-113">Not supported.</span></span> |
|<span data-ttu-id="e1c4b-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="e1c4b-114">Application</span></span> | <span data-ttu-id="e1c4b-115">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="e1c4b-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="e1c4b-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="e1c4b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1c4b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="e1c4b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1c4b-118">Request headers</span></span>

| <span data-ttu-id="e1c4b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e1c4b-119">Name</span></span>       | <span data-ttu-id="e1c4b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e1c4b-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e1c4b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1c4b-121">Authorization</span></span> | <span data-ttu-id="e1c4b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1c4b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1c4b-124">Content-type</span></span> | <span data-ttu-id="e1c4b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1c4b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1c4b-127">Request body</span></span>

<span data-ttu-id="e1c4b-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e1c4b-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e1c4b-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e1c4b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1c4b-131">Property</span></span>     | <span data-ttu-id="e1c4b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e1c4b-132">Type</span></span>        | <span data-ttu-id="e1c4b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e1c4b-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e1c4b-134">реЦипиентшифтид</span><span class="sxs-lookup"><span data-stu-id="e1c4b-134">recipientShiftId</span></span>|<span data-ttu-id="e1c4b-135">String</span><span class="sxs-lookup"><span data-stu-id="e1c4b-135">String</span></span>|<span data-ttu-id="e1c4b-136">Идентификатор получателя запроса на замену.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-136">The ID of the recipient of the swap request.</span></span> <span data-ttu-id="e1c4b-137">Это пользователь, который запрашивается для замены.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-137">This is the user who is requested to swap with.</span></span>|

## <a name="response"></a><span data-ttu-id="e1c4b-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1c4b-138">Response</span></span>

<span data-ttu-id="e1c4b-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-139">If successful, this method returns a `200 OK` response code and an updated [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1c4b-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="e1c4b-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e1c4b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1c4b-141">Request</span></span>

<span data-ttu-id="e1c4b-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e1c4b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1c4b-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1c4b-144">C#</span><span class="sxs-lookup"><span data-stu-id="e1c4b-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-swapshiftschangerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1c4b-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1c4b-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-swapshiftschangerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1c4b-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1c4b-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-swapshiftschangerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e1c4b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1c4b-147">Response</span></span>

<span data-ttu-id="e1c4b-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-148">The following is an example of the response.</span></span>

> <span data-ttu-id="e1c4b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1c4b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

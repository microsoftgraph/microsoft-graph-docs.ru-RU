---
title: Обновление Опеншифтчанжерекуест
description: Обновление свойств объекта Опеншифтчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e58461437206809e1c71803c03781b704323fc81
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895821"
---
# <a name="update-openshiftchangerequest"></a><span data-ttu-id="4c140-103">Обновление опеншифтчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="4c140-103">Update openshiftchangerequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c140-104">Обновление свойств объекта [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="4c140-104">Update the properties of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c140-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c140-105">Permissions</span></span>

<span data-ttu-id="4c140-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c140-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c140-108">Permission type</span></span>                        | <span data-ttu-id="4c140-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c140-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4c140-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c140-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c140-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c140-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4c140-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c140-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c140-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c140-113">Not supported.</span></span> |
| <span data-ttu-id="4c140-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c140-114">Application</span></span>                            | <span data-ttu-id="4c140-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c140-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c140-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c140-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="4c140-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c140-117">Request headers</span></span>

| <span data-ttu-id="4c140-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4c140-118">Name</span></span>       | <span data-ttu-id="4c140-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4c140-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4c140-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c140-120">Authorization</span></span> | <span data-ttu-id="4c140-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c140-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c140-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c140-123">Content-type</span></span> | <span data-ttu-id="4c140-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c140-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c140-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c140-126">Request body</span></span>

<span data-ttu-id="4c140-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4c140-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4c140-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4c140-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4c140-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4c140-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4c140-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c140-130">Property</span></span>     | <span data-ttu-id="4c140-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4c140-131">Type</span></span>        | <span data-ttu-id="4c140-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4c140-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4c140-133">опеншифтид</span><span class="sxs-lookup"><span data-stu-id="4c140-133">openShiftId</span></span>|<span data-ttu-id="4c140-134">String</span><span class="sxs-lookup"><span data-stu-id="4c140-134">String</span></span>|<span data-ttu-id="4c140-135">Идентификатор для открытой смены.</span><span class="sxs-lookup"><span data-stu-id="4c140-135">ID for the open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="4c140-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c140-136">Response</span></span>

<span data-ttu-id="4c140-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c140-137">If successful, this method returns a `200 OK` response code and an updated [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c140-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c140-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c140-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c140-139">Request</span></span>

<span data-ttu-id="4c140-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c140-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_openshiftchangerequest"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests
Content-type: application/json

{
  "openShiftId": "openShiftId-value"
}
```

### <a name="response"></a><span data-ttu-id="4c140-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c140-141">Response</span></span>

<span data-ttu-id="4c140-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c140-142">The following is an example of the response.</span></span>

> <span data-ttu-id="4c140-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c140-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "openShiftId": "openShiftId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update openshiftchangerequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

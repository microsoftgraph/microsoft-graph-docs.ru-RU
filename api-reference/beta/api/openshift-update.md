---
title: Обновление Опеншифт
description: Обновление свойств объекта Опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5863b3a52eb195fed205788480cf1e5eda1237eb
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895833"
---
# <a name="update-openshift"></a><span data-ttu-id="0409a-103">Обновление Опеншифт</span><span class="sxs-lookup"><span data-stu-id="0409a-103">Update openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0409a-104">Обновление свойств объекта [опеншифт](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="0409a-104">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0409a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0409a-105">Permissions</span></span>

<span data-ttu-id="0409a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0409a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0409a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0409a-108">Permission type</span></span>                        | <span data-ttu-id="0409a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0409a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0409a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0409a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0409a-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0409a-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="0409a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0409a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0409a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0409a-113">Not supported.</span></span> |
| <span data-ttu-id="0409a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0409a-114">Application</span></span>                            | <span data-ttu-id="0409a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0409a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0409a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0409a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/openShifts
```

## <a name="request-headers"></a><span data-ttu-id="0409a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0409a-117">Request headers</span></span>

| <span data-ttu-id="0409a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0409a-118">Name</span></span>       | <span data-ttu-id="0409a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0409a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0409a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0409a-120">Authorization</span></span> | <span data-ttu-id="0409a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0409a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0409a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0409a-123">Content-type</span></span> | <span data-ttu-id="0409a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0409a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0409a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0409a-126">Request body</span></span>

<span data-ttu-id="0409a-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0409a-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0409a-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0409a-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0409a-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0409a-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0409a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0409a-130">Property</span></span>     | <span data-ttu-id="0409a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0409a-131">Type</span></span>        | <span data-ttu-id="0409a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0409a-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0409a-133">драфтопеншифт</span><span class="sxs-lookup"><span data-stu-id="0409a-133">draftOpenShift</span></span>|<span data-ttu-id="0409a-134">опеншифтитем</span><span class="sxs-lookup"><span data-stu-id="0409a-134">openShiftItem</span></span>|<span data-ttu-id="0409a-135">Неопубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="0409a-135">An unpublished open shift.</span></span>|
|<span data-ttu-id="0409a-136">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="0409a-136">schedulingGroupId</span></span>|<span data-ttu-id="0409a-137">String</span><span class="sxs-lookup"><span data-stu-id="0409a-137">String</span></span>| <span data-ttu-id="0409a-138">Планирование кода группы.</span><span class="sxs-lookup"><span data-stu-id="0409a-138">Scheduling group id.</span></span> |
|<span data-ttu-id="0409a-139">шаредопеншифт</span><span class="sxs-lookup"><span data-stu-id="0409a-139">sharedOpenShift</span></span>|<span data-ttu-id="0409a-140">опеншифтитем</span><span class="sxs-lookup"><span data-stu-id="0409a-140">openShiftItem</span></span>|<span data-ttu-id="0409a-141">Опубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="0409a-141">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="0409a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0409a-142">Response</span></span>

<span data-ttu-id="0409a-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [опеншифт](../resources/openshift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0409a-143">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0409a-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="0409a-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0409a-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="0409a-145">Request</span></span>

<span data-ttu-id="0409a-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0409a-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_openshift"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts
Content-type: application/json

{
  "sharedOpenShift": {
    "openSlotCount": 99
  },
  "draftOpenShift": {
    "openSlotCount": 99
  },
  "schedulingGroupId": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263"
}
```

### <a name="response"></a><span data-ttu-id="0409a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0409a-147">Response</span></span>

<span data-ttu-id="0409a-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0409a-148">The following is an example of the response.</span></span>

> <span data-ttu-id="0409a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0409a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "sharedOpenShift": {
    "openSlotCount": 99
  },
  "draftOpenShift": {
    "openSlotCount": 99
  },
  "schedulingGroupId": "schedulingGroupId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update openshift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

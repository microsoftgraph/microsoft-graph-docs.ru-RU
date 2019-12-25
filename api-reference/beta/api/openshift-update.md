---
title: Обновление Опеншифт
description: Обновление свойств объекта Опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 821ad6579d7e77959263aab91511e71e0352e364
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867803"
---
# <a name="update-openshift"></a><span data-ttu-id="39386-103">Обновление Опеншифт</span><span class="sxs-lookup"><span data-stu-id="39386-103">Update openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39386-104">Обновление свойств объекта [опеншифт](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="39386-104">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39386-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39386-105">Permissions</span></span>

<span data-ttu-id="39386-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39386-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39386-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39386-108">Permission type</span></span>                        | <span data-ttu-id="39386-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39386-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="39386-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39386-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="39386-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39386-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="39386-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39386-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39386-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39386-113">Not supported.</span></span> |
| <span data-ttu-id="39386-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39386-114">Application</span></span>                            | <span data-ttu-id="39386-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39386-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39386-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39386-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/openShifts
```

## <a name="request-headers"></a><span data-ttu-id="39386-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39386-117">Request headers</span></span>

| <span data-ttu-id="39386-118">Имя</span><span class="sxs-lookup"><span data-stu-id="39386-118">Name</span></span>       | <span data-ttu-id="39386-119">Описание</span><span class="sxs-lookup"><span data-stu-id="39386-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="39386-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39386-120">Authorization</span></span> | <span data-ttu-id="39386-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39386-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39386-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="39386-123">Content-type</span></span> | <span data-ttu-id="39386-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39386-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39386-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39386-126">Request body</span></span>

<span data-ttu-id="39386-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="39386-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="39386-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="39386-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="39386-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="39386-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="39386-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="39386-130">Property</span></span>     | <span data-ttu-id="39386-131">Тип</span><span class="sxs-lookup"><span data-stu-id="39386-131">Type</span></span>        | <span data-ttu-id="39386-132">Описание</span><span class="sxs-lookup"><span data-stu-id="39386-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="39386-133">драфтопеншифт</span><span class="sxs-lookup"><span data-stu-id="39386-133">draftOpenShift</span></span>|<span data-ttu-id="39386-134">опеншифтитем</span><span class="sxs-lookup"><span data-stu-id="39386-134">openShiftItem</span></span>|<span data-ttu-id="39386-135">Неопубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="39386-135">An unpublished open shift.</span></span>|
|<span data-ttu-id="39386-136">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="39386-136">schedulingGroupId</span></span>|<span data-ttu-id="39386-137">String</span><span class="sxs-lookup"><span data-stu-id="39386-137">String</span></span>| <span data-ttu-id="39386-138">Планирование кода группы.</span><span class="sxs-lookup"><span data-stu-id="39386-138">Scheduling group id.</span></span> |
|<span data-ttu-id="39386-139">шаредопеншифт</span><span class="sxs-lookup"><span data-stu-id="39386-139">sharedOpenShift</span></span>|<span data-ttu-id="39386-140">опеншифтитем</span><span class="sxs-lookup"><span data-stu-id="39386-140">openShiftItem</span></span>|<span data-ttu-id="39386-141">Опубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="39386-141">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="39386-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="39386-142">Response</span></span>

<span data-ttu-id="39386-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [опеншифт](../resources/openshift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39386-143">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39386-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="39386-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="39386-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="39386-145">Request</span></span>

<span data-ttu-id="39386-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39386-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="39386-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="39386-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="39386-148">C#</span><span class="sxs-lookup"><span data-stu-id="39386-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="39386-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39386-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="39386-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39386-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="39386-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="39386-151">Response</span></span>

<span data-ttu-id="39386-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39386-152">The following is an example of the response.</span></span>

> <span data-ttu-id="39386-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39386-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

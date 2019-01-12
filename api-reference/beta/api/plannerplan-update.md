---
title: Обновление plannerPlan
description: Обновление свойства объекта **plannerPlan** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 46c4c5707d4e602b75e48a989e6e67136c12387a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945232"
---
# <a name="update-plannerplan"></a><span data-ttu-id="144b0-103">Обновление plannerPlan</span><span class="sxs-lookup"><span data-stu-id="144b0-103">Update plannerPlan</span></span>

> <span data-ttu-id="144b0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="144b0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="144b0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="144b0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="144b0-106">Обновление свойства объекта **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="144b0-106">Update the properties of **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="144b0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="144b0-107">Permissions</span></span>
<span data-ttu-id="144b0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="144b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="144b0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="144b0-110">Permission type</span></span>      | <span data-ttu-id="144b0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="144b0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="144b0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="144b0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="144b0-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="144b0-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="144b0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="144b0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="144b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="144b0-115">Not supported.</span></span>    |
|<span data-ttu-id="144b0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="144b0-116">Application</span></span> | <span data-ttu-id="144b0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="144b0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="144b0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="144b0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>
```

## <a name="request-headers"></a><span data-ttu-id="144b0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="144b0-119">Request headers</span></span>

| <span data-ttu-id="144b0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="144b0-120">Name</span></span>       | <span data-ttu-id="144b0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="144b0-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="144b0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="144b0-122">Authorization</span></span>  | <span data-ttu-id="144b0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="144b0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="144b0-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="144b0-125">If-Match</span></span>  | <span data-ttu-id="144b0-p104">Последнее известное значение ETag обновляемого объекта plannerPlan. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="144b0-p104">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="144b0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="144b0-128">Request body</span></span>
<span data-ttu-id="144b0-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="144b0-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="144b0-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="144b0-132">Property</span></span>     | <span data-ttu-id="144b0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="144b0-133">Type</span></span>   |<span data-ttu-id="144b0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="144b0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="144b0-135">owner</span><span class="sxs-lookup"><span data-stu-id="144b0-135">owner</span></span>|<span data-ttu-id="144b0-136">Строка</span><span class="sxs-lookup"><span data-stu-id="144b0-136">String</span></span>|<span data-ttu-id="144b0-p106">Идентификатор `id` [группы](../resources/group.md), которой принадлежит план. Чтобы в этом поле можно было указать значение, должна существовать подходящая группа. Указанное значение может изменить только владелец.</span><span class="sxs-lookup"><span data-stu-id="144b0-p106">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="144b0-140">title</span><span class="sxs-lookup"><span data-stu-id="144b0-140">title</span></span>|<span data-ttu-id="144b0-141">Строка</span><span class="sxs-lookup"><span data-stu-id="144b0-141">String</span></span>|<span data-ttu-id="144b0-142">Название плана.</span><span class="sxs-lookup"><span data-stu-id="144b0-142">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="144b0-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="144b0-143">Response</span></span>

<span data-ttu-id="144b0-144">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="144b0-144">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="144b0-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="144b0-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="144b0-148">Пример</span><span class="sxs-lookup"><span data-stu-id="144b0-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="144b0-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="144b0-149">Request</span></span>
<span data-ttu-id="144b0-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="144b0-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/<id>
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
##### <a name="response"></a><span data-ttu-id="144b0-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="144b0-151">Response</span></span>
<span data-ttu-id="144b0-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="144b0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

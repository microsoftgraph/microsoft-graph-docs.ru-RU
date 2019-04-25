---
title: Обновление plannerPlan
description: Обновление свойств объекта **plannerPlan** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d4f8f3c3704c1108485ec21e5ac4a8836a401925
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525700"
---
# <a name="update-plannerplan"></a><span data-ttu-id="52825-103">Обновление plannerPlan</span><span class="sxs-lookup"><span data-stu-id="52825-103">Update plannerPlan</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52825-104">Обновление свойств объекта **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="52825-104">Update the properties of **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="52825-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52825-105">Permissions</span></span>
<span data-ttu-id="52825-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52825-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52825-108">Permission type</span></span>      | <span data-ttu-id="52825-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52825-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52825-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52825-110">Delegated (work or school account)</span></span> | <span data-ttu-id="52825-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52825-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="52825-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52825-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52825-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52825-113">Not supported.</span></span>    |
|<span data-ttu-id="52825-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52825-114">Application</span></span> | <span data-ttu-id="52825-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52825-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52825-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52825-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>
```

## <a name="request-headers"></a><span data-ttu-id="52825-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52825-117">Request headers</span></span>

| <span data-ttu-id="52825-118">Имя</span><span class="sxs-lookup"><span data-stu-id="52825-118">Name</span></span>       | <span data-ttu-id="52825-119">Описание</span><span class="sxs-lookup"><span data-stu-id="52825-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="52825-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52825-120">Authorization</span></span>  | <span data-ttu-id="52825-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52825-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52825-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="52825-123">If-Match</span></span>  | <span data-ttu-id="52825-p103">Последнее известное значение ETag обновляемого объекта plannerPlan. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52825-p103">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52825-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52825-126">Request body</span></span>
<span data-ttu-id="52825-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="52825-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="52825-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="52825-130">Property</span></span>     | <span data-ttu-id="52825-131">Тип</span><span class="sxs-lookup"><span data-stu-id="52825-131">Type</span></span>   |<span data-ttu-id="52825-132">Описание</span><span class="sxs-lookup"><span data-stu-id="52825-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52825-133">owner</span><span class="sxs-lookup"><span data-stu-id="52825-133">owner</span></span>|<span data-ttu-id="52825-134">String</span><span class="sxs-lookup"><span data-stu-id="52825-134">String</span></span>|<span data-ttu-id="52825-p105">Идентификатор `id` [группы](../resources/group.md), которой принадлежит план. Чтобы в этом поле можно было указать значение, должна существовать подходящая группа. Указанное значение может изменить только владелец.</span><span class="sxs-lookup"><span data-stu-id="52825-p105">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="52825-138">title</span><span class="sxs-lookup"><span data-stu-id="52825-138">title</span></span>|<span data-ttu-id="52825-139">Строка</span><span class="sxs-lookup"><span data-stu-id="52825-139">String</span></span>|<span data-ttu-id="52825-140">Название плана.</span><span class="sxs-lookup"><span data-stu-id="52825-140">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="52825-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="52825-141">Response</span></span>

<span data-ttu-id="52825-142">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="52825-142">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="52825-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="52825-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="52825-146">Пример</span><span class="sxs-lookup"><span data-stu-id="52825-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52825-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="52825-147">Request</span></span>
<span data-ttu-id="52825-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52825-148">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="52825-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="52825-149">Response</span></span>
<span data-ttu-id="52825-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52825-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerplan-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

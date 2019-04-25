---
title: Обновление объекта plannerBucketTaskBoardTaskFormat
description: Обновление свойств объекта **plannerBucketTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f5cf735121fe20200c533a6ce8c77fc8d65ccfde
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525693"
---
# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="698be-103">Обновление объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="698be-103">Update plannerBucketTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="698be-104">Обновление свойств объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="698be-104">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="698be-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="698be-105">Permissions</span></span>
<span data-ttu-id="698be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="698be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="698be-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="698be-108">Permission type</span></span>      | <span data-ttu-id="698be-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="698be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="698be-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="698be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="698be-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="698be-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="698be-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="698be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="698be-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="698be-113">Not supported.</span></span>    |
|<span data-ttu-id="698be-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="698be-114">Application</span></span> | <span data-ttu-id="698be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="698be-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="698be-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="698be-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="698be-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="698be-117">Optional request headers</span></span>
| <span data-ttu-id="698be-118">Имя</span><span class="sxs-lookup"><span data-stu-id="698be-118">Name</span></span>       | <span data-ttu-id="698be-119">Описание</span><span class="sxs-lookup"><span data-stu-id="698be-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="698be-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="698be-120">Authorization</span></span>  | <span data-ttu-id="698be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="698be-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="698be-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="698be-123">If-Match</span></span>  | <span data-ttu-id="698be-p103">Последнее известное значение ETag обновляемого объекта **plannerBucketTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="698be-p103">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="698be-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="698be-126">Request body</span></span>
<span data-ttu-id="698be-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="698be-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="698be-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="698be-130">Property</span></span>     | <span data-ttu-id="698be-131">Тип</span><span class="sxs-lookup"><span data-stu-id="698be-131">Type</span></span>   |<span data-ttu-id="698be-132">Описание</span><span class="sxs-lookup"><span data-stu-id="698be-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="698be-133">orderHint</span><span class="sxs-lookup"><span data-stu-id="698be-133">orderHint</span></span>|<span data-ttu-id="698be-134">Строка</span><span class="sxs-lookup"><span data-stu-id="698be-134">String</span></span>|<span data-ttu-id="698be-p105">Указание, используемое для расположения задач в окне "Сегмент" доски задачи. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="698be-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="698be-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="698be-137">Response</span></span>

<span data-ttu-id="698be-138">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="698be-138">If successful, this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="698be-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="698be-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="698be-142">Пример</span><span class="sxs-lookup"><span data-stu-id="698be-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="698be-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="698be-143">Request</span></span>
<span data-ttu-id="698be-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="698be-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="698be-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="698be-145">Response</span></span>
<span data-ttu-id="698be-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="698be-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerbuckettaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerbuckettaskboardtaskformat-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: Обновление объекта plannerProgressTaskBoardTaskFormat
description: Обновление свойств объекта **plannerProgressTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 63654112e2a8192d2f84ea42252491f03a839602
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945190"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="662d4-103">Обновление объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="662d4-103">Update plannerProgressTaskBoardTaskFormat</span></span>

> <span data-ttu-id="662d4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="662d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="662d4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="662d4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="662d4-106">Обновление свойств объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="662d4-106">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="662d4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="662d4-107">Permissions</span></span>
<span data-ttu-id="662d4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="662d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="662d4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="662d4-110">Permission type</span></span>      | <span data-ttu-id="662d4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="662d4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="662d4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="662d4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="662d4-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="662d4-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="662d4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="662d4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="662d4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="662d4-115">Not supported.</span></span>    |
|<span data-ttu-id="662d4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="662d4-116">Application</span></span> | <span data-ttu-id="662d4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="662d4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="662d4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="662d4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="662d4-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="662d4-119">Optional request headers</span></span>
| <span data-ttu-id="662d4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="662d4-120">Name</span></span>       | <span data-ttu-id="662d4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="662d4-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="662d4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="662d4-122">Authorization</span></span>  | <span data-ttu-id="662d4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="662d4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="662d4-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="662d4-125">If-Match</span></span>  | <span data-ttu-id="662d4-p104">Последнее известное значение ETag обновляемого объекта **plannerProgressTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="662d4-p104">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="662d4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="662d4-128">Request body</span></span>
<span data-ttu-id="662d4-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="662d4-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="662d4-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="662d4-132">Property</span></span>     | <span data-ttu-id="662d4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="662d4-133">Type</span></span>   |<span data-ttu-id="662d4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="662d4-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="662d4-135">orderHint</span><span class="sxs-lookup"><span data-stu-id="662d4-135">orderHint</span></span>|<span data-ttu-id="662d4-136">String</span><span class="sxs-lookup"><span data-stu-id="662d4-136">String</span></span>|<span data-ttu-id="662d4-137">Значение подсказки для упорядочивания задачи на представление о ходе выполнения задач платы.</span><span class="sxs-lookup"><span data-stu-id="662d4-137">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="662d4-138">Формат определяется в [с помощью подсказки порядке в планировщике](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="662d4-138">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="662d4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="662d4-139">Response</span></span>

<span data-ttu-id="662d4-140">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="662d4-140">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="662d4-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="662d4-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="662d4-144">Пример</span><span class="sxs-lookup"><span data-stu-id="662d4-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="662d4-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="662d4-145">Request</span></span>
<span data-ttu-id="662d4-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="662d4-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/<id>/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="662d4-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="662d4-147">Response</span></span>
<span data-ttu-id="662d4-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="662d4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Обновление объекта chartaxistitle
description: Обновление свойств объекта chartaxistitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fd6b38b2ff7b0c65ed58b97326c9bb1e63d34079
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966372"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="3f909-103">Обновление объекта chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="3f909-103">Update chartaxistitle</span></span>

> <span data-ttu-id="3f909-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3f909-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f909-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f909-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3f909-106">Обновление свойств объекта chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="3f909-106">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3f909-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f909-107">Permissions</span></span>
<span data-ttu-id="3f909-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f909-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f909-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f909-110">Permission type</span></span>      | <span data-ttu-id="3f909-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f909-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f909-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f909-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3f909-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f909-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3f909-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f909-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f909-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f909-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3f909-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f909-116">Application</span></span> | <span data-ttu-id="3f909-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f909-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f909-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f909-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="3f909-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f909-119">Optional request headers</span></span>
| <span data-ttu-id="3f909-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3f909-120">Name</span></span>       | <span data-ttu-id="3f909-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3f909-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3f909-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f909-122">Authorization</span></span>  | <span data-ttu-id="3f909-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f909-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3f909-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3f909-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3f909-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3f909-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f909-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3f909-128">Request body</span></span>
<span data-ttu-id="3f909-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3f909-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3f909-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f909-132">Property</span></span>     | <span data-ttu-id="3f909-133">Тип</span><span class="sxs-lookup"><span data-stu-id="3f909-133">Type</span></span>   |<span data-ttu-id="3f909-134">Описание</span><span class="sxs-lookup"><span data-stu-id="3f909-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f909-135">text</span><span class="sxs-lookup"><span data-stu-id="3f909-135">text</span></span>|<span data-ttu-id="3f909-136">строка</span><span class="sxs-lookup"><span data-stu-id="3f909-136">string</span></span>|<span data-ttu-id="3f909-137">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="3f909-137">Represents the axis title.</span></span>|
|<span data-ttu-id="3f909-138">visible</span><span class="sxs-lookup"><span data-stu-id="3f909-138">visible</span></span>|<span data-ttu-id="3f909-139">boolean</span><span class="sxs-lookup"><span data-stu-id="3f909-139">boolean</span></span>|<span data-ttu-id="3f909-140">Логическое значение, которое определяет видимость названия оси.</span><span class="sxs-lookup"><span data-stu-id="3f909-140">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="3f909-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f909-141">Response</span></span>

<span data-ttu-id="3f909-142">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartAxisTitle](../resources/chartaxistitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f909-142">If successful, this method returns a `200 OK` response code and updated [ChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3f909-143">Пример</span><span class="sxs-lookup"><span data-stu-id="3f909-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f909-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f909-144">Request</span></span>
<span data-ttu-id="3f909-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f909-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="3f909-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f909-146">Response</span></span>
<span data-ttu-id="3f909-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3f909-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Обновление Воркбукчартаксиститле
description: Обновление свойств объекта воркбукчартаксиститле.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 11f54440ce6ec7c57024376b43e1cebbccbafaa4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327821"
---
# <a name="update-workbookchartaxistitle"></a><span data-ttu-id="24e5f-103">Обновление Воркбукчартаксиститле</span><span class="sxs-lookup"><span data-stu-id="24e5f-103">Update workbookChartAxisTitle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24e5f-104">Обновление свойств объекта Воркбукчартаксиститле.</span><span class="sxs-lookup"><span data-stu-id="24e5f-104">Update the properties of workbookChartAxisTitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="24e5f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24e5f-105">Permissions</span></span>
<span data-ttu-id="24e5f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24e5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24e5f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24e5f-108">Permission type</span></span>      | <span data-ttu-id="24e5f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24e5f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24e5f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24e5f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24e5f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24e5f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="24e5f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24e5f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24e5f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24e5f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="24e5f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24e5f-114">Application</span></span> | <span data-ttu-id="24e5f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24e5f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24e5f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24e5f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="24e5f-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24e5f-117">Optional request headers</span></span>
| <span data-ttu-id="24e5f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="24e5f-118">Name</span></span>       | <span data-ttu-id="24e5f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="24e5f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="24e5f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24e5f-120">Authorization</span></span>  | <span data-ttu-id="24e5f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24e5f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24e5f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="24e5f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="24e5f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="24e5f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24e5f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24e5f-126">Request body</span></span>
<span data-ttu-id="24e5f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="24e5f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="24e5f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="24e5f-130">Property</span></span>     | <span data-ttu-id="24e5f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="24e5f-131">Type</span></span>   |<span data-ttu-id="24e5f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="24e5f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24e5f-133">text</span><span class="sxs-lookup"><span data-stu-id="24e5f-133">text</span></span>|<span data-ttu-id="24e5f-134">string</span><span class="sxs-lookup"><span data-stu-id="24e5f-134">string</span></span>|<span data-ttu-id="24e5f-135">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="24e5f-135">Represents the axis title.</span></span>|
|<span data-ttu-id="24e5f-136">visible</span><span class="sxs-lookup"><span data-stu-id="24e5f-136">visible</span></span>|<span data-ttu-id="24e5f-137">boolean</span><span class="sxs-lookup"><span data-stu-id="24e5f-137">boolean</span></span>|<span data-ttu-id="24e5f-138">Логическое значение, которое определяет видимость названия оси.</span><span class="sxs-lookup"><span data-stu-id="24e5f-138">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="24e5f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="24e5f-139">Response</span></span>

<span data-ttu-id="24e5f-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартаксиститле](../resources/workbookchartaxistitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24e5f-140">If successful, this method returns a `200 OK` response code and updated [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24e5f-141">Пример</span><span class="sxs-lookup"><span data-stu-id="24e5f-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24e5f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="24e5f-142">Request</span></span>
<span data-ttu-id="24e5f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24e5f-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="24e5f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="24e5f-144">Response</span></span>
<span data-ttu-id="24e5f-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24e5f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

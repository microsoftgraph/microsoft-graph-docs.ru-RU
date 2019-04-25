---
title: Обновление объекта ChartTitle
description: Обновление свойств объекта charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 08feb358af9ee67dda6f7da37b10c9788b83a224
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566250"
---
# <a name="update-charttitle"></a><span data-ttu-id="4b90f-103">Обновление объекта ChartTitle</span><span class="sxs-lookup"><span data-stu-id="4b90f-103">Update charttitle</span></span>

<span data-ttu-id="4b90f-104">Обновление свойств объекта charttitle.</span><span class="sxs-lookup"><span data-stu-id="4b90f-104">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b90f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b90f-105">Permissions</span></span>
<span data-ttu-id="4b90f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b90f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b90f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b90f-108">Permission type</span></span>      | <span data-ttu-id="4b90f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b90f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b90f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b90f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b90f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b90f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b90f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b90f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b90f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b90f-113">Not supported.</span></span>    |
|<span data-ttu-id="4b90f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b90f-114">Application</span></span> | <span data-ttu-id="4b90f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b90f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b90f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b90f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="4b90f-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b90f-117">Optional request headers</span></span>
| <span data-ttu-id="4b90f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4b90f-118">Name</span></span>       | <span data-ttu-id="4b90f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4b90f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4b90f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b90f-120">Authorization</span></span>  | <span data-ttu-id="4b90f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b90f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b90f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4b90f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4b90f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4b90f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b90f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b90f-126">Request body</span></span>
<span data-ttu-id="4b90f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4b90f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4b90f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b90f-130">Property</span></span>     | <span data-ttu-id="4b90f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b90f-131">Type</span></span>   |<span data-ttu-id="4b90f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b90f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b90f-133">overlay</span><span class="sxs-lookup"><span data-stu-id="4b90f-133">overlay</span></span>|<span data-ttu-id="4b90f-134">boolean</span><span class="sxs-lookup"><span data-stu-id="4b90f-134">boolean</span></span>|<span data-ttu-id="4b90f-135">Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.</span><span class="sxs-lookup"><span data-stu-id="4b90f-135">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="4b90f-136">text</span><span class="sxs-lookup"><span data-stu-id="4b90f-136">text</span></span>|<span data-ttu-id="4b90f-137">string</span><span class="sxs-lookup"><span data-stu-id="4b90f-137">string</span></span>|<span data-ttu-id="4b90f-138">Представляет текст заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="4b90f-138">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="4b90f-139">visible</span><span class="sxs-lookup"><span data-stu-id="4b90f-139">visible</span></span>|<span data-ttu-id="4b90f-140">boolean</span><span class="sxs-lookup"><span data-stu-id="4b90f-140">boolean</span></span>|<span data-ttu-id="4b90f-141">Логическое значение, представляющее видимость объекта заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="4b90f-141">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="4b90f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b90f-142">Response</span></span>

<span data-ttu-id="4b90f-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчарттитле](../resources/charttitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b90f-143">If successful, this method returns a `200 OK` response code and updated [WorkbookChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4b90f-144">Пример</span><span class="sxs-lookup"><span data-stu-id="4b90f-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b90f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b90f-145">Request</span></span>
<span data-ttu-id="4b90f-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b90f-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="4b90f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b90f-147">Response</span></span>
<span data-ttu-id="4b90f-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b90f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

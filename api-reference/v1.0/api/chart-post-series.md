---
title: Создание объекта ChartSeries
description: С помощью этого API можно создать объект ChartSeries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 053fd380728928241c146787c03b87a5207a0b7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575438"
---
# <a name="create-chartseries"></a><span data-ttu-id="cce2d-103">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="cce2d-103">Create ChartSeries</span></span>

<span data-ttu-id="cce2d-104">С помощью этого API можно создать объект ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="cce2d-104">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="cce2d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cce2d-105">Permissions</span></span>
<span data-ttu-id="cce2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cce2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cce2d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cce2d-108">Permission type</span></span>      | <span data-ttu-id="cce2d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cce2d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cce2d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cce2d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cce2d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cce2d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cce2d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cce2d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cce2d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cce2d-113">Not supported.</span></span>    |
|<span data-ttu-id="cce2d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cce2d-114">Application</span></span> | <span data-ttu-id="cce2d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cce2d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cce2d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cce2d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="cce2d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cce2d-117">Request headers</span></span>
| <span data-ttu-id="cce2d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cce2d-118">Name</span></span>       | <span data-ttu-id="cce2d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="cce2d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cce2d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cce2d-120">Authorization</span></span>  | <span data-ttu-id="cce2d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cce2d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cce2d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cce2d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cce2d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="cce2d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cce2d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cce2d-126">Request body</span></span>
<span data-ttu-id="cce2d-127">В тексте запроса добавьте представление объекта [Воркбукчартсериес](../resources/chartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cce2d-127">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cce2d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="cce2d-128">Response</span></span>

<span data-ttu-id="cce2d-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбукчартсериес](../resources/chartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cce2d-129">If successful, this method returns `201 Created` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cce2d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cce2d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cce2d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cce2d-131">Request</span></span>
<span data-ttu-id="cce2d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cce2d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="cce2d-133">В тексте запроса добавьте представление объекта [Воркбукчартсериес](../resources/chartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cce2d-133">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cce2d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cce2d-134">Response</span></span>
<span data-ttu-id="cce2d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cce2d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Получение объекта ChartTitle
description: Получение свойств и связей объекта charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bcf3f066daa048595c2adc16f1dd19a68dcadd73
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566257"
---
# <a name="get-charttitle"></a><span data-ttu-id="da579-103">Получение объекта ChartTitle</span><span class="sxs-lookup"><span data-stu-id="da579-103">Get ChartTitle</span></span>

<span data-ttu-id="da579-104">Получение свойств и связей объекта charttitle.</span><span class="sxs-lookup"><span data-stu-id="da579-104">Retrieve the properties and relationships of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="da579-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da579-105">Permissions</span></span>
<span data-ttu-id="da579-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da579-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da579-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da579-108">Permission type</span></span>      | <span data-ttu-id="da579-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da579-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da579-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da579-110">Delegated (work or school account)</span></span> | <span data-ttu-id="da579-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da579-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="da579-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da579-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da579-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da579-113">Not supported.</span></span>    |
|<span data-ttu-id="da579-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da579-114">Application</span></span> | <span data-ttu-id="da579-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da579-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da579-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da579-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="da579-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="da579-117">Optional query parameters</span></span>
<span data-ttu-id="da579-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="da579-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da579-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da579-119">Request headers</span></span>
| <span data-ttu-id="da579-120">Имя</span><span class="sxs-lookup"><span data-stu-id="da579-120">Name</span></span>      |<span data-ttu-id="da579-121">Описание</span><span class="sxs-lookup"><span data-stu-id="da579-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="da579-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da579-122">Authorization</span></span>  | <span data-ttu-id="da579-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da579-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da579-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="da579-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="da579-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="da579-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da579-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da579-128">Request body</span></span>
<span data-ttu-id="da579-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da579-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da579-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="da579-130">Response</span></span>

<span data-ttu-id="da579-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукчарттитле](../resources/charttitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da579-131">If successful, this method returns a `200 OK` response code and [WorkbookChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da579-132">Пример</span><span class="sxs-lookup"><span data-stu-id="da579-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da579-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="da579-133">Request</span></span>
<span data-ttu-id="da579-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da579-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_charttitle"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
```
##### <a name="response"></a><span data-ttu-id="da579-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="da579-135">Response</span></span>
<span data-ttu-id="da579-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da579-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get ChartTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

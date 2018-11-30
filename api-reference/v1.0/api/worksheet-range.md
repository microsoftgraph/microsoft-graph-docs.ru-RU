---
title: 'Worksheet: Range'
description: Возвращает объект диапазона, указанный по адресу или имени.
ms.openlocfilehash: ad829b9b18919e1ec5c560f521603826a42a2912
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025912"
---
# <a name="worksheet-range"></a><span data-ttu-id="51e8d-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="51e8d-103">Worksheet: Range</span></span>

<span data-ttu-id="51e8d-104">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="51e8d-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="51e8d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51e8d-105">Permissions</span></span>
<span data-ttu-id="51e8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51e8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51e8d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51e8d-108">Permission type</span></span>      | <span data-ttu-id="51e8d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51e8d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51e8d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51e8d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="51e8d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51e8d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="51e8d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51e8d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51e8d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51e8d-113">Not supported.</span></span>    |
|<span data-ttu-id="51e8d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51e8d-114">Application</span></span> | <span data-ttu-id="51e8d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51e8d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51e8d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51e8d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="51e8d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51e8d-117">Request headers</span></span>
| <span data-ttu-id="51e8d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="51e8d-118">Name</span></span>       | <span data-ttu-id="51e8d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="51e8d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="51e8d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51e8d-120">Authorization</span></span>  | <span data-ttu-id="51e8d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51e8d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51e8d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="51e8d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="51e8d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="51e8d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="51e8d-126">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="51e8d-126">Function parameters</span></span>

| <span data-ttu-id="51e8d-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="51e8d-127">Parameter</span></span>    | <span data-ttu-id="51e8d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="51e8d-128">Type</span></span>   |<span data-ttu-id="51e8d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="51e8d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51e8d-130">address</span><span class="sxs-lookup"><span data-stu-id="51e8d-130">address</span></span>|<span data-ttu-id="51e8d-131">string</span><span class="sxs-lookup"><span data-stu-id="51e8d-131">string</span></span>|<span data-ttu-id="51e8d-p104">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="51e8d-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="51e8d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="51e8d-135">Response</span></span>

<span data-ttu-id="51e8d-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="51e8d-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51e8d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="51e8d-137">Example</span></span>
<span data-ttu-id="51e8d-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="51e8d-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="51e8d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="51e8d-139">Request</span></span>
<span data-ttu-id="51e8d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51e8d-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```

##### <a name="response"></a><span data-ttu-id="51e8d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="51e8d-141">Response</span></span>
<span data-ttu-id="51e8d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="51e8d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<span data-ttu-id="51e8d-145">Если необязательный `address` параметр не указан, эта функция возвращает диапазон всего рабочего листа.</span><span class="sxs-lookup"><span data-stu-id="51e8d-145">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="51e8d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="51e8d-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```

##### <a name="response"></a><span data-ttu-id="51e8d-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="51e8d-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
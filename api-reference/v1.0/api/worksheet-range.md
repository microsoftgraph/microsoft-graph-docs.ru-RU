---
title: 'Worksheet: Range'
description: Возвращает объект диапазона, указанный по адресу или имени.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: f057b93cbc0bd2e846330b9e5e1e49b2323bf8b2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873320"
---
# <a name="worksheet-range"></a><span data-ttu-id="ec77e-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="ec77e-103">Worksheet: Range</span></span>

<span data-ttu-id="ec77e-104">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="ec77e-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec77e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec77e-105">Permissions</span></span>
<span data-ttu-id="ec77e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec77e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec77e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec77e-108">Permission type</span></span>      | <span data-ttu-id="ec77e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec77e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec77e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec77e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec77e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec77e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec77e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec77e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec77e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec77e-113">Not supported.</span></span>    |
|<span data-ttu-id="ec77e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec77e-114">Application</span></span> | <span data-ttu-id="ec77e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec77e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec77e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec77e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="ec77e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec77e-117">Request headers</span></span>
| <span data-ttu-id="ec77e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ec77e-118">Name</span></span>       | <span data-ttu-id="ec77e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ec77e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ec77e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec77e-120">Authorization</span></span>  | <span data-ttu-id="ec77e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec77e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec77e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ec77e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ec77e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ec77e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="ec77e-126">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="ec77e-126">Function parameters</span></span>

| <span data-ttu-id="ec77e-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="ec77e-127">Parameter</span></span>    | <span data-ttu-id="ec77e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="ec77e-128">Type</span></span>   |<span data-ttu-id="ec77e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="ec77e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec77e-130">address</span><span class="sxs-lookup"><span data-stu-id="ec77e-130">address</span></span>|<span data-ttu-id="ec77e-131">string</span><span class="sxs-lookup"><span data-stu-id="ec77e-131">string</span></span>|<span data-ttu-id="ec77e-p104">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="ec77e-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="ec77e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec77e-135">Response</span></span>

<span data-ttu-id="ec77e-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ec77e-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec77e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="ec77e-137">Example</span></span>
<span data-ttu-id="ec77e-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ec77e-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ec77e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec77e-139">Request</span></span>
<span data-ttu-id="ec77e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec77e-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```

##### <a name="response"></a><span data-ttu-id="ec77e-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec77e-141">Response</span></span>
<span data-ttu-id="ec77e-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ec77e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="ec77e-145">Если необязательный `address` параметр не указан, эта функция возвращает диапазон всего рабочего листа.</span><span class="sxs-lookup"><span data-stu-id="ec77e-145">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="ec77e-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec77e-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```

##### <a name="response"></a><span data-ttu-id="ec77e-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec77e-147">Response</span></span>

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

---
title: 'Range: EntireRow'
description: Возвращает объект, представляющий всю строку диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4e07b3da46d30e3163c62b182d55d9f3fea3a9df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503690"
---
# <a name="range-entirerow"></a><span data-ttu-id="fc6ef-103">Range: EntireRow</span><span class="sxs-lookup"><span data-stu-id="fc6ef-103">Range: EntireRow</span></span>

<span data-ttu-id="fc6ef-104">Возвращает объект, представляющий всю строку диапазона.</span><span class="sxs-lookup"><span data-stu-id="fc6ef-104">Gets an object that represents the entire row of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc6ef-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc6ef-105">Permissions</span></span>
<span data-ttu-id="fc6ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc6ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc6ef-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc6ef-108">Permission type</span></span>      | <span data-ttu-id="fc6ef-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc6ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc6ef-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc6ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fc6ef-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc6ef-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc6ef-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc6ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc6ef-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc6ef-113">Not supported.</span></span>    |
|<span data-ttu-id="fc6ef-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc6ef-114">Application</span></span> | <span data-ttu-id="fc6ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc6ef-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc6ef-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc6ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/entireRow
GET /workbook/worksheets/{id|name}/range(address='<address>'/entireRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/entireRow

```
## <a name="request-headers"></a><span data-ttu-id="fc6ef-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc6ef-117">Request headers</span></span>
| <span data-ttu-id="fc6ef-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fc6ef-118">Name</span></span>       | <span data-ttu-id="fc6ef-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fc6ef-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc6ef-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc6ef-120">Authorization</span></span>  | <span data-ttu-id="fc6ef-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc6ef-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc6ef-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fc6ef-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fc6ef-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fc6ef-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc6ef-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc6ef-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="fc6ef-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc6ef-127">Response</span></span>

<span data-ttu-id="fc6ef-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fc6ef-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc6ef-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fc6ef-129">Example</span></span>
<span data-ttu-id="fc6ef-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fc6ef-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc6ef-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc6ef-131">Request</span></span>
<span data-ttu-id="fc6ef-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc6ef-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_entirerow"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/entireRow
```

##### <a name="response"></a><span data-ttu-id="fc6ef-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc6ef-133">Response</span></span>
<span data-ttu-id="fc6ef-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc6ef-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: EntireRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

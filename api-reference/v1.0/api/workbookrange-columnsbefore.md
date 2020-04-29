---
title: 'workbookRange: columnsBefore'
description: Возвращает определенное количество столбцов слева от заданного диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 10d7d5b8c88feb2e6bcc2fb90a5ea7bd97f4a1fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508760"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="a4fcd-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="a4fcd-103">workbookRange: columnsBefore</span></span>

<span data-ttu-id="a4fcd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4fcd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4fcd-105">Возвращает определенное количество столбцов слева от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="a4fcd-105">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4fcd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4fcd-106">Permissions</span></span>
<span data-ttu-id="a4fcd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4fcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4fcd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4fcd-109">Permission type</span></span>      | <span data-ttu-id="a4fcd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4fcd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4fcd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4fcd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a4fcd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4fcd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a4fcd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4fcd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4fcd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4fcd-114">Not supported.</span></span>    |
|<span data-ttu-id="a4fcd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4fcd-115">Application</span></span> | <span data-ttu-id="a4fcd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4fcd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4fcd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4fcd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="a4fcd-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a4fcd-118">Function parameters</span></span>

| <span data-ttu-id="a4fcd-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="a4fcd-119">Parameter</span></span>    | <span data-ttu-id="a4fcd-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a4fcd-120">Type</span></span>   |<span data-ttu-id="a4fcd-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a4fcd-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4fcd-122">count</span><span class="sxs-lookup"><span data-stu-id="a4fcd-122">count</span></span>|<span data-ttu-id="a4fcd-123">Int32</span><span class="sxs-lookup"><span data-stu-id="a4fcd-123">Int32</span></span>|<span data-ttu-id="a4fcd-p102">Необязательный. Количество столбцов, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="a4fcd-p102">Optional. The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="a4fcd-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4fcd-129">Request headers</span></span>
| <span data-ttu-id="a4fcd-130">Имя</span><span class="sxs-lookup"><span data-stu-id="a4fcd-130">Name</span></span>       | <span data-ttu-id="a4fcd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a4fcd-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a4fcd-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4fcd-132">Authorization</span></span>  | <span data-ttu-id="a4fcd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4fcd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a4fcd-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a4fcd-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="a4fcd-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a4fcd-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4fcd-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a4fcd-138">Request body</span></span>
<span data-ttu-id="a4fcd-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4fcd-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4fcd-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4fcd-140">Response</span></span>
<span data-ttu-id="a4fcd-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a4fcd-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4fcd-142">Пример</span><span class="sxs-lookup"><span data-stu-id="a4fcd-142">Example</span></span>
<span data-ttu-id="a4fcd-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a4fcd-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a4fcd-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4fcd-144">Request</span></span>
<span data-ttu-id="a4fcd-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4fcd-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4fcd-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4fcd-146">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsbefore",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```
# <a name="c"></a>[<span data-ttu-id="a4fcd-147">C#</span><span class="sxs-lookup"><span data-stu-id="a4fcd-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsbefore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4fcd-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4fcd-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsbefore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4fcd-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4fcd-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsbefore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4fcd-150">Java</span><span class="sxs-lookup"><span data-stu-id="a4fcd-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsbefore-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a4fcd-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4fcd-151">Response</span></span>
<span data-ttu-id="a4fcd-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4fcd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

---
title: Обновление объекта FormatProtection
description: Обновление свойств объекта FormatProtection.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: a4550b0092a53af077e7475b1cb8b0a9febb1b62
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369444"
---
# <a name="update-formatprotection"></a><span data-ttu-id="59983-103">Обновление объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="59983-103">Update formatprotection</span></span>

<span data-ttu-id="59983-104">Обновление свойств объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="59983-104">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="59983-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59983-105">Permissions</span></span>
<span data-ttu-id="59983-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59983-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59983-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59983-108">Permission type</span></span>      | <span data-ttu-id="59983-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59983-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="59983-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59983-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59983-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59983-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="59983-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59983-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59983-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59983-113">Not supported.</span></span>    | 
|<span data-ttu-id="59983-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59983-114">Application</span></span> | <span data-ttu-id="59983-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59983-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="59983-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59983-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="59983-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59983-117">Optional request headers</span></span>
| <span data-ttu-id="59983-118">Имя</span><span class="sxs-lookup"><span data-stu-id="59983-118">Name</span></span>       | <span data-ttu-id="59983-119">Описание</span><span class="sxs-lookup"><span data-stu-id="59983-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="59983-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59983-120">Authorization</span></span>  | <span data-ttu-id="59983-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59983-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="59983-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="59983-123">Request body</span></span>
<span data-ttu-id="59983-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="59983-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="59983-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="59983-127">Property</span></span>     | <span data-ttu-id="59983-128">Тип</span><span class="sxs-lookup"><span data-stu-id="59983-128">Type</span></span>   |<span data-ttu-id="59983-129">Описание</span><span class="sxs-lookup"><span data-stu-id="59983-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59983-130">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="59983-130">formulaHidden</span></span>|<span data-ttu-id="59983-131">boolean</span><span class="sxs-lookup"><span data-stu-id="59983-131">boolean</span></span>|<span data-ttu-id="59983-p104">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="59983-p104">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="59983-134">locked</span><span class="sxs-lookup"><span data-stu-id="59983-134">locked</span></span>|<span data-ttu-id="59983-135">boolean</span><span class="sxs-lookup"><span data-stu-id="59983-135">boolean</span></span>|<span data-ttu-id="59983-p105">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="59983-p105">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="59983-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="59983-138">Response</span></span>

<span data-ttu-id="59983-139">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [FormatProtection](../resources/formatprotection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59983-139">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59983-140">Пример</span><span class="sxs-lookup"><span data-stu-id="59983-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59983-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="59983-141">Request</span></span>
<span data-ttu-id="59983-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59983-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="59983-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="59983-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59983-144">C#</span><span class="sxs-lookup"><span data-stu-id="59983-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-formatprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59983-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59983-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-formatprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59983-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="59983-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-formatprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="59983-147">Java</span><span class="sxs-lookup"><span data-stu-id="59983-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-formatprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59983-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="59983-148">Response</span></span>
<span data-ttu-id="59983-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59983-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

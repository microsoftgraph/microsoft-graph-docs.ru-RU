---
title: Обновление объекта FormatProtection
description: Обновление свойств объекта FormatProtection.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 43f7b9f1c0f7e8885f871b7e760a78e866a4cf0f
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573700"
---
# <a name="update-formatprotection"></a><span data-ttu-id="586df-103">Обновление объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="586df-103">Update formatprotection</span></span>

<span data-ttu-id="586df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="586df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="586df-105">Обновление свойств объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="586df-105">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="586df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="586df-106">Permissions</span></span>
<span data-ttu-id="586df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="586df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="586df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="586df-109">Permission type</span></span>      | <span data-ttu-id="586df-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="586df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="586df-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="586df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="586df-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="586df-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="586df-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="586df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="586df-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="586df-114">Not supported.</span></span>    |
|<span data-ttu-id="586df-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="586df-115">Application</span></span> | <span data-ttu-id="586df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="586df-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="586df-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="586df-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format/protection
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/protection
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/protection
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="586df-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="586df-118">Optional request headers</span></span>
| <span data-ttu-id="586df-119">Имя</span><span class="sxs-lookup"><span data-stu-id="586df-119">Name</span></span>       | <span data-ttu-id="586df-120">Описание</span><span class="sxs-lookup"><span data-stu-id="586df-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="586df-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="586df-121">Authorization</span></span>  | <span data-ttu-id="586df-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="586df-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="586df-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="586df-124">Request body</span></span>
<span data-ttu-id="586df-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="586df-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="586df-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="586df-128">Property</span></span>     | <span data-ttu-id="586df-129">Тип</span><span class="sxs-lookup"><span data-stu-id="586df-129">Type</span></span>   |<span data-ttu-id="586df-130">Описание</span><span class="sxs-lookup"><span data-stu-id="586df-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="586df-131">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="586df-131">formulaHidden</span></span>|<span data-ttu-id="586df-132">boolean</span><span class="sxs-lookup"><span data-stu-id="586df-132">boolean</span></span>|<span data-ttu-id="586df-p104">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="586df-p104">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="586df-135">locked</span><span class="sxs-lookup"><span data-stu-id="586df-135">locked</span></span>|<span data-ttu-id="586df-136">boolean</span><span class="sxs-lookup"><span data-stu-id="586df-136">boolean</span></span>|<span data-ttu-id="586df-p105">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="586df-p105">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="586df-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="586df-139">Response</span></span>

<span data-ttu-id="586df-140">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [FormatProtection](../resources/formatprotection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="586df-140">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="586df-141">Пример</span><span class="sxs-lookup"><span data-stu-id="586df-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="586df-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="586df-142">Request</span></span>
<span data-ttu-id="586df-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="586df-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="586df-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="586df-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="586df-145">C#</span><span class="sxs-lookup"><span data-stu-id="586df-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-formatprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="586df-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="586df-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-formatprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="586df-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="586df-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-formatprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="586df-148">Java</span><span class="sxs-lookup"><span data-stu-id="586df-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-formatprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="586df-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="586df-149">Response</span></span>
<span data-ttu-id="586df-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="586df-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


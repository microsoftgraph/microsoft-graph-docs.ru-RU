---
title: Обновление объекта NamedItem
description: Обновление свойств объекта nameditem.
localization_priority: Normal
ms.openlocfilehash: 8f9f4bd9902b334e6f606e93d287d8f45d5cd787
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612097"
---
# <a name="update-nameditem"></a><span data-ttu-id="fe9bf-103">Обновление объекта NamedItem</span><span class="sxs-lookup"><span data-stu-id="fe9bf-103">Update nameditem</span></span>

<span data-ttu-id="fe9bf-104">Обновление свойств объекта nameditem.</span><span class="sxs-lookup"><span data-stu-id="fe9bf-104">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe9bf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe9bf-105">Permissions</span></span>
<span data-ttu-id="fe9bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe9bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe9bf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe9bf-108">Permission type</span></span>      | <span data-ttu-id="fe9bf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe9bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe9bf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe9bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe9bf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe9bf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fe9bf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe9bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe9bf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe9bf-113">Not supported.</span></span>    |
|<span data-ttu-id="fe9bf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe9bf-114">Application</span></span> | <span data-ttu-id="fe9bf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe9bf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe9bf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe9bf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="fe9bf-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe9bf-117">Optional request headers</span></span>
| <span data-ttu-id="fe9bf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fe9bf-118">Name</span></span>       | <span data-ttu-id="fe9bf-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fe9bf-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fe9bf-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe9bf-120">Authorization</span></span>  | <span data-ttu-id="fe9bf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe9bf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe9bf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fe9bf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fe9bf-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fe9bf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe9bf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe9bf-126">Request body</span></span>
<span data-ttu-id="fe9bf-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fe9bf-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fe9bf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe9bf-130">Property</span></span>     | <span data-ttu-id="fe9bf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fe9bf-131">Type</span></span>   |<span data-ttu-id="fe9bf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fe9bf-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe9bf-133">visible</span><span class="sxs-lookup"><span data-stu-id="fe9bf-133">visible</span></span>|<span data-ttu-id="fe9bf-134">boolean</span><span class="sxs-lookup"><span data-stu-id="fe9bf-134">boolean</span></span>|<span data-ttu-id="fe9bf-135">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="fe9bf-135">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="fe9bf-136">comment</span><span class="sxs-lookup"><span data-stu-id="fe9bf-136">comment</span></span>|   <span data-ttu-id="fe9bf-137">строка</span><span class="sxs-lookup"><span data-stu-id="fe9bf-137">string</span></span>  |<span data-ttu-id="fe9bf-138">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="fe9bf-138">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="fe9bf-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe9bf-139">Response</span></span>

<span data-ttu-id="fe9bf-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукнамедитем](../resources/nameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe9bf-140">If successful, this method returns a `200 OK` response code and updated [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe9bf-141">Пример</span><span class="sxs-lookup"><span data-stu-id="fe9bf-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe9bf-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe9bf-142">Request</span></span>
<span data-ttu-id="fe9bf-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe9bf-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="fe9bf-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe9bf-144">Response</span></span>
<span data-ttu-id="fe9bf-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe9bf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fe9bf-148">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="fe9bf-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fe9bf-149">Языках</span><span class="sxs-lookup"><span data-stu-id="fe9bf-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_nameditem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe9bf-150">Язык</span><span class="sxs-lookup"><span data-stu-id="fe9bf-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_nameditem-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/nameditem-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/nameditem-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

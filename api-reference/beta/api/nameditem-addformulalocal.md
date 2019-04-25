---
title: Add Named Item FormulaLocal
description: Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.
localization_priority: Normal
ms.openlocfilehash: 064bc4a6e8183b58242522dfe663d2585eed09b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540166"
---
# <a name="add-named-item-formulalocal"></a><span data-ttu-id="2811c-103">Add Named Item FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="2811c-103">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="2811c-104">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="2811c-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="2811c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2811c-105">Permissions</span></span>
<span data-ttu-id="2811c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2811c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2811c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2811c-108">Permission type</span></span>      | <span data-ttu-id="2811c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2811c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2811c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2811c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2811c-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="2811c-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="2811c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2811c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2811c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2811c-113">Not supported.</span></span>    |
|<span data-ttu-id="2811c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2811c-114">Application</span></span> | <span data-ttu-id="2811c-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="2811c-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2811c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2811c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="2811c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2811c-117">Request headers</span></span>
| <span data-ttu-id="2811c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2811c-118">Name</span></span>       | <span data-ttu-id="2811c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2811c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2811c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2811c-120">Authorization</span></span>  | <span data-ttu-id="2811c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2811c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2811c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2811c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2811c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2811c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2811c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2811c-126">Request body</span></span>
<span data-ttu-id="2811c-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2811c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2811c-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="2811c-128">Parameter</span></span>    | <span data-ttu-id="2811c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2811c-129">Type</span></span>   |<span data-ttu-id="2811c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2811c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2811c-131">name</span><span class="sxs-lookup"><span data-stu-id="2811c-131">name</span></span>|<span data-ttu-id="2811c-132">string</span><span class="sxs-lookup"><span data-stu-id="2811c-132">string</span></span>|<span data-ttu-id="2811c-133">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="2811c-133">The name of the named item.</span></span>|
|<span data-ttu-id="2811c-134">формула</span><span class="sxs-lookup"><span data-stu-id="2811c-134">formula</span></span>|<span data-ttu-id="2811c-135">string</span><span class="sxs-lookup"><span data-stu-id="2811c-135">string</span></span>|<span data-ttu-id="2811c-136">Формула или диапазон, на которые будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="2811c-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="2811c-137">примечание</span><span class="sxs-lookup"><span data-stu-id="2811c-137">comment</span></span>|<span data-ttu-id="2811c-138">string</span><span class="sxs-lookup"><span data-stu-id="2811c-138">string</span></span>|<span data-ttu-id="2811c-139">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="2811c-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="2811c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2811c-140">Response</span></span>

<span data-ttu-id="2811c-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [NamedItem](../resources/nameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2811c-141">If successful, this method returns `200 OK` response code and [NamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2811c-142">Пример</span><span class="sxs-lookup"><span data-stu-id="2811c-142">Example</span></span>
<span data-ttu-id="2811c-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2811c-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2811c-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2811c-144">Request</span></span>
<span data-ttu-id="2811c-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2811c-145">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```

##### <a name="response"></a><span data-ttu-id="2811c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2811c-146">Response</span></span>
<span data-ttu-id="2811c-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2811c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test7%27)",
    "comment": "Comment for the named item",
    "name": "test7",
    "scope": "Workbook",
    "type": "String",
    "value": "0",
    "visible": true
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

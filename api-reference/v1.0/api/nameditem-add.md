---
title: Add Named Item
description: Добавляет новое имя в определенную коллекцию, используя языковой стандарт пользователя для формулы.
localization_priority: Normal
ms.openlocfilehash: eab6116768523d021577bef345151c3e62681fe5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852614"
---
# <a name="add-named-item"></a><span data-ttu-id="3d5a7-103">Add Named Item</span><span class="sxs-lookup"><span data-stu-id="3d5a7-103">Add Named Item</span></span>

<span data-ttu-id="3d5a7-104">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="3d5a7-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d5a7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d5a7-105">Permissions</span></span>
<span data-ttu-id="3d5a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d5a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d5a7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d5a7-108">Permission type</span></span>      | <span data-ttu-id="3d5a7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d5a7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d5a7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d5a7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d5a7-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d5a7-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="3d5a7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d5a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d5a7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d5a7-113">Not supported.</span></span>    |
|<span data-ttu-id="3d5a7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d5a7-114">Application</span></span> | <span data-ttu-id="3d5a7-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d5a7-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d5a7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d5a7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="3d5a7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d5a7-117">Request headers</span></span>
| <span data-ttu-id="3d5a7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3d5a7-118">Name</span></span>       | <span data-ttu-id="3d5a7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3d5a7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3d5a7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d5a7-120">Authorization</span></span>  | <span data-ttu-id="3d5a7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d5a7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d5a7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3d5a7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3d5a7-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3d5a7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d5a7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3d5a7-126">Request body</span></span>
<span data-ttu-id="3d5a7-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3d5a7-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3d5a7-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="3d5a7-128">Parameter</span></span>    | <span data-ttu-id="3d5a7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3d5a7-129">Type</span></span>   |<span data-ttu-id="3d5a7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3d5a7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d5a7-131">name</span><span class="sxs-lookup"><span data-stu-id="3d5a7-131">name</span></span>|<span data-ttu-id="3d5a7-132">строка</span><span class="sxs-lookup"><span data-stu-id="3d5a7-132">string</span></span>|<span data-ttu-id="3d5a7-133">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="3d5a7-133">The name of the named item.</span></span>|
|<span data-ttu-id="3d5a7-134">ссылка</span><span class="sxs-lookup"><span data-stu-id="3d5a7-134">reference</span></span>|<span data-ttu-id="3d5a7-135">Json</span><span class="sxs-lookup"><span data-stu-id="3d5a7-135">Json</span></span>|<span data-ttu-id="3d5a7-136">Формула или диапазон, на которые будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="3d5a7-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="3d5a7-137">примечание</span><span class="sxs-lookup"><span data-stu-id="3d5a7-137">comment</span></span>|<span data-ttu-id="3d5a7-138">строка</span><span class="sxs-lookup"><span data-stu-id="3d5a7-138">string</span></span>|<span data-ttu-id="3d5a7-139">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="3d5a7-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="3d5a7-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d5a7-140">Response</span></span>

<span data-ttu-id="3d5a7-141">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [WorkbookNamedItem](../resources/nameditem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3d5a7-141">If successful, this method returns `200 OK` response code and [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="3d5a7-142">Пример</span><span class="sxs-lookup"><span data-stu-id="3d5a7-142">Example</span></span>
<span data-ttu-id="3d5a7-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3d5a7-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3d5a7-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d5a7-144">Request</span></span>
<span data-ttu-id="3d5a7-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d5a7-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```

##### <a name="response"></a><span data-ttu-id="3d5a7-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d5a7-146">Response</span></span>
<span data-ttu-id="3d5a7-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3d5a7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
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
  "suppressions": [
    "Warning: NamedItemcollection_add/value:
      Schemas type was 'Custom' which is not supported. Add a resource type to the definition of property: value"
  ],
  "tocPath": ""
}-->

---
title: Add Named Item
description: Добавляет новое имя в определенную коллекцию, используя языковой стандарт пользователя для формулы.
localization_priority: Normal
ms.openlocfilehash: 57ae84505327f2afbe2936b2671b655e76a85bd4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836703"
---
# <a name="add-named-item"></a><span data-ttu-id="74da4-103">Add Named Item</span><span class="sxs-lookup"><span data-stu-id="74da4-103">Add Named Item</span></span>

> <span data-ttu-id="74da4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74da4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74da4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74da4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74da4-106">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="74da4-106">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="74da4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74da4-107">Permissions</span></span>
<span data-ttu-id="74da4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74da4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74da4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74da4-110">Permission type</span></span>      | <span data-ttu-id="74da4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74da4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74da4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74da4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="74da4-113">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="74da4-113">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="74da4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74da4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74da4-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74da4-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74da4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74da4-116">Application</span></span> | <span data-ttu-id="74da4-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="74da4-117">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74da4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74da4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="74da4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74da4-119">Request headers</span></span>
| <span data-ttu-id="74da4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="74da4-120">Name</span></span>       | <span data-ttu-id="74da4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="74da4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="74da4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74da4-122">Authorization</span></span>  | <span data-ttu-id="74da4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74da4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74da4-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="74da4-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="74da4-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="74da4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74da4-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74da4-128">Request body</span></span>
<span data-ttu-id="74da4-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="74da4-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="74da4-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="74da4-130">Parameter</span></span>    | <span data-ttu-id="74da4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="74da4-131">Type</span></span>   |<span data-ttu-id="74da4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="74da4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74da4-133">name</span><span class="sxs-lookup"><span data-stu-id="74da4-133">name</span></span>|<span data-ttu-id="74da4-134">строка</span><span class="sxs-lookup"><span data-stu-id="74da4-134">string</span></span>|<span data-ttu-id="74da4-135">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="74da4-135">The name of the named item.</span></span>|
|<span data-ttu-id="74da4-136">ссылка</span><span class="sxs-lookup"><span data-stu-id="74da4-136">reference</span></span>|<span data-ttu-id="74da4-137">string</span><span class="sxs-lookup"><span data-stu-id="74da4-137">string</span></span>|<span data-ttu-id="74da4-138">Формула или диапазон, на которые будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="74da4-138">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="74da4-139">примечание</span><span class="sxs-lookup"><span data-stu-id="74da4-139">comment</span></span>|<span data-ttu-id="74da4-140">строка</span><span class="sxs-lookup"><span data-stu-id="74da4-140">string</span></span>|<span data-ttu-id="74da4-141">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="74da4-141">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="74da4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="74da4-142">Response</span></span>

<span data-ttu-id="74da4-143">В случае успеха этот метод возвращает код отклика `200 OK` и объект [NamedItem](../resources/nameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="74da4-143">If successful, this method returns `200 OK` response code and [NamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74da4-144">Пример</span><span class="sxs-lookup"><span data-stu-id="74da4-144">Example</span></span>
<span data-ttu-id="74da4-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="74da4-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="74da4-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="74da4-146">Request</span></span>
<span data-ttu-id="74da4-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74da4-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```

##### <a name="response"></a><span data-ttu-id="74da4-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="74da4-148">Response</span></span>
<span data-ttu-id="74da4-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="74da4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->

---
title: Add Named Item
description: Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.
localization_priority: Normal
ms.openlocfilehash: dd35f2ded1c08c5f6b99a017b89dd6b5b50026b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540242"
---
# <a name="add-named-item"></a><span data-ttu-id="2fea6-103">Add Named Item</span><span class="sxs-lookup"><span data-stu-id="2fea6-103">Add Named Item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fea6-104">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="2fea6-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fea6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2fea6-105">Permissions</span></span>
<span data-ttu-id="2fea6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fea6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fea6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2fea6-108">Permission type</span></span>      | <span data-ttu-id="2fea6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2fea6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fea6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2fea6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2fea6-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="2fea6-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="2fea6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2fea6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fea6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fea6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2fea6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2fea6-114">Application</span></span> | <span data-ttu-id="2fea6-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="2fea6-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fea6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fea6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="2fea6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2fea6-117">Request headers</span></span>
| <span data-ttu-id="2fea6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2fea6-118">Name</span></span>       | <span data-ttu-id="2fea6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2fea6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2fea6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2fea6-120">Authorization</span></span>  | <span data-ttu-id="2fea6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2fea6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2fea6-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2fea6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2fea6-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2fea6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fea6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2fea6-126">Request body</span></span>
<span data-ttu-id="2fea6-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2fea6-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2fea6-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="2fea6-128">Parameter</span></span>    | <span data-ttu-id="2fea6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2fea6-129">Type</span></span>   |<span data-ttu-id="2fea6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2fea6-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fea6-131">name</span><span class="sxs-lookup"><span data-stu-id="2fea6-131">name</span></span>|<span data-ttu-id="2fea6-132">string</span><span class="sxs-lookup"><span data-stu-id="2fea6-132">string</span></span>|<span data-ttu-id="2fea6-133">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="2fea6-133">The name of the named item.</span></span>|
|<span data-ttu-id="2fea6-134">ссылка</span><span class="sxs-lookup"><span data-stu-id="2fea6-134">reference</span></span>|<span data-ttu-id="2fea6-135">string</span><span class="sxs-lookup"><span data-stu-id="2fea6-135">string</span></span>|<span data-ttu-id="2fea6-136">Формула или диапазон, на которые будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="2fea6-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="2fea6-137">примечание</span><span class="sxs-lookup"><span data-stu-id="2fea6-137">comment</span></span>|<span data-ttu-id="2fea6-138">string</span><span class="sxs-lookup"><span data-stu-id="2fea6-138">string</span></span>|<span data-ttu-id="2fea6-139">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="2fea6-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="2fea6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fea6-140">Response</span></span>

<span data-ttu-id="2fea6-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [NamedItem](../resources/nameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2fea6-141">If successful, this method returns `200 OK` response code and [NamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fea6-142">Пример</span><span class="sxs-lookup"><span data-stu-id="2fea6-142">Example</span></span>
<span data-ttu-id="2fea6-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2fea6-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2fea6-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fea6-144">Request</span></span>
<span data-ttu-id="2fea6-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fea6-145">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2fea6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fea6-146">Response</span></span>
<span data-ttu-id="2fea6-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2fea6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/nameditem-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

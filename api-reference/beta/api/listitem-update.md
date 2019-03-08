---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Изменение записи в списке SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 84164a1acd54d7492c3c0cee9d7afe6e27c87f09
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481687"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="c59f4-102">Изменение элемента в списке</span><span class="sxs-lookup"><span data-stu-id="c59f4-102">Update an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c59f4-103">Изменение свойств ресурса **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="c59f4-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c59f4-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c59f4-104">Permissions</span></span>

<span data-ttu-id="c59f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c59f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c59f4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c59f4-107">Permission type</span></span>      | <span data-ttu-id="c59f4-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c59f4-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c59f4-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c59f4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c59f4-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c59f4-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c59f4-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c59f4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c59f4-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c59f4-112">Not supported.</span></span>    |
|<span data-ttu-id="c59f4-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c59f4-113">Application</span></span> | <span data-ttu-id="c59f4-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c59f4-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c59f4-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c59f4-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="c59f4-116">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c59f4-116">Optional request headers</span></span>

| <span data-ttu-id="c59f4-117">Имя</span><span class="sxs-lookup"><span data-stu-id="c59f4-117">Name</span></span>       | <span data-ttu-id="c59f4-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c59f4-118">Value</span></span> | <span data-ttu-id="c59f4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c59f4-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="c59f4-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="c59f4-120">_if-match_</span></span> | <span data-ttu-id="c59f4-121">etag</span><span class="sxs-lookup"><span data-stu-id="c59f4-121">etag</span></span>  | <span data-ttu-id="c59f4-122">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом eTag элемента, то будет возвращен ответ `412 Precondition Failed`, а элемент не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="c59f4-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="c59f4-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c59f4-123">Request body</span></span>

<span data-ttu-id="c59f4-124">Включите представление объекта [fieldValueSet][] в формате JSON в тело запроса, указав поля, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c59f4-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="c59f4-125">Пример</span><span class="sxs-lookup"><span data-stu-id="c59f4-125">Example</span></span>

<span data-ttu-id="c59f4-126">В примере ниже показано, как обновить поля Color (Цвет) и Quantity (Количество) элемента списка, указав новые значения.</span><span class="sxs-lookup"><span data-stu-id="c59f4-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="c59f4-127">Все остальные значения для ресурса listItem останутся без изменений.</span><span class="sxs-lookup"><span data-stu-id="c59f4-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="c59f4-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c59f4-128">Response</span></span>

<span data-ttu-id="c59f4-129">При успешном выполнении этот метод возвращает объект [fieldValueSet][] для обновленного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c59f4-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

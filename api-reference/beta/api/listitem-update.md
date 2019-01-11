---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Изменение записи в списке SharePoint
localization_priority: Normal
ms.openlocfilehash: 0b6053f997422f396825aafe058dfd5252986ca1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872480"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="0310b-102">Изменение элемента в списке</span><span class="sxs-lookup"><span data-stu-id="0310b-102">Update an item in a list</span></span>

> <span data-ttu-id="0310b-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0310b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0310b-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0310b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0310b-105">Изменение свойств ресурса **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="0310b-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="0310b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0310b-106">Permissions</span></span>

<span data-ttu-id="0310b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0310b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0310b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0310b-109">Permission type</span></span>      | <span data-ttu-id="0310b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0310b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0310b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0310b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0310b-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0310b-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0310b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0310b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0310b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0310b-114">Not supported.</span></span>    |
|<span data-ttu-id="0310b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0310b-115">Application</span></span> | <span data-ttu-id="0310b-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0310b-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0310b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0310b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="0310b-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0310b-118">Optional request headers</span></span>

| <span data-ttu-id="0310b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0310b-119">Name</span></span>       | <span data-ttu-id="0310b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0310b-120">Value</span></span> | <span data-ttu-id="0310b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0310b-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="0310b-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="0310b-122">_if-match_</span></span> | <span data-ttu-id="0310b-123">etag</span><span class="sxs-lookup"><span data-stu-id="0310b-123">etag</span></span>  | <span data-ttu-id="0310b-124">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом eTag элемента, то будет возвращен ответ `412 Precondition Failed`, а элемент не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="0310b-124">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="0310b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0310b-125">Request body</span></span>

<span data-ttu-id="0310b-126">Включите представление объекта [fieldValueSet][] в формате JSON в тело запроса, указав поля, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0310b-126">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="0310b-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0310b-127">Example</span></span>

<span data-ttu-id="0310b-128">В примере ниже показано, как обновить поля Color (Цвет) и Quantity (Количество) элемента списка, указав новые значения.</span><span class="sxs-lookup"><span data-stu-id="0310b-128">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="0310b-129">Все остальные значения для ресурса listItem останутся без изменений.</span><span class="sxs-lookup"><span data-stu-id="0310b-129">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="0310b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0310b-130">Response</span></span>

<span data-ttu-id="0310b-131">При успешном выполнении этот метод возвращает объект [fieldValueSet][] для обновленного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0310b-131">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update"
} -->

---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Изменение записи в списке SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 393d8031f5dafd61e6b41d584aad988fa610b7b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966638"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="33073-102">Изменение элемента в списке</span><span class="sxs-lookup"><span data-stu-id="33073-102">Update an item in a list</span></span>

> <span data-ttu-id="33073-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="33073-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33073-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33073-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33073-105">Изменение свойств ресурса **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="33073-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="33073-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33073-106">Permissions</span></span>

<span data-ttu-id="33073-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33073-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33073-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33073-109">Permission type</span></span>      | <span data-ttu-id="33073-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33073-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33073-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33073-111">Delegated (work or school account)</span></span> | <span data-ttu-id="33073-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33073-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="33073-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33073-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33073-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33073-114">Not supported.</span></span>    |
|<span data-ttu-id="33073-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33073-115">Application</span></span> | <span data-ttu-id="33073-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33073-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33073-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33073-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="33073-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33073-118">Optional request headers</span></span>

| <span data-ttu-id="33073-119">Имя</span><span class="sxs-lookup"><span data-stu-id="33073-119">Name</span></span>       | <span data-ttu-id="33073-120">Значение</span><span class="sxs-lookup"><span data-stu-id="33073-120">Value</span></span> | <span data-ttu-id="33073-121">Описание</span><span class="sxs-lookup"><span data-stu-id="33073-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="33073-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="33073-122">_if-match_</span></span> | <span data-ttu-id="33073-123">etag</span><span class="sxs-lookup"><span data-stu-id="33073-123">etag</span></span>  | <span data-ttu-id="33073-124">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом eTag элемента, то будет возвращен ответ `412 Precondition Failed`, а элемент не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="33073-124">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="33073-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33073-125">Request body</span></span>

<span data-ttu-id="33073-126">Включите представление объекта [fieldValueSet][] в формате JSON в тело запроса, указав поля, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="33073-126">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="33073-127">Пример</span><span class="sxs-lookup"><span data-stu-id="33073-127">Example</span></span>

<span data-ttu-id="33073-128">В примере ниже показано, как обновить поля Color (Цвет) и Quantity (Количество) элемента списка, указав новые значения.</span><span class="sxs-lookup"><span data-stu-id="33073-128">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="33073-129">Все остальные значения для ресурса listItem останутся без изменений.</span><span class="sxs-lookup"><span data-stu-id="33073-129">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="33073-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="33073-130">Response</span></span>

<span data-ttu-id="33073-131">При успешном выполнении этот метод возвращает объект [fieldValueSet][] для обновленного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="33073-131">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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

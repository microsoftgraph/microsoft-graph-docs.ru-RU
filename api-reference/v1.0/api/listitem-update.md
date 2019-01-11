---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Изменение записи в списке SharePoint
localization_priority: Priority
ms.openlocfilehash: e96bcc25af715b644a1e3670514c85f8f6fd0e8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805447"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="2c13a-102">Изменение элемента в списке</span><span class="sxs-lookup"><span data-stu-id="2c13a-102">Update an item in a list</span></span>

<span data-ttu-id="2c13a-103">Изменение свойств ресурса **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="2c13a-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c13a-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c13a-104">Permissions</span></span>

<span data-ttu-id="2c13a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c13a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c13a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c13a-107">Permission type</span></span>      | <span data-ttu-id="2c13a-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c13a-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c13a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c13a-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2c13a-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c13a-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c13a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c13a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c13a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c13a-112">Not supported.</span></span>    |
|<span data-ttu-id="2c13a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c13a-113">Application</span></span> | <span data-ttu-id="2c13a-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c13a-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c13a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c13a-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="2c13a-116">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c13a-116">Optional request headers</span></span>

| <span data-ttu-id="2c13a-117">Имя</span><span class="sxs-lookup"><span data-stu-id="2c13a-117">Name</span></span>       | <span data-ttu-id="2c13a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2c13a-118">Value</span></span> | <span data-ttu-id="2c13a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2c13a-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="2c13a-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="2c13a-120">_if-match_</span></span> | <span data-ttu-id="2c13a-121">etag</span><span class="sxs-lookup"><span data-stu-id="2c13a-121">etag</span></span>  | <span data-ttu-id="2c13a-122">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом eTag элемента, то будет возвращен ответ `412 Precondition Failed`, а элемент не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="2c13a-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="2c13a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c13a-123">Request body</span></span>

<span data-ttu-id="2c13a-124">Включите представление объекта [fieldValueSet][] в формате JSON в тело запроса, указав поля, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="2c13a-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="2c13a-125">Пример</span><span class="sxs-lookup"><span data-stu-id="2c13a-125">Example</span></span>

<span data-ttu-id="2c13a-126">В примере ниже показано, как обновить поля Color (Цвет) и Quantity (Количество) элемента списка, указав новые значения.</span><span class="sxs-lookup"><span data-stu-id="2c13a-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="2c13a-127">Все остальные значения для ресурса listItem останутся без изменений.</span><span class="sxs-lookup"><span data-stu-id="2c13a-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="2c13a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c13a-128">Response</span></span>

<span data-ttu-id="2c13a-129">При успешном выполнении этот метод возвращает объект [fieldValueSet][] для обновленного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2c13a-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.fieldValueSet", "truncated": true } -->

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

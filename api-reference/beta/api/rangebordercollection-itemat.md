---
title: 'RangeBorderCollection: ItemAt'
description: Возвращает объект границы, указанный по индексу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: aed32a6381f298d86f9fe34d833d71e401b736a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919801"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="2c25c-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="2c25c-103">RangeBorderCollection: ItemAt</span></span>

> <span data-ttu-id="2c25c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2c25c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c25c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c25c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2c25c-106">Возвращает объект границы, указанный по индексу.</span><span class="sxs-lookup"><span data-stu-id="2c25c-106">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="2c25c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c25c-107">Permissions</span></span>
<span data-ttu-id="2c25c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c25c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c25c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c25c-110">Permission type</span></span>      | <span data-ttu-id="2c25c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c25c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c25c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c25c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2c25c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c25c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2c25c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c25c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c25c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c25c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2c25c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c25c-116">Application</span></span> | <span data-ttu-id="2c25c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c25c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c25c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c25c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders/ItemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/ItemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="2c25c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c25c-119">Request headers</span></span>
| <span data-ttu-id="2c25c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2c25c-120">Name</span></span>       | <span data-ttu-id="2c25c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2c25c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2c25c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c25c-122">Authorization</span></span>  | <span data-ttu-id="2c25c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c25c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2c25c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2c25c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2c25c-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2c25c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c25c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c25c-128">Request body</span></span>
<span data-ttu-id="2c25c-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2c25c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2c25c-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="2c25c-130">Parameter</span></span>    | <span data-ttu-id="2c25c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2c25c-131">Type</span></span>   |<span data-ttu-id="2c25c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2c25c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c25c-133">index</span><span class="sxs-lookup"><span data-stu-id="2c25c-133">index</span></span>|<span data-ttu-id="2c25c-134">число</span><span class="sxs-lookup"><span data-stu-id="2c25c-134">number</span></span>|<span data-ttu-id="2c25c-p105">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="2c25c-p105">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="2c25c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c25c-137">Response</span></span>

<span data-ttu-id="2c25c-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [RangeBorder](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c25c-138">If successful, this method returns `200 OK` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c25c-139">Пример</span><span class="sxs-lookup"><span data-stu-id="2c25c-139">Example</span></span>
<span data-ttu-id="2c25c-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2c25c-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2c25c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c25c-141">Request</span></span>
<span data-ttu-id="2c25c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c25c-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="2c25c-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c25c-143">Response</span></span>
<span data-ttu-id="2c25c-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2c25c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

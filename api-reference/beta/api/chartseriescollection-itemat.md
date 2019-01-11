---
title: 'ChartSeriesCollection: ItemAt'
description: Возвращает ряд на основании сведений о его позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 31a5f3608bdbad379584dec26b6551009fd7fa6c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813925"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="06dce-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="06dce-103">ChartSeriesCollection: ItemAt</span></span>

> <span data-ttu-id="06dce-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06dce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06dce-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06dce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06dce-106">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="06dce-106">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="06dce-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06dce-107">Permissions</span></span>
<span data-ttu-id="06dce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06dce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06dce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06dce-110">Permission type</span></span>      | <span data-ttu-id="06dce-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06dce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06dce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06dce-112">Delegated (work or school account)</span></span> | <span data-ttu-id="06dce-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06dce-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="06dce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06dce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06dce-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06dce-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="06dce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06dce-116">Application</span></span> | <span data-ttu-id="06dce-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06dce-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06dce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06dce-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="06dce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06dce-119">Request headers</span></span>
| <span data-ttu-id="06dce-120">Имя</span><span class="sxs-lookup"><span data-stu-id="06dce-120">Name</span></span>       | <span data-ttu-id="06dce-121">Описание</span><span class="sxs-lookup"><span data-stu-id="06dce-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="06dce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06dce-122">Authorization</span></span>  | <span data-ttu-id="06dce-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06dce-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="06dce-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="06dce-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="06dce-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="06dce-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="06dce-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="06dce-128">Request body</span></span>
<span data-ttu-id="06dce-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="06dce-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="06dce-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="06dce-130">Parameter</span></span>    | <span data-ttu-id="06dce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="06dce-131">Type</span></span>   |<span data-ttu-id="06dce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="06dce-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06dce-133">index</span><span class="sxs-lookup"><span data-stu-id="06dce-133">index</span></span>|<span data-ttu-id="06dce-134">число</span><span class="sxs-lookup"><span data-stu-id="06dce-134">number</span></span>|<span data-ttu-id="06dce-p105">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="06dce-p105">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="06dce-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="06dce-137">Response</span></span>

<span data-ttu-id="06dce-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [ChartSeries](../resources/chartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06dce-138">If successful, this method returns `200 OK` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06dce-139">Пример</span><span class="sxs-lookup"><span data-stu-id="06dce-139">Example</span></span>
<span data-ttu-id="06dce-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="06dce-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="06dce-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="06dce-141">Request</span></span>
<span data-ttu-id="06dce-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06dce-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="06dce-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="06dce-143">Response</span></span>
<span data-ttu-id="06dce-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="06dce-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

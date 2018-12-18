---
title: 'ChartPointsCollection: ItemAt'
description: Получение точки на основании сведений о ее позиции в ряду.
author: lumine2008
ms.openlocfilehash: f48a51e8da2c3dca76952460da61b492ea1235ee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311587"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="ebfc3-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="ebfc3-103">ChartPointsCollection: ItemAt</span></span>

> <span data-ttu-id="ebfc3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ebfc3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebfc3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebfc3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebfc3-106">Получение точки на основании сведений о ее позиции в ряду.</span><span class="sxs-lookup"><span data-stu-id="ebfc3-106">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebfc3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebfc3-107">Permissions</span></span>
<span data-ttu-id="ebfc3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebfc3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebfc3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebfc3-110">Permission type</span></span>      | <span data-ttu-id="ebfc3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebfc3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebfc3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebfc3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ebfc3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebfc3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ebfc3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebfc3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebfc3-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebfc3-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ebfc3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebfc3-116">Application</span></span> | <span data-ttu-id="ebfc3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebfc3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebfc3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebfc3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="ebfc3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebfc3-119">Request headers</span></span>
| <span data-ttu-id="ebfc3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ebfc3-120">Name</span></span>       | <span data-ttu-id="ebfc3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ebfc3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ebfc3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebfc3-122">Authorization</span></span>  | <span data-ttu-id="ebfc3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebfc3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebfc3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ebfc3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ebfc3-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ebfc3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebfc3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebfc3-128">Request body</span></span>
<span data-ttu-id="ebfc3-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ebfc3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ebfc3-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="ebfc3-130">Parameter</span></span>    | <span data-ttu-id="ebfc3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ebfc3-131">Type</span></span>   |<span data-ttu-id="ebfc3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ebfc3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebfc3-133">index</span><span class="sxs-lookup"><span data-stu-id="ebfc3-133">index</span></span>|<span data-ttu-id="ebfc3-134">number</span><span class="sxs-lookup"><span data-stu-id="ebfc3-134">number</span></span>|<span data-ttu-id="ebfc3-p105">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="ebfc3-p105">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="ebfc3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebfc3-137">Response</span></span>

<span data-ttu-id="ebfc3-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [ChartPoint](../resources/chartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ebfc3-138">If successful, this method returns `200 OK` response code and [ChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebfc3-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ebfc3-139">Example</span></span>
<span data-ttu-id="ebfc3-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ebfc3-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ebfc3-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebfc3-141">Request</span></span>
<span data-ttu-id="ebfc3-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebfc3-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="ebfc3-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="ebfc3-143">Response</span></span>
<span data-ttu-id="ebfc3-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ebfc3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 20

{
  "value": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
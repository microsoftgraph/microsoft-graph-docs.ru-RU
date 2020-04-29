---
title: Обновление значка
description: Обновление свойств объекта значка.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d8cd6839991e16c5b8517d8ce3630fe81862cd1b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516789"
---
# <a name="update-icon"></a><span data-ttu-id="9a641-103">Обновление значка</span><span class="sxs-lookup"><span data-stu-id="9a641-103">Update icon</span></span>

<span data-ttu-id="9a641-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a641-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a641-105">Обновление свойств объекта значка.</span><span class="sxs-lookup"><span data-stu-id="9a641-105">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a641-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a641-106">Permissions</span></span>
<span data-ttu-id="9a641-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a641-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a641-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a641-109">Permission type</span></span>      | <span data-ttu-id="9a641-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a641-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="9a641-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a641-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a641-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a641-112">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="9a641-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a641-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a641-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a641-114">Not supported.</span></span>    | 
|<span data-ttu-id="9a641-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a641-115">Application</span></span> | <span data-ttu-id="9a641-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a641-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9a641-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a641-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="9a641-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a641-118">Optional request headers</span></span>
| <span data-ttu-id="9a641-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9a641-119">Name</span></span>       | <span data-ttu-id="9a641-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9a641-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9a641-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a641-121">Authorization</span></span>  | <span data-ttu-id="9a641-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a641-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9a641-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a641-124">Request body</span></span>
<span data-ttu-id="9a641-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9a641-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9a641-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a641-128">Property</span></span>     | <span data-ttu-id="9a641-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9a641-129">Type</span></span>   |<span data-ttu-id="9a641-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9a641-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a641-131">index</span><span class="sxs-lookup"><span data-stu-id="9a641-131">index</span></span>|<span data-ttu-id="9a641-132">int</span><span class="sxs-lookup"><span data-stu-id="9a641-132">int</span></span>|<span data-ttu-id="9a641-133">Представляет собой индекс значка данного набора.</span><span class="sxs-lookup"><span data-stu-id="9a641-133">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="9a641-134">set</span><span class="sxs-lookup"><span data-stu-id="9a641-134">set</span></span>|<span data-ttu-id="9a641-135">string</span><span class="sxs-lookup"><span data-stu-id="9a641-135">string</span></span>|<span data-ttu-id="9a641-136">Представляет набор, в который входит значок.</span><span class="sxs-lookup"><span data-stu-id="9a641-136">Represents the set that the icon is part of.</span></span> <span data-ttu-id="9a641-137">Возможные значения `Invalid`:, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags` `ThreeTrafficLights1` `ThreeTrafficLights2` `ThreeSigns`,,,, `ThreeSymbols`, `ThreeSymbols2` `FourArrows` `FourArrowsGray` `FourRedToBlack`,,,,,, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`,,,,,.</span><span class="sxs-lookup"><span data-stu-id="9a641-137">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="9a641-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a641-138">Response</span></span>

<span data-ttu-id="9a641-139">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Icon](../resources/icon.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a641-139">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a641-140">Пример</span><span class="sxs-lookup"><span data-stu-id="9a641-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a641-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a641-141">Request</span></span>
<span data-ttu-id="9a641-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a641-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="9a641-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a641-143">Response</span></span>
<span data-ttu-id="9a641-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a641-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Обновление значка
description: Обновление свойств объекта значка.
localization_priority: Normal
ms.openlocfilehash: fec104af279586fe1d532361ba7b016ed3a64bf3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323932"
---
# <a name="update-icon"></a><span data-ttu-id="eeeeb-103">Обновление значка</span><span class="sxs-lookup"><span data-stu-id="eeeeb-103">Update icon</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eeeeb-104">Обновление свойств объекта значка.</span><span class="sxs-lookup"><span data-stu-id="eeeeb-104">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="eeeeb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eeeeb-105">Permissions</span></span>
<span data-ttu-id="eeeeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeeeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeeeb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eeeeb-108">Permission type</span></span>      | <span data-ttu-id="eeeeb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eeeeb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eeeeb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eeeeb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eeeeb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeeeb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eeeeb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eeeeb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eeeeb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeeeb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eeeeb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eeeeb-114">Application</span></span> | <span data-ttu-id="eeeeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeeeb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eeeeb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eeeeb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="eeeeb-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eeeeb-117">Optional request headers</span></span>
| <span data-ttu-id="eeeeb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="eeeeb-118">Name</span></span>       | <span data-ttu-id="eeeeb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="eeeeb-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="eeeeb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eeeeb-120">Authorization</span></span>  | <span data-ttu-id="eeeeb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eeeeb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eeeeb-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eeeeb-123">Request body</span></span>
<span data-ttu-id="eeeeb-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="eeeeb-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eeeeb-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="eeeeb-127">Property</span></span>     | <span data-ttu-id="eeeeb-128">Тип</span><span class="sxs-lookup"><span data-stu-id="eeeeb-128">Type</span></span>   |<span data-ttu-id="eeeeb-129">Описание</span><span class="sxs-lookup"><span data-stu-id="eeeeb-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eeeeb-130">index</span><span class="sxs-lookup"><span data-stu-id="eeeeb-130">index</span></span>|<span data-ttu-id="eeeeb-131">int</span><span class="sxs-lookup"><span data-stu-id="eeeeb-131">int</span></span>|<span data-ttu-id="eeeeb-132">Представляет собой индекс значка данного набора.</span><span class="sxs-lookup"><span data-stu-id="eeeeb-132">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="eeeeb-133">set</span><span class="sxs-lookup"><span data-stu-id="eeeeb-133">set</span></span>|<span data-ttu-id="eeeeb-134">string</span><span class="sxs-lookup"><span data-stu-id="eeeeb-134">string</span></span>|<span data-ttu-id="eeeeb-p104">Представляет набор, в который входит значок. Возможные значения: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="eeeeb-p104">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="eeeeb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeeeb-137">Response</span></span>

<span data-ttu-id="eeeeb-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукикон](../resources/workbookicon.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eeeeb-138">If successful, this method returns a `200 OK` response code and updated [workbookIcon](../resources/workbookicon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eeeeb-139">Пример</span><span class="sxs-lookup"><span data-stu-id="eeeeb-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eeeeb-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="eeeeb-140">Request</span></span>
<span data-ttu-id="eeeeb-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eeeeb-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="eeeeb-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeeeb-142">Response</span></span>
<span data-ttu-id="eeeeb-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eeeeb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

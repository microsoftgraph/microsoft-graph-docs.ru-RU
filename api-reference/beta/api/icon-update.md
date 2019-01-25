---
title: Обновление значка
description: Обновление свойств объекта значка.
localization_priority: Normal
ms.openlocfilehash: 995c67a54e6394e23ef58cc3dc730473b437c6f5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529707"
---
# <a name="update-icon"></a><span data-ttu-id="f9f6c-103">Обновление значка</span><span class="sxs-lookup"><span data-stu-id="f9f6c-103">Update icon</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9f6c-104">Обновление свойств объекта значка.</span><span class="sxs-lookup"><span data-stu-id="f9f6c-104">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9f6c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9f6c-105">Permissions</span></span>
<span data-ttu-id="f9f6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9f6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9f6c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9f6c-108">Permission type</span></span>      | <span data-ttu-id="f9f6c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9f6c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9f6c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9f6c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f9f6c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9f6c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f9f6c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9f6c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9f6c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9f6c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f9f6c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9f6c-114">Application</span></span> | <span data-ttu-id="f9f6c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9f6c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9f6c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9f6c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="f9f6c-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9f6c-117">Optional request headers</span></span>
| <span data-ttu-id="f9f6c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f9f6c-118">Name</span></span>       | <span data-ttu-id="f9f6c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f9f6c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f9f6c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9f6c-120">Authorization</span></span>  | <span data-ttu-id="f9f6c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9f6c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9f6c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9f6c-123">Request body</span></span>
<span data-ttu-id="f9f6c-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f9f6c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f9f6c-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9f6c-127">Property</span></span>     | <span data-ttu-id="f9f6c-128">Тип</span><span class="sxs-lookup"><span data-stu-id="f9f6c-128">Type</span></span>   |<span data-ttu-id="f9f6c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f9f6c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9f6c-130">index</span><span class="sxs-lookup"><span data-stu-id="f9f6c-130">index</span></span>|<span data-ttu-id="f9f6c-131">int</span><span class="sxs-lookup"><span data-stu-id="f9f6c-131">int</span></span>|<span data-ttu-id="f9f6c-132">Представляет собой индекс значка данного набора.</span><span class="sxs-lookup"><span data-stu-id="f9f6c-132">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="f9f6c-133">set</span><span class="sxs-lookup"><span data-stu-id="f9f6c-133">set</span></span>|<span data-ttu-id="f9f6c-134">string</span><span class="sxs-lookup"><span data-stu-id="f9f6c-134">string</span></span>|<span data-ttu-id="f9f6c-p104">Представляет набор, в который входит значок. Возможные значения: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="f9f6c-p104">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="f9f6c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9f6c-137">Response</span></span>

<span data-ttu-id="f9f6c-138">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Icon](../resources/icon.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9f6c-138">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9f6c-139">Пример</span><span class="sxs-lookup"><span data-stu-id="f9f6c-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9f6c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9f6c-140">Request</span></span>
<span data-ttu-id="f9f6c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9f6c-141">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f9f6c-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9f6c-142">Response</span></span>
<span data-ttu-id="f9f6c-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f9f6c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.icon"
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
  "suppressions": [
    "Error: /api-reference/beta/api/icon-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

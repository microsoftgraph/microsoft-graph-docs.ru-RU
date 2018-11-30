---
title: Обновление значка
description: Обновление свойств объекта значка.
ms.openlocfilehash: 5b9d049eb4d7bf3c596392c289738538799f8386
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081451"
---
# <a name="update-icon"></a><span data-ttu-id="bdbfe-103">Обновление значка</span><span class="sxs-lookup"><span data-stu-id="bdbfe-103">Update icon</span></span>

> <span data-ttu-id="bdbfe-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bdbfe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdbfe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdbfe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bdbfe-106">Обновление свойств объекта значка.</span><span class="sxs-lookup"><span data-stu-id="bdbfe-106">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bdbfe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdbfe-107">Permissions</span></span>
<span data-ttu-id="bdbfe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdbfe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdbfe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdbfe-110">Permission type</span></span>      | <span data-ttu-id="bdbfe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdbfe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdbfe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdbfe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bdbfe-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdbfe-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bdbfe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdbfe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdbfe-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdbfe-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bdbfe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdbfe-116">Application</span></span> | <span data-ttu-id="bdbfe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdbfe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdbfe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdbfe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="bdbfe-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdbfe-119">Optional request headers</span></span>
| <span data-ttu-id="bdbfe-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bdbfe-120">Name</span></span>       | <span data-ttu-id="bdbfe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bdbfe-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bdbfe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdbfe-122">Authorization</span></span>  | <span data-ttu-id="bdbfe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdbfe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdbfe-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdbfe-125">Request body</span></span>
<span data-ttu-id="bdbfe-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="bdbfe-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bdbfe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdbfe-129">Property</span></span>     | <span data-ttu-id="bdbfe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bdbfe-130">Type</span></span>   |<span data-ttu-id="bdbfe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bdbfe-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdbfe-132">index</span><span class="sxs-lookup"><span data-stu-id="bdbfe-132">index</span></span>|<span data-ttu-id="bdbfe-133">целое</span><span class="sxs-lookup"><span data-stu-id="bdbfe-133">int</span></span>|<span data-ttu-id="bdbfe-134">Представляет собой индекс значка данного набора.</span><span class="sxs-lookup"><span data-stu-id="bdbfe-134">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="bdbfe-135">set</span><span class="sxs-lookup"><span data-stu-id="bdbfe-135">set</span></span>|<span data-ttu-id="bdbfe-136">string</span><span class="sxs-lookup"><span data-stu-id="bdbfe-136">string</span></span>|<span data-ttu-id="bdbfe-p105">Представляет набор, в который входит значок. Возможные значения: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="bdbfe-p105">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="bdbfe-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdbfe-139">Response</span></span>

<span data-ttu-id="bdbfe-140">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Icon](../resources/icon.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bdbfe-140">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bdbfe-141">Пример</span><span class="sxs-lookup"><span data-stu-id="bdbfe-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bdbfe-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdbfe-142">Request</span></span>
<span data-ttu-id="bdbfe-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdbfe-143">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="bdbfe-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdbfe-144">Response</span></span>
<span data-ttu-id="bdbfe-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="bdbfe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
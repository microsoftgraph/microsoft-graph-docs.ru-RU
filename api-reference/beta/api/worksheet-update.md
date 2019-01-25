---
title: Обновление листа
description: Обновление свойств объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bf726ce3ad9bff427b3ec78d572017f6aea162e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519586"
---
# <a name="update-worksheet"></a><span data-ttu-id="1d626-103">Обновление листа</span><span class="sxs-lookup"><span data-stu-id="1d626-103">Update worksheet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d626-104">Обновление свойств объекта листа.</span><span class="sxs-lookup"><span data-stu-id="1d626-104">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d626-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d626-105">Permissions</span></span>
<span data-ttu-id="1d626-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d626-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d626-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d626-108">Permission type</span></span>      | <span data-ttu-id="1d626-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d626-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d626-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d626-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1d626-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d626-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d626-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d626-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d626-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d626-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d626-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d626-114">Application</span></span> | <span data-ttu-id="1d626-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d626-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d626-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d626-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1d626-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d626-117">Optional request headers</span></span>
| <span data-ttu-id="1d626-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1d626-118">Name</span></span>       | <span data-ttu-id="1d626-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1d626-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1d626-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d626-120">Authorization</span></span>  | <span data-ttu-id="1d626-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d626-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d626-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1d626-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1d626-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1d626-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d626-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d626-126">Request body</span></span>
<span data-ttu-id="1d626-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1d626-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1d626-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d626-130">Property</span></span>     | <span data-ttu-id="1d626-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1d626-131">Type</span></span>   |<span data-ttu-id="1d626-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1d626-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d626-133">name</span><span class="sxs-lookup"><span data-stu-id="1d626-133">name</span></span>|<span data-ttu-id="1d626-134">строка</span><span class="sxs-lookup"><span data-stu-id="1d626-134">string</span></span>|<span data-ttu-id="1d626-135">Отображаемое имя листа.</span><span class="sxs-lookup"><span data-stu-id="1d626-135">The display name of the worksheet.</span></span>|
|<span data-ttu-id="1d626-136">position</span><span class="sxs-lookup"><span data-stu-id="1d626-136">position</span></span>|<span data-ttu-id="1d626-137">int</span><span class="sxs-lookup"><span data-stu-id="1d626-137">int</span></span>|<span data-ttu-id="1d626-138">Положение листа (начиная с нуля) в книге.</span><span class="sxs-lookup"><span data-stu-id="1d626-138">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="1d626-139">visibility</span><span class="sxs-lookup"><span data-stu-id="1d626-139">visibility</span></span>|<span data-ttu-id="1d626-140">string</span><span class="sxs-lookup"><span data-stu-id="1d626-140">string</span></span>|<span data-ttu-id="1d626-p105">Видимость листа. Возможные значения: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="1d626-p105">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="1d626-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d626-143">Response</span></span>

<span data-ttu-id="1d626-144">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Worksheet](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d626-144">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d626-145">Пример</span><span class="sxs-lookup"><span data-stu-id="1d626-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d626-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d626-146">Request</span></span>
<span data-ttu-id="1d626-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d626-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="1d626-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d626-148">Response</span></span>
<span data-ttu-id="1d626-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1d626-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

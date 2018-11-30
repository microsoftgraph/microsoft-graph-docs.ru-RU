---
title: Обновление листа
description: Обновление свойств объекта листа.
ms.openlocfilehash: 893bfb8ea9f5f6852550f072ea43421709705e2d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024457"
---
# <a name="update-worksheet"></a><span data-ttu-id="56b35-103">Обновление листа</span><span class="sxs-lookup"><span data-stu-id="56b35-103">Update worksheet</span></span>

<span data-ttu-id="56b35-104">Обновление свойств объекта листа.</span><span class="sxs-lookup"><span data-stu-id="56b35-104">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="56b35-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56b35-105">Permissions</span></span>
<span data-ttu-id="56b35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56b35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56b35-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56b35-108">Permission type</span></span>      | <span data-ttu-id="56b35-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56b35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56b35-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56b35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="56b35-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56b35-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="56b35-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56b35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56b35-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56b35-113">Not supported.</span></span>    |
|<span data-ttu-id="56b35-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56b35-114">Application</span></span> | <span data-ttu-id="56b35-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56b35-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56b35-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56b35-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="56b35-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56b35-117">Optional request headers</span></span>
| <span data-ttu-id="56b35-118">Имя</span><span class="sxs-lookup"><span data-stu-id="56b35-118">Name</span></span>       | <span data-ttu-id="56b35-119">Описание</span><span class="sxs-lookup"><span data-stu-id="56b35-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="56b35-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56b35-120">Authorization</span></span>  | <span data-ttu-id="56b35-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56b35-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56b35-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="56b35-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="56b35-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="56b35-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56b35-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56b35-126">Request body</span></span>
<span data-ttu-id="56b35-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="56b35-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="56b35-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="56b35-130">Property</span></span>     | <span data-ttu-id="56b35-131">Тип</span><span class="sxs-lookup"><span data-stu-id="56b35-131">Type</span></span>   |<span data-ttu-id="56b35-132">Описание</span><span class="sxs-lookup"><span data-stu-id="56b35-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56b35-133">name</span><span class="sxs-lookup"><span data-stu-id="56b35-133">name</span></span>|<span data-ttu-id="56b35-134">строка</span><span class="sxs-lookup"><span data-stu-id="56b35-134">string</span></span>|<span data-ttu-id="56b35-135">Отображаемое имя листа.</span><span class="sxs-lookup"><span data-stu-id="56b35-135">The display name of the worksheet.</span></span>|
|<span data-ttu-id="56b35-136">position</span><span class="sxs-lookup"><span data-stu-id="56b35-136">position</span></span>|<span data-ttu-id="56b35-137">целое</span><span class="sxs-lookup"><span data-stu-id="56b35-137">int</span></span>|<span data-ttu-id="56b35-138">Положение листа (начиная с нуля) в книге.</span><span class="sxs-lookup"><span data-stu-id="56b35-138">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="56b35-139">visibility</span><span class="sxs-lookup"><span data-stu-id="56b35-139">visibility</span></span>|<span data-ttu-id="56b35-140">string</span><span class="sxs-lookup"><span data-stu-id="56b35-140">string</span></span>|<span data-ttu-id="56b35-141">Видимость рабочего листа.</span><span class="sxs-lookup"><span data-stu-id="56b35-141">The Visibility of the worksheet.</span></span> <span data-ttu-id="56b35-142">Возможные значения: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="56b35-142">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="56b35-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="56b35-143">Response</span></span>

<span data-ttu-id="56b35-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленный объект [WorkbookWorksheet](../resources/worksheet.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="56b35-144">If successful, this method returns a `200 OK` response code and updated [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56b35-145">Пример</span><span class="sxs-lookup"><span data-stu-id="56b35-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56b35-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="56b35-146">Request</span></span>
<span data-ttu-id="56b35-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56b35-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="56b35-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="56b35-148">Response</span></span>
<span data-ttu-id="56b35-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="56b35-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
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
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
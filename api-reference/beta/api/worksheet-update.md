---
title: Обновление листа
description: Обновление свойств объекта листа.
author: lumine2008
ms.openlocfilehash: ab61b65c03ea69a77253226c5be785d0314117bc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326441"
---
# <a name="update-worksheet"></a><span data-ttu-id="ff842-103">Обновление листа</span><span class="sxs-lookup"><span data-stu-id="ff842-103">Update worksheet</span></span>

> <span data-ttu-id="ff842-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ff842-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff842-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff842-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff842-106">Обновление свойств объекта листа.</span><span class="sxs-lookup"><span data-stu-id="ff842-106">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff842-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff842-107">Permissions</span></span>
<span data-ttu-id="ff842-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff842-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff842-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff842-110">Permission type</span></span>      | <span data-ttu-id="ff842-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff842-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff842-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff842-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ff842-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff842-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ff842-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff842-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff842-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff842-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ff842-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff842-116">Application</span></span> | <span data-ttu-id="ff842-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff842-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff842-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff842-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ff842-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff842-119">Optional request headers</span></span>
| <span data-ttu-id="ff842-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ff842-120">Name</span></span>       | <span data-ttu-id="ff842-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ff842-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ff842-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff842-122">Authorization</span></span>  | <span data-ttu-id="ff842-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff842-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff842-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ff842-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ff842-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ff842-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff842-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff842-128">Request body</span></span>
<span data-ttu-id="ff842-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ff842-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ff842-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff842-132">Property</span></span>     | <span data-ttu-id="ff842-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ff842-133">Type</span></span>   |<span data-ttu-id="ff842-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ff842-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff842-135">name</span><span class="sxs-lookup"><span data-stu-id="ff842-135">name</span></span>|<span data-ttu-id="ff842-136">строка</span><span class="sxs-lookup"><span data-stu-id="ff842-136">string</span></span>|<span data-ttu-id="ff842-137">Отображаемое имя листа.</span><span class="sxs-lookup"><span data-stu-id="ff842-137">The display name of the worksheet.</span></span>|
|<span data-ttu-id="ff842-138">position</span><span class="sxs-lookup"><span data-stu-id="ff842-138">position</span></span>|<span data-ttu-id="ff842-139">целое</span><span class="sxs-lookup"><span data-stu-id="ff842-139">int</span></span>|<span data-ttu-id="ff842-140">Положение листа (начиная с нуля) в книге.</span><span class="sxs-lookup"><span data-stu-id="ff842-140">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="ff842-141">visibility</span><span class="sxs-lookup"><span data-stu-id="ff842-141">visibility</span></span>|<span data-ttu-id="ff842-142">string</span><span class="sxs-lookup"><span data-stu-id="ff842-142">string</span></span>|<span data-ttu-id="ff842-p106">Видимость листа. Возможные значения: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="ff842-p106">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="ff842-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff842-145">Response</span></span>

<span data-ttu-id="ff842-146">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Worksheet](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff842-146">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff842-147">Пример</span><span class="sxs-lookup"><span data-stu-id="ff842-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff842-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff842-148">Request</span></span>
<span data-ttu-id="ff842-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff842-149">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ff842-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff842-150">Response</span></span>
<span data-ttu-id="ff842-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ff842-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
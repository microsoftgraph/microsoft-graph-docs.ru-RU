---
title: Обновление объекта tableRow
description: Обновление свойств объекта tablerow.
author: lumine2008
ms.openlocfilehash: cdc0049db5455891f844d2955554c73f5e77bb4e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311552"
---
# <a name="update-tablerow"></a><span data-ttu-id="f277f-103">Обновление объекта tableRow</span><span class="sxs-lookup"><span data-stu-id="f277f-103">Update tablerow</span></span>

> <span data-ttu-id="f277f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f277f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f277f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f277f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f277f-106">Обновление свойств объекта tablerow.</span><span class="sxs-lookup"><span data-stu-id="f277f-106">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f277f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f277f-107">Permissions</span></span>
<span data-ttu-id="f277f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f277f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f277f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f277f-110">Permission type</span></span>      | <span data-ttu-id="f277f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f277f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f277f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f277f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f277f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f277f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f277f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f277f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f277f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f277f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f277f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f277f-116">Application</span></span> | <span data-ttu-id="f277f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f277f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f277f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f277f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows(<index>)
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="f277f-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f277f-119">Optional request headers</span></span>
| <span data-ttu-id="f277f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f277f-120">Name</span></span>       | <span data-ttu-id="f277f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f277f-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f277f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f277f-122">Authorization</span></span>  | <span data-ttu-id="f277f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f277f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f277f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f277f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f277f-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f277f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f277f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f277f-128">Request body</span></span>
<span data-ttu-id="f277f-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f277f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f277f-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="f277f-132">Property</span></span>     | <span data-ttu-id="f277f-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f277f-133">Type</span></span>   |<span data-ttu-id="f277f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f277f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f277f-135">values</span><span class="sxs-lookup"><span data-stu-id="f277f-135">values</span></span>|<span data-ttu-id="f277f-136">json</span><span class="sxs-lookup"><span data-stu-id="f277f-136">json</span></span>|<span data-ttu-id="f277f-p106">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="f277f-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="f277f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f277f-140">Response</span></span>

<span data-ttu-id="f277f-141">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [tableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f277f-141">If successful, this method returns a `200 OK` response code and updated [TableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f277f-142">Пример</span><span class="sxs-lookup"><span data-stu-id="f277f-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f277f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="f277f-143">Request</span></span>
<span data-ttu-id="f277f-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f277f-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="f277f-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="f277f-145">Response</span></span>
<span data-ttu-id="f277f-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f277f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
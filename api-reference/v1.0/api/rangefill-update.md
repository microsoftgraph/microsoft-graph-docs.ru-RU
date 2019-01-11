---
title: Обновление объекта rangeFill
description: Обновление свойств объекта rangefill.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 869f5c1624cd8ea3da859a57c386caeda1065995
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810096"
---
# <a name="update-rangefill"></a><span data-ttu-id="4f843-103">Обновление объекта rangeFill</span><span class="sxs-lookup"><span data-stu-id="4f843-103">Update rangefill</span></span>

<span data-ttu-id="4f843-104">Обновление свойств объекта rangefill.</span><span class="sxs-lookup"><span data-stu-id="4f843-104">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f843-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f843-105">Permissions</span></span>
<span data-ttu-id="4f843-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f843-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f843-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f843-108">Permission type</span></span>      | <span data-ttu-id="4f843-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f843-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f843-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f843-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4f843-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f843-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f843-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f843-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f843-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f843-113">Not supported.</span></span>    |
|<span data-ttu-id="4f843-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f843-114">Application</span></span> | <span data-ttu-id="4f843-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f843-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f843-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f843-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="4f843-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f843-117">Optional request headers</span></span>
| <span data-ttu-id="4f843-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4f843-118">Name</span></span>       | <span data-ttu-id="4f843-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4f843-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4f843-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f843-120">Authorization</span></span>  | <span data-ttu-id="4f843-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f843-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f843-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4f843-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4f843-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4f843-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f843-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f843-126">Request body</span></span>
<span data-ttu-id="4f843-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4f843-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4f843-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f843-130">Property</span></span>     | <span data-ttu-id="4f843-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4f843-131">Type</span></span>   |<span data-ttu-id="4f843-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4f843-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f843-133">color</span><span class="sxs-lookup"><span data-stu-id="4f843-133">color</span></span>|<span data-ttu-id="4f843-134">строка</span><span class="sxs-lookup"><span data-stu-id="4f843-134">string</span></span>|<span data-ttu-id="4f843-135">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="4f843-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="4f843-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f843-136">Response</span></span>

<span data-ttu-id="4f843-137">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленный объект [WorkbookRangeFill](../resources/rangefill.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4f843-137">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4f843-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4f843-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f843-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f843-139">Request</span></span>
<span data-ttu-id="4f843-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f843-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="4f843-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f843-141">Response</span></span>
<span data-ttu-id="4f843-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4f843-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

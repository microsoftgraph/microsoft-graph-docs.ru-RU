---
title: 'Worksheet: Range'
description: Возвращает объект диапазона, указанный по адресу или имени.
ms.openlocfilehash: defe05f953d5fe7cd5fafda6ae16f04bb9f91e86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079410"
---
# <a name="worksheet-range"></a><span data-ttu-id="c8e49-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="c8e49-103">Worksheet: Range</span></span>

> <span data-ttu-id="c8e49-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c8e49-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8e49-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e49-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8e49-106">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="c8e49-106">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8e49-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e49-107">Permissions</span></span>
<span data-ttu-id="c8e49-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8e49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8e49-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e49-110">Permission type</span></span>      | <span data-ttu-id="c8e49-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8e49-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8e49-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8e49-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c8e49-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8e49-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8e49-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8e49-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8e49-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8e49-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8e49-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8e49-116">Application</span></span> | <span data-ttu-id="c8e49-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e49-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8e49-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8e49-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="c8e49-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8e49-119">Request headers</span></span>
| <span data-ttu-id="c8e49-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c8e49-120">Name</span></span>       | <span data-ttu-id="c8e49-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c8e49-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c8e49-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8e49-122">Authorization</span></span>  | <span data-ttu-id="c8e49-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8e49-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8e49-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c8e49-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c8e49-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c8e49-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8e49-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8e49-128">Request body</span></span>
<span data-ttu-id="c8e49-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c8e49-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c8e49-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="c8e49-130">Parameter</span></span>    | <span data-ttu-id="c8e49-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c8e49-131">Type</span></span>   |<span data-ttu-id="c8e49-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c8e49-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8e49-133">address</span><span class="sxs-lookup"><span data-stu-id="c8e49-133">address</span></span>|<span data-ttu-id="c8e49-134">string</span><span class="sxs-lookup"><span data-stu-id="c8e49-134">string</span></span>|<span data-ttu-id="c8e49-p105">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="c8e49-p105">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="c8e49-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8e49-138">Response</span></span>

<span data-ttu-id="c8e49-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c8e49-139">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8e49-140">Пример</span><span class="sxs-lookup"><span data-stu-id="c8e49-140">Example</span></span>
<span data-ttu-id="c8e49-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c8e49-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c8e49-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8e49-142">Request</span></span>
<span data-ttu-id="c8e49-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8e49-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```

##### <a name="response"></a><span data-ttu-id="c8e49-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8e49-144">Response</span></span>
<span data-ttu-id="c8e49-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c8e49-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
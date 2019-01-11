---
title: 'Worksheet: Range'
description: Возвращает объект диапазона, указанный по адресу или имени.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 78865ab8f7e4aa7d59bb6f3c782731bae058ae80
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860671"
---
# <a name="worksheet-range"></a><span data-ttu-id="8eecd-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="8eecd-103">Worksheet: Range</span></span>

> <span data-ttu-id="8eecd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8eecd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eecd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eecd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8eecd-106">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="8eecd-106">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="8eecd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8eecd-107">Permissions</span></span>
<span data-ttu-id="8eecd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eecd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eecd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8eecd-110">Permission type</span></span>      | <span data-ttu-id="8eecd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8eecd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8eecd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8eecd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8eecd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8eecd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8eecd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8eecd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8eecd-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8eecd-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8eecd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8eecd-116">Application</span></span> | <span data-ttu-id="8eecd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eecd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8eecd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8eecd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="8eecd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8eecd-119">Request headers</span></span>
| <span data-ttu-id="8eecd-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8eecd-120">Name</span></span>       | <span data-ttu-id="8eecd-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8eecd-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8eecd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8eecd-122">Authorization</span></span>  | <span data-ttu-id="8eecd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8eecd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8eecd-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8eecd-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8eecd-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8eecd-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eecd-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8eecd-128">Request body</span></span>
<span data-ttu-id="8eecd-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8eecd-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8eecd-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="8eecd-130">Parameter</span></span>    | <span data-ttu-id="8eecd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8eecd-131">Type</span></span>   |<span data-ttu-id="8eecd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8eecd-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8eecd-133">address</span><span class="sxs-lookup"><span data-stu-id="8eecd-133">address</span></span>|<span data-ttu-id="8eecd-134">string</span><span class="sxs-lookup"><span data-stu-id="8eecd-134">string</span></span>|<span data-ttu-id="8eecd-p105">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="8eecd-p105">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="8eecd-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8eecd-138">Response</span></span>

<span data-ttu-id="8eecd-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8eecd-139">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eecd-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8eecd-140">Example</span></span>
<span data-ttu-id="8eecd-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8eecd-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8eecd-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8eecd-142">Request</span></span>
<span data-ttu-id="8eecd-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8eecd-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8eecd-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="8eecd-144">Response</span></span>
<span data-ttu-id="8eecd-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8eecd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

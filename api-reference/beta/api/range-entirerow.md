---
title: 'Range: EntireRow'
description: Возвращает объект, представляющий всю строку диапазона.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: bb79370e8c2e8f220b45ace9491929a887678840
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832216"
---
# <a name="range-entirerow"></a><span data-ttu-id="ee7f2-103">Range: EntireRow</span><span class="sxs-lookup"><span data-stu-id="ee7f2-103">Range: EntireRow</span></span>

> <span data-ttu-id="ee7f2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee7f2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ee7f2-106">Возвращает объект, представляющий всю строку диапазона.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-106">Gets an object that represents the entire row of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee7f2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee7f2-107">Permissions</span></span>
<span data-ttu-id="ee7f2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee7f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee7f2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee7f2-110">Permission type</span></span>      | <span data-ttu-id="ee7f2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee7f2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee7f2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee7f2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ee7f2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee7f2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ee7f2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee7f2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee7f2-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee7f2-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ee7f2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee7f2-116">Application</span></span> | <span data-ttu-id="ee7f2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee7f2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee7f2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/EntireRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/EntireRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/EntireRow

```
## <a name="request-headers"></a><span data-ttu-id="ee7f2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee7f2-119">Request headers</span></span>
| <span data-ttu-id="ee7f2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ee7f2-120">Name</span></span>       | <span data-ttu-id="ee7f2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ee7f2-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ee7f2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee7f2-122">Authorization</span></span>  | <span data-ttu-id="ee7f2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee7f2-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ee7f2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ee7f2-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee7f2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee7f2-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ee7f2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee7f2-129">Response</span></span>

<span data-ttu-id="ee7f2-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee7f2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ee7f2-131">Example</span></span>
<span data-ttu-id="ee7f2-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ee7f2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee7f2-133">Request</span></span>
<span data-ttu-id="ee7f2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_entirerow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/EntireRow
```

##### <a name="response"></a><span data-ttu-id="ee7f2-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee7f2-135">Response</span></span>
<span data-ttu-id="ee7f2-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: EntireRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

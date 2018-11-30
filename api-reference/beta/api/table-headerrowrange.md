---
title: 'Table: HeaderRowRange'
description: Получает объект диапазона, связанный со строкой заголовков таблицы.
ms.openlocfilehash: 2f6a21b54812e691f581a560dac4dfa89b4de010
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076411"
---
# <a name="table-headerrowrange"></a><span data-ttu-id="671d8-103">Table: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="671d8-103">Table: HeaderRowRange</span></span>

> <span data-ttu-id="671d8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="671d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="671d8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="671d8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="671d8-106">Получает объект диапазона, связанный со строкой заголовков таблицы.</span><span class="sxs-lookup"><span data-stu-id="671d8-106">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="671d8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="671d8-107">Permissions</span></span>
<span data-ttu-id="671d8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="671d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="671d8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="671d8-110">Permission type</span></span>      | <span data-ttu-id="671d8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="671d8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="671d8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="671d8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="671d8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="671d8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="671d8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="671d8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="671d8-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="671d8-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="671d8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="671d8-116">Application</span></span> | <span data-ttu-id="671d8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="671d8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="671d8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="671d8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/HeaderRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/HeaderRowRange

```
## <a name="request-headers"></a><span data-ttu-id="671d8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="671d8-119">Request headers</span></span>
| <span data-ttu-id="671d8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="671d8-120">Name</span></span>       | <span data-ttu-id="671d8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="671d8-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="671d8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="671d8-122">Authorization</span></span>  | <span data-ttu-id="671d8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="671d8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="671d8-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="671d8-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="671d8-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="671d8-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="671d8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="671d8-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="671d8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="671d8-129">Response</span></span>

<span data-ttu-id="671d8-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="671d8-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="671d8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="671d8-131">Example</span></span>
<span data-ttu-id="671d8-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="671d8-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="671d8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="671d8-133">Request</span></span>
<span data-ttu-id="671d8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="671d8-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_headerrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/HeaderRowRange
```

##### <a name="response"></a><span data-ttu-id="671d8-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="671d8-135">Response</span></span>
<span data-ttu-id="671d8-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="671d8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
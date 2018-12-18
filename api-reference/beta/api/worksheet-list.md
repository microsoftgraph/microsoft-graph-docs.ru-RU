---
title: Список WorksheetCollection
description: Получение списка объектов листов.
author: lumine2008
ms.openlocfilehash: 23688e9f1159d9864c39720b7e4f2676eec6b43a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322143"
---
# <a name="list-worksheetcollection"></a><span data-ttu-id="46aad-103">Список WorksheetCollection</span><span class="sxs-lookup"><span data-stu-id="46aad-103">List WorksheetCollection</span></span>

> <span data-ttu-id="46aad-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46aad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46aad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46aad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46aad-106">Получение списка объектов листов.</span><span class="sxs-lookup"><span data-stu-id="46aad-106">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="46aad-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46aad-107">Permissions</span></span>
<span data-ttu-id="46aad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46aad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46aad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46aad-110">Permission type</span></span>      | <span data-ttu-id="46aad-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46aad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46aad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46aad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="46aad-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46aad-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="46aad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46aad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46aad-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46aad-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="46aad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46aad-116">Application</span></span> | <span data-ttu-id="46aad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46aad-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46aad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46aad-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="46aad-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="46aad-119">Optional query parameters</span></span>
<span data-ttu-id="46aad-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="46aad-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46aad-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46aad-121">Request headers</span></span>
| <span data-ttu-id="46aad-122">Имя</span><span class="sxs-lookup"><span data-stu-id="46aad-122">Name</span></span>      |<span data-ttu-id="46aad-123">Описание</span><span class="sxs-lookup"><span data-stu-id="46aad-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46aad-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46aad-124">Authorization</span></span>  | <span data-ttu-id="46aad-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46aad-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46aad-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="46aad-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="46aad-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="46aad-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46aad-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46aad-130">Request body</span></span>
<span data-ttu-id="46aad-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46aad-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46aad-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="46aad-132">Response</span></span>

<span data-ttu-id="46aad-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Worksheet](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46aad-133">If successful, this method returns a `200 OK` response code and collection of [Worksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46aad-134">Пример</span><span class="sxs-lookup"><span data-stu-id="46aad-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46aad-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="46aad-135">Request</span></span>
<span data-ttu-id="46aad-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46aad-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheetcollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="46aad-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="46aad-137">Response</span></span>
<span data-ttu-id="46aad-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="46aad-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List WorksheetCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: Получение общих папок
description: Получение списка общих принтеров.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 5e3e58c34481022ca23507b20af71c8ff0de4388
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216968"
---
# <a name="list-shares"></a><span data-ttu-id="8b387-103">Список общих папок</span><span class="sxs-lookup"><span data-stu-id="8b387-103">List shares</span></span>

<span data-ttu-id="8b387-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b387-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b387-105">Получение списка **принтершарес**.</span><span class="sxs-lookup"><span data-stu-id="8b387-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b387-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b387-106">Permissions</span></span>
<span data-ttu-id="8b387-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b387-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8b387-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="8b387-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="8b387-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b387-110">Permission type</span></span> | <span data-ttu-id="8b387-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b387-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8b387-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b387-112">Delegated (work or school account)</span></span>| <span data-ttu-id="8b387-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="8b387-113">Users.Read.All</span></span> |
|<span data-ttu-id="8b387-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b387-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b387-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b387-115">Not Supported.</span></span>|
|<span data-ttu-id="8b387-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b387-116">Application</span></span>|<span data-ttu-id="8b387-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b387-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b387-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b387-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8b387-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8b387-119">Optional query parameters</span></span>
<span data-ttu-id="8b387-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8b387-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8b387-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8b387-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="8b387-122">Исключения</span><span class="sxs-lookup"><span data-stu-id="8b387-122">Exceptions</span></span>
<span data-ttu-id="8b387-123">Некоторые операторы не поддерживаются: `$count` , `$orderby` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="8b387-123">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b387-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b387-124">Request headers</span></span>
| <span data-ttu-id="8b387-125">Имя</span><span class="sxs-lookup"><span data-stu-id="8b387-125">Name</span></span>      |<span data-ttu-id="8b387-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8b387-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b387-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b387-127">Authorization</span></span> | <span data-ttu-id="8b387-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b387-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b387-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b387-130">Request body</span></span>
<span data-ttu-id="8b387-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b387-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8b387-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b387-132">Response</span></span>
<span data-ttu-id="8b387-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтершаре](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b387-133">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b387-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8b387-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b387-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b387-135">Request</span></span>
<span data-ttu-id="8b387-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b387-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b387-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b387-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_shares"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares
```
# <a name="c"></a>[<span data-ttu-id="8b387-138">C#</span><span class="sxs-lookup"><span data-stu-id="8b387-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shares-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b387-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b387-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shares-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b387-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b387-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shares-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8b387-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b387-141">Response</span></span>
<span data-ttu-id="8b387-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8b387-142">The following is an example of the response.</span></span>
><span data-ttu-id="8b387-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b387-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "PrinterShareName",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List shares",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

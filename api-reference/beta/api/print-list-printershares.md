---
title: Получение Принтершарес
description: Получение списка общих принтеров.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 02fc83e45a19165a23600c9c03bc94e74ff9f493
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948299"
---
# <a name="list-printershares"></a><span data-ttu-id="75f27-103">Список Принтершарес</span><span class="sxs-lookup"><span data-stu-id="75f27-103">List printerShares</span></span>

<span data-ttu-id="75f27-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75f27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75f27-105">Получение списка **принтершарес**.</span><span class="sxs-lookup"><span data-stu-id="75f27-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="75f27-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75f27-106">Permissions</span></span>
<span data-ttu-id="75f27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75f27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="75f27-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="75f27-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="75f27-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75f27-110">Permission type</span></span> | <span data-ttu-id="75f27-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75f27-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="75f27-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75f27-112">Delegated (work or school account)</span></span>| <span data-ttu-id="75f27-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="75f27-113">Users.Read.All</span></span> |
|<span data-ttu-id="75f27-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75f27-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75f27-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f27-115">Not Supported.</span></span>|
|<span data-ttu-id="75f27-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75f27-116">Application</span></span>|<span data-ttu-id="75f27-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f27-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75f27-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75f27-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printerShares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75f27-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75f27-119">Optional query parameters</span></span>
<span data-ttu-id="75f27-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="75f27-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="75f27-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="75f27-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="75f27-122">Исключения</span><span class="sxs-lookup"><span data-stu-id="75f27-122">Exceptions</span></span>

* <span data-ttu-id="75f27-123">`$count` Оператор не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f27-123">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75f27-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75f27-124">Request headers</span></span>
| <span data-ttu-id="75f27-125">Имя</span><span class="sxs-lookup"><span data-stu-id="75f27-125">Name</span></span>      |<span data-ttu-id="75f27-126">Описание</span><span class="sxs-lookup"><span data-stu-id="75f27-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="75f27-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75f27-127">Authorization</span></span> | <span data-ttu-id="75f27-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75f27-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75f27-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75f27-130">Request body</span></span>
<span data-ttu-id="75f27-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75f27-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="75f27-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="75f27-132">Response</span></span>
<span data-ttu-id="75f27-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтершаре](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75f27-133">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="75f27-134">Пример</span><span class="sxs-lookup"><span data-stu-id="75f27-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75f27-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="75f27-135">Request</span></span>
<span data-ttu-id="75f27-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75f27-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75f27-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="75f27-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershares"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printerShares
```
# <a name="c"></a>[<span data-ttu-id="75f27-138">C#</span><span class="sxs-lookup"><span data-stu-id="75f27-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershares-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75f27-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75f27-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershares-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75f27-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75f27-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershares-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="75f27-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f27-141">Response</span></span>
<span data-ttu-id="75f27-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75f27-142">The following is an example of the response.</span></span>
><span data-ttu-id="75f27-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75f27-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printerShares",
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
  "description": "List printerShares",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

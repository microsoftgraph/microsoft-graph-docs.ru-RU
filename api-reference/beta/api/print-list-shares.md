---
title: Получать акции
description: Извлечение списка акций принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 045df17f2d59f7d8f3081fb28b8a39314e9cacf1
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766506"
---
# <a name="list-shares"></a><span data-ttu-id="c3802-103">Перечисление общих ресурсов</span><span class="sxs-lookup"><span data-stu-id="c3802-103">List shares</span></span>

<span data-ttu-id="c3802-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3802-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3802-105">Извлечение списка **printerShares**.</span><span class="sxs-lookup"><span data-stu-id="c3802-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3802-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3802-106">Permissions</span></span>
<span data-ttu-id="c3802-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3802-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c3802-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c3802-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="c3802-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3802-110">Permission type</span></span> | <span data-ttu-id="c3802-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3802-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c3802-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3802-112">Delegated (work or school account)</span></span>| <span data-ttu-id="c3802-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3802-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="c3802-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3802-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3802-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3802-115">Not Supported.</span></span>|
|<span data-ttu-id="c3802-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c3802-116">Application</span></span>|<span data-ttu-id="c3802-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3802-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3802-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3802-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3802-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c3802-119">Optional query parameters</span></span>
<span data-ttu-id="c3802-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c3802-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c3802-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c3802-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="c3802-122">Чтобы увидеть список возможностей каждой доли принтера, включайте параметр необязательный `$select=capabilities` запрос.</span><span class="sxs-lookup"><span data-stu-id="c3802-122">To see a list of each printer share's capabilities, include the optional `$select=capabilities` query parameter.</span></span>

### <a name="exceptions"></a><span data-ttu-id="c3802-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="c3802-123">Exceptions</span></span>
<span data-ttu-id="c3802-124">Некоторые операторы не поддерживаются: `$count` , `$orderby` `$search` .</span><span class="sxs-lookup"><span data-stu-id="c3802-124">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3802-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3802-125">Request headers</span></span>
| <span data-ttu-id="c3802-126">Имя</span><span class="sxs-lookup"><span data-stu-id="c3802-126">Name</span></span>      |<span data-ttu-id="c3802-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c3802-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3802-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3802-128">Authorization</span></span> | <span data-ttu-id="c3802-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3802-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3802-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3802-131">Request body</span></span>
<span data-ttu-id="c3802-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3802-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c3802-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3802-133">Response</span></span>
<span data-ttu-id="c3802-134">В случае успешного использования этот метод возвращает код отклика и коллекцию объектов `200 OK` [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3802-134">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3802-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c3802-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3802-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3802-136">Request</span></span>
<span data-ttu-id="c3802-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3802-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c3802-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3802-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_shares"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares
```
# <a name="c"></a>[<span data-ttu-id="c3802-139">C#</span><span class="sxs-lookup"><span data-stu-id="c3802-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shares-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3802-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3802-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shares-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3802-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3802-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shares-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3802-142">Java</span><span class="sxs-lookup"><span data-stu-id="c3802-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shares-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c3802-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3802-143">Response</span></span>
<span data-ttu-id="c3802-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c3802-144">The following is an example of the response.</span></span>
><span data-ttu-id="c3802-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3802-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "displayName": "PrinterShareName",
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



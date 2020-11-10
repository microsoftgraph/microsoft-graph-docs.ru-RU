---
title: Получение общих папок
description: Получение списка общих принтеров.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 3b258bdf6b6bf46ca3c4798b326210cf0edbf9fb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967072"
---
# <a name="list-shares"></a><span data-ttu-id="ef000-103">Перечисление общих ресурсов</span><span class="sxs-lookup"><span data-stu-id="ef000-103">List shares</span></span>

<span data-ttu-id="ef000-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef000-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef000-105">Получение списка **принтершарес**.</span><span class="sxs-lookup"><span data-stu-id="ef000-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef000-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef000-106">Permissions</span></span>
<span data-ttu-id="ef000-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef000-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ef000-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="ef000-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="ef000-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef000-110">Permission type</span></span> | <span data-ttu-id="ef000-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef000-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ef000-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef000-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ef000-113">Принтершаре. Read. ALL, Принтершаре. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ef000-113">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="ef000-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef000-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef000-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef000-115">Not Supported.</span></span>|
|<span data-ttu-id="ef000-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ef000-116">Application</span></span>|<span data-ttu-id="ef000-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef000-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef000-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef000-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef000-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef000-119">Optional query parameters</span></span>
<span data-ttu-id="ef000-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ef000-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ef000-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ef000-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="ef000-122">Чтобы просмотреть список всех возможностей общего доступа к принтерам, включите необязательный `$select=capabilities` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="ef000-122">To see a list of each printer share's capabilities, include the optional `$select=capabilities` query parameter.</span></span>

### <a name="exceptions"></a><span data-ttu-id="ef000-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="ef000-123">Exceptions</span></span>
<span data-ttu-id="ef000-124">Некоторые операторы не поддерживаются: `$count` , `$orderby` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="ef000-124">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef000-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef000-125">Request headers</span></span>
| <span data-ttu-id="ef000-126">Имя</span><span class="sxs-lookup"><span data-stu-id="ef000-126">Name</span></span>      |<span data-ttu-id="ef000-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ef000-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ef000-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef000-128">Authorization</span></span> | <span data-ttu-id="ef000-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef000-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef000-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef000-131">Request body</span></span>
<span data-ttu-id="ef000-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef000-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ef000-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef000-133">Response</span></span>
<span data-ttu-id="ef000-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтершаре](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef000-134">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ef000-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ef000-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef000-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef000-136">Request</span></span>
<span data-ttu-id="ef000-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef000-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ef000-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef000-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_shares"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares
```
# <a name="c"></a>[<span data-ttu-id="ef000-139">C#</span><span class="sxs-lookup"><span data-stu-id="ef000-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shares-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef000-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef000-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shares-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef000-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef000-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shares-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef000-142">Java</span><span class="sxs-lookup"><span data-stu-id="ef000-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shares-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ef000-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef000-143">Response</span></span>
<span data-ttu-id="ef000-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef000-144">The following is an example of the response.</span></span>
><span data-ttu-id="ef000-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef000-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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



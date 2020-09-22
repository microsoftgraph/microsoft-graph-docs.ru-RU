---
title: Получение printerShare
description: Получение свойств и связей общего ресурса принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c34a3a0c0e425035d71108c98aed7c2aa75c3333
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035514"
---
# <a name="get-printershare"></a><span data-ttu-id="ba252-103">Получение printerShare</span><span class="sxs-lookup"><span data-stu-id="ba252-103">Get printerShare</span></span>

<span data-ttu-id="ba252-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba252-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba252-105">Получение свойств и связей общего ресурса принтера.</span><span class="sxs-lookup"><span data-stu-id="ba252-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba252-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba252-106">Permissions</span></span>
<span data-ttu-id="ba252-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba252-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ba252-109">В дополнение к следующим разрешениям пользователь или клиент приложения должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="ba252-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="ba252-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba252-110">Permission type</span></span> | <span data-ttu-id="ba252-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba252-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ba252-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba252-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ba252-113">Принтершаре. Read. ALL, Принтершаре. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ba252-113">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="ba252-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba252-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba252-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba252-115">Not Supported.</span></span>|
|<span data-ttu-id="ba252-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba252-116">Application</span></span>|<span data-ttu-id="ba252-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba252-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba252-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba252-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}
GET /print/printers/{id}/share
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba252-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ba252-119">Optional query parameters</span></span>
<span data-ttu-id="ba252-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ba252-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ba252-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ba252-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="ba252-122">Exceptions</span><span class="sxs-lookup"><span data-stu-id="ba252-122">Exceptions</span></span>
* <span data-ttu-id="ba252-123">`$count`Оператор не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba252-123">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba252-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba252-124">Request headers</span></span>
| <span data-ttu-id="ba252-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ba252-125">Name</span></span>      |<span data-ttu-id="ba252-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ba252-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba252-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba252-127">Authorization</span></span> | <span data-ttu-id="ba252-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba252-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba252-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba252-130">Request body</span></span>
<span data-ttu-id="ba252-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba252-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ba252-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba252-132">Response</span></span>
<span data-ttu-id="ba252-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтершаре](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba252-133">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ba252-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ba252-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba252-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba252-135">Request</span></span>
<span data-ttu-id="ba252-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba252-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ba252-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba252-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}
```
# <a name="c"></a>[<span data-ttu-id="ba252-138">C#</span><span class="sxs-lookup"><span data-stu-id="ba252-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba252-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba252-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba252-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba252-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ba252-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba252-141">Response</span></span>
<span data-ttu-id="ba252-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba252-142">The following is an example of the response.</span></span>
><span data-ttu-id="ba252-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba252-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "name": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



---
title: Получение Воркбукаппликатион
description: Получение свойств и связей объекта Воркбукаппликатион.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 743ebaaf60c76b5191fca1b17b70dbfdca3fcf8c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970777"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="02905-103">Получение Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="02905-103">Get workbookApplication</span></span>

<span data-ttu-id="02905-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02905-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02905-105">Получение свойств и связей объекта [воркбукаппликатион](../resources/workbookapplication.md) .</span><span class="sxs-lookup"><span data-stu-id="02905-105">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02905-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02905-106">Permissions</span></span>
<span data-ttu-id="02905-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02905-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02905-109">Permission type</span></span>      | <span data-ttu-id="02905-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02905-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02905-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02905-111">Delegated (work or school account)</span></span> | <span data-ttu-id="02905-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02905-112">Files.ReadWrite</span></span>   |
|<span data-ttu-id="02905-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02905-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02905-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02905-114">Not supported.</span></span>    |
|<span data-ttu-id="02905-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02905-115">Application</span></span> | <span data-ttu-id="02905-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02905-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02905-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02905-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```

## <a name="request-headers"></a><span data-ttu-id="02905-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02905-118">Request headers</span></span>
| <span data-ttu-id="02905-119">Имя</span><span class="sxs-lookup"><span data-stu-id="02905-119">Name</span></span>      |<span data-ttu-id="02905-120">Описание</span><span class="sxs-lookup"><span data-stu-id="02905-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02905-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02905-121">Authorization</span></span>  | <span data-ttu-id="02905-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02905-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02905-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="02905-124">Request body</span></span>
<span data-ttu-id="02905-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02905-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02905-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="02905-126">Response</span></span>

<span data-ttu-id="02905-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукаппликатион](../resources/workbookapplication.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="02905-127">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02905-128">Пример</span><span class="sxs-lookup"><span data-stu-id="02905-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="02905-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="02905-129">Request</span></span>
<span data-ttu-id="02905-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02905-130">Here is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="02905-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="02905-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/application
```
# <a name="c"></a>[<span data-ttu-id="02905-132">C#</span><span class="sxs-lookup"><span data-stu-id="02905-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02905-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02905-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02905-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02905-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02905-135">Java</span><span class="sxs-lookup"><span data-stu-id="02905-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02905-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="02905-136">Response</span></span>
<span data-ttu-id="02905-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="02905-137">Here is an example of the response.</span></span> 

> <span data-ttu-id="02905-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02905-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookApplication"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get workbookApplication",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


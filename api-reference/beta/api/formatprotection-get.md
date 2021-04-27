---
title: Получение объекта FormatProtection
description: Получение свойств и связей объекта FormatProtection.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: 40d24ef867a58c887cc649193a8b733887bbb52b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042263"
---
# <a name="get-formatprotection"></a><span data-ttu-id="78fa0-103">Получение объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="78fa0-103">Get FormatProtection</span></span>

<span data-ttu-id="78fa0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78fa0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78fa0-105">Получение свойств и связей объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="78fa0-105">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="78fa0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78fa0-106">Permissions</span></span>
<span data-ttu-id="78fa0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78fa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78fa0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78fa0-109">Permission type</span></span>      | <span data-ttu-id="78fa0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78fa0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78fa0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78fa0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="78fa0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78fa0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="78fa0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78fa0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78fa0-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78fa0-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="78fa0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78fa0-115">Application</span></span> | <span data-ttu-id="78fa0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78fa0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78fa0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78fa0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/format/protection
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/protection
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/protection
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78fa0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="78fa0-118">Optional query parameters</span></span>
<span data-ttu-id="78fa0-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="78fa0-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78fa0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78fa0-120">Request headers</span></span>
| <span data-ttu-id="78fa0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="78fa0-121">Name</span></span>      |<span data-ttu-id="78fa0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="78fa0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="78fa0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78fa0-123">Authorization</span></span>  | <span data-ttu-id="78fa0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78fa0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78fa0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78fa0-126">Request body</span></span>
<span data-ttu-id="78fa0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78fa0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78fa0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="78fa0-128">Response</span></span>

<span data-ttu-id="78fa0-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [FormatProtection](../resources/formatprotection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="78fa0-129">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78fa0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="78fa0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78fa0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="78fa0-131">Request</span></span>
<span data-ttu-id="78fa0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78fa0-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="78fa0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="78fa0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/protection
```
# <a name="c"></a>[<span data-ttu-id="78fa0-134">C#</span><span class="sxs-lookup"><span data-stu-id="78fa0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-formatprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78fa0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78fa0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-formatprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78fa0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78fa0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-formatprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78fa0-137">Java</span><span class="sxs-lookup"><span data-stu-id="78fa0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-formatprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="78fa0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="78fa0-138">Response</span></span>
<span data-ttu-id="78fa0-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="78fa0-139">Here is an example of the response.</span></span> <span data-ttu-id="78fa0-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="78fa0-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

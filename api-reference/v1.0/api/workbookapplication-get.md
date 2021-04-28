---
title: Get workbookApplication
description: Извлечение свойств и связей объекта workbookApplication.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c3b9a48ebc05964196d97860c891d180d90d7c0d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054275"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="bcb26-103">Get workbookApplication</span><span class="sxs-lookup"><span data-stu-id="bcb26-103">Get workbookApplication</span></span>

<span data-ttu-id="bcb26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcb26-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bcb26-105">Извлечение свойств и связей объекта [workbookApplication.](../resources/workbookapplication.md)</span><span class="sxs-lookup"><span data-stu-id="bcb26-105">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcb26-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcb26-106">Permissions</span></span>
<span data-ttu-id="bcb26-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcb26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcb26-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcb26-109">Permission type</span></span>      | <span data-ttu-id="bcb26-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcb26-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcb26-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcb26-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bcb26-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcb26-112">Files.ReadWrite</span></span>   |
|<span data-ttu-id="bcb26-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcb26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcb26-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcb26-114">Not supported.</span></span>    |
|<span data-ttu-id="bcb26-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcb26-115">Application</span></span> | <span data-ttu-id="bcb26-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcb26-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcb26-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcb26-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/application
GET /me/drive/root:/{item-path}:/workbook/application
```

## <a name="request-headers"></a><span data-ttu-id="bcb26-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcb26-118">Request headers</span></span>
| <span data-ttu-id="bcb26-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bcb26-119">Name</span></span>      |<span data-ttu-id="bcb26-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bcb26-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bcb26-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcb26-121">Authorization</span></span>  | <span data-ttu-id="bcb26-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcb26-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcb26-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcb26-124">Request body</span></span>
<span data-ttu-id="bcb26-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcb26-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcb26-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcb26-126">Response</span></span>

<span data-ttu-id="bcb26-127">В случае успеха этот метод возвращает код ответа и `200 OK` объект [workbookApplication](../resources/workbookapplication.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bcb26-127">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcb26-128">Пример</span><span class="sxs-lookup"><span data-stu-id="bcb26-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="bcb26-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcb26-129">Request</span></span>
<span data-ttu-id="bcb26-130">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcb26-130">Here is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bcb26-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcb26-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/application
```
# <a name="c"></a>[<span data-ttu-id="bcb26-132">C#</span><span class="sxs-lookup"><span data-stu-id="bcb26-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcb26-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcb26-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcb26-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcb26-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcb26-135">Java</span><span class="sxs-lookup"><span data-stu-id="bcb26-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bcb26-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcb26-136">Response</span></span>
<span data-ttu-id="bcb26-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bcb26-137">Here is an example of the response.</span></span> 

> <span data-ttu-id="bcb26-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bcb26-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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


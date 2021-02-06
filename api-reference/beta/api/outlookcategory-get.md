---
title: Получение категории Outlook
description: Получение свойств и отношений указанного объекта outlookCategory.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2593b2d80b6e457b81e6c1309c29eda97743c832
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133089"
---
# <a name="get-outlook-category"></a><span data-ttu-id="0ef48-103">Получение категории Outlook</span><span class="sxs-lookup"><span data-stu-id="0ef48-103">Get Outlook category</span></span>

<span data-ttu-id="0ef48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ef48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ef48-105">Получение свойств и отношений указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="0ef48-105">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ef48-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ef48-106">Permissions</span></span>
<span data-ttu-id="0ef48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ef48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ef48-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ef48-109">Permission type</span></span>      | <span data-ttu-id="0ef48-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ef48-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ef48-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ef48-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ef48-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0ef48-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="0ef48-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ef48-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ef48-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0ef48-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="0ef48-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ef48-115">Application</span></span> | <span data-ttu-id="0ef48-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0ef48-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ef48-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ef48-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ef48-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ef48-118">Optional query parameters</span></span>
<span data-ttu-id="0ef48-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0ef48-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ef48-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ef48-120">Request headers</span></span>
| <span data-ttu-id="0ef48-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0ef48-121">Name</span></span>      |<span data-ttu-id="0ef48-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0ef48-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ef48-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ef48-123">Authorization</span></span>  | <span data-ttu-id="0ef48-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ef48-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ef48-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ef48-126">Request body</span></span>
<span data-ttu-id="0ef48-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ef48-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ef48-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ef48-128">Response</span></span>

<span data-ttu-id="0ef48-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [outlookCategory](../resources/outlookcategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0ef48-129">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ef48-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0ef48-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ef48-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ef48-131">Request</span></span>
<span data-ttu-id="0ef48-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ef48-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0ef48-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ef48-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
# <a name="c"></a>[<span data-ttu-id="0ef48-134">C#</span><span class="sxs-lookup"><span data-stu-id="0ef48-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ef48-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ef48-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ef48-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ef48-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ef48-137">Java</span><span class="sxs-lookup"><span data-stu-id="0ef48-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0ef48-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ef48-138">Response</span></span>
<span data-ttu-id="0ef48-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ef48-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 249

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
  "displayName":"Yellow category",
  "color":"preset3"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

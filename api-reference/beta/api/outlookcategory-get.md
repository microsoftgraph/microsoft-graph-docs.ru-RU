---
title: Получение категории Outlook
description: Получение свойств и отношений указанного объекта outlookCategory.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 03fb374564faec3a57df62e96780019db87f5333
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450690"
---
# <a name="get-outlook-category"></a><span data-ttu-id="f043a-103">Получение категории Outlook</span><span class="sxs-lookup"><span data-stu-id="f043a-103">Get Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f043a-104">Получение свойств и отношений указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="f043a-104">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f043a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f043a-105">Permissions</span></span>
<span data-ttu-id="f043a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f043a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f043a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f043a-108">Permission type</span></span>      | <span data-ttu-id="f043a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f043a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f043a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f043a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f043a-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="f043a-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="f043a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f043a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f043a-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="f043a-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="f043a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f043a-114">Application</span></span> | <span data-ttu-id="f043a-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="f043a-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f043a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f043a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f043a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f043a-117">Optional query parameters</span></span>
<span data-ttu-id="f043a-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f043a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f043a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f043a-119">Request headers</span></span>
| <span data-ttu-id="f043a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f043a-120">Name</span></span>      |<span data-ttu-id="f043a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f043a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f043a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f043a-122">Authorization</span></span>  | <span data-ttu-id="f043a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f043a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f043a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f043a-125">Request body</span></span>
<span data-ttu-id="f043a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f043a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f043a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f043a-127">Response</span></span>

<span data-ttu-id="f043a-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [outlookCategory](../resources/outlookcategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f043a-128">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f043a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f043a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f043a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f043a-130">Request</span></span>
<span data-ttu-id="f043a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f043a-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f043a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f043a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f043a-133">C#</span><span class="sxs-lookup"><span data-stu-id="f043a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f043a-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="f043a-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f043a-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f043a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f043a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f043a-136">Response</span></span>
<span data-ttu-id="f043a-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f043a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

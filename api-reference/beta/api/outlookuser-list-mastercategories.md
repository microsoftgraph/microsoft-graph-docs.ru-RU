---
title: Перечисление категорий Outlook
description: Получение всех категорий, определенных для пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 50c3b2cc688d66dfec2a02ba4c49f12f41bf173b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447189"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="136d6-103">Перечисление категорий Outlook</span><span class="sxs-lookup"><span data-stu-id="136d6-103">List Outlook categories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="136d6-104">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="136d6-104">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="136d6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="136d6-105">Permissions</span></span>
<span data-ttu-id="136d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="136d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="136d6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="136d6-108">Permission type</span></span>      | <span data-ttu-id="136d6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="136d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="136d6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="136d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="136d6-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="136d6-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="136d6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="136d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="136d6-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="136d6-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="136d6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="136d6-114">Application</span></span> | <span data-ttu-id="136d6-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="136d6-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="136d6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="136d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="136d6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="136d6-117">Optional query parameters</span></span>
<span data-ttu-id="136d6-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="136d6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="136d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="136d6-119">Request headers</span></span>
| <span data-ttu-id="136d6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="136d6-120">Name</span></span>      |<span data-ttu-id="136d6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="136d6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="136d6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="136d6-122">Authorization</span></span>  | <span data-ttu-id="136d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="136d6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="136d6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="136d6-125">Request body</span></span>
<span data-ttu-id="136d6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="136d6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="136d6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="136d6-127">Response</span></span>

<span data-ttu-id="136d6-128">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [outlookCategory](../resources/outlookcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="136d6-128">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="136d6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="136d6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="136d6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="136d6-130">Request</span></span>
<span data-ttu-id="136d6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="136d6-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="136d6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="136d6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="136d6-133">C#</span><span class="sxs-lookup"><span data-stu-id="136d6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mastercategories-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="136d6-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="136d6-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mastercategories-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="136d6-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="136d6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mastercategories-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="136d6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="136d6-136">Response</span></span>
<span data-ttu-id="136d6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="136d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 727

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
  "value":[
    {
      "id":"5a9a6aa8-b65f-4357-b1f9-60c6bf6330d8",
      "displayName":"Red category",
      "color":"preset0"
    },
    {
      "id":"4b1c2495-54c9-4a5e-90a2-0ab0b31987d8",
      "displayName":"Orange category",
      "color":"preset1"
    },
    {
      "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
      "displayName":"Yellow category",
      "color":"preset3"
    },
    {
      "id":"79c8d8f8-9db1-49ec-99ce-ae25793e7232",
      "displayName":"Green category",
      "color":"preset4"
    },
    {
      "id":"626e696c-6a10-48b8-89b9-12de3160cfb9",
      "displayName":"Blue category",
      "color":"preset7"
    },
    {
      "id":"453d06d0-447d-41f7-91cd-aa0f6b190b5b",
      "displayName":"Purple category",
      "color":"preset8"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

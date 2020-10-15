---
title: Перечисление категорий Outlook
description: Получение всех категорий, определенных для пользователя.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5a564d036f5f3a499bde3bce92437f2a3dd70a42
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461435"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="b4dfc-103">Перечисление категорий Outlook</span><span class="sxs-lookup"><span data-stu-id="b4dfc-103">List Outlook categories</span></span>

<span data-ttu-id="b4dfc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4dfc-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="b4dfc-105">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4dfc-105">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4dfc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4dfc-106">Permissions</span></span>
<span data-ttu-id="b4dfc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4dfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4dfc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4dfc-109">Permission type</span></span>      | <span data-ttu-id="b4dfc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4dfc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4dfc-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4dfc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b4dfc-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="b4dfc-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="b4dfc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4dfc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4dfc-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="b4dfc-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="b4dfc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4dfc-115">Application</span></span> | <span data-ttu-id="b4dfc-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="b4dfc-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4dfc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4dfc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b4dfc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b4dfc-118">Optional query parameters</span></span>
<span data-ttu-id="b4dfc-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b4dfc-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4dfc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4dfc-120">Request headers</span></span>
| <span data-ttu-id="b4dfc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b4dfc-121">Name</span></span>      |<span data-ttu-id="b4dfc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b4dfc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b4dfc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4dfc-123">Authorization</span></span>  | <span data-ttu-id="b4dfc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4dfc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4dfc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4dfc-126">Request body</span></span>
<span data-ttu-id="b4dfc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4dfc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4dfc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4dfc-128">Response</span></span>

<span data-ttu-id="b4dfc-129">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [outlookCategory](../resources/outlookcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b4dfc-129">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b4dfc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b4dfc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4dfc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4dfc-131">Request</span></span>
<span data-ttu-id="b4dfc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4dfc-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b4dfc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4dfc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories
```
# <a name="c"></a>[<span data-ttu-id="b4dfc-134">C#</span><span class="sxs-lookup"><span data-stu-id="b4dfc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mastercategories-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4dfc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4dfc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mastercategories-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4dfc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4dfc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mastercategories-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4dfc-137">Java</span><span class="sxs-lookup"><span data-stu-id="b4dfc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mastercategories-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b4dfc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4dfc-138">Response</span></span>
<span data-ttu-id="b4dfc-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4dfc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
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
<!-- {
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

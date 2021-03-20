---
title: Получение соглашения
description: Извлечение свойств и связей объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 92b794270c0912f1320f8bb2b5dcf47d1f976f5e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942920"
---
# <a name="get-agreement"></a><span data-ttu-id="acd47-103">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="acd47-103">Get agreement</span></span>

<span data-ttu-id="acd47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acd47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acd47-105">Извлечение свойств и связей объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="acd47-105">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="acd47-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="acd47-106">Permissions</span></span>
<span data-ttu-id="acd47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acd47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acd47-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acd47-109">Permission type</span></span>                        | <span data-ttu-id="acd47-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="acd47-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="acd47-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acd47-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="acd47-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="acd47-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="acd47-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acd47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acd47-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acd47-114">Not supported.</span></span> |
|<span data-ttu-id="acd47-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="acd47-115">Application</span></span>                            | <span data-ttu-id="acd47-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acd47-116">Not supported.</span></span> |

<span data-ttu-id="acd47-117">При вызове от имени пользователя пользователю необходимо принадлежать к одной из следующих ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="acd47-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="acd47-118">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="acd47-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="acd47-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="acd47-119">Global Administrator</span></span>
+ <span data-ttu-id="acd47-120">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="acd47-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="acd47-121">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="acd47-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="acd47-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acd47-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements/{id}
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="acd47-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="acd47-123">Request headers</span></span>
| <span data-ttu-id="acd47-124">Имя</span><span class="sxs-lookup"><span data-stu-id="acd47-124">Name</span></span>         | <span data-ttu-id="acd47-125">Тип</span><span class="sxs-lookup"><span data-stu-id="acd47-125">Type</span></span>        | <span data-ttu-id="acd47-126">Описание</span><span class="sxs-lookup"><span data-stu-id="acd47-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="acd47-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="acd47-127">Authorization</span></span> | <span data-ttu-id="acd47-128">string</span><span class="sxs-lookup"><span data-stu-id="acd47-128">string</span></span> | <span data-ttu-id="acd47-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="acd47-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="acd47-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="acd47-131">Request body</span></span>
<span data-ttu-id="acd47-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="acd47-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="acd47-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="acd47-133">Response</span></span>
<span data-ttu-id="acd47-134">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` соглашения в тексте ответа. [](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="acd47-134">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="acd47-135">Пример</span><span class="sxs-lookup"><span data-stu-id="acd47-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="acd47-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="acd47-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="acd47-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="acd47-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}?$expand=files
```
# <a name="c"></a>[<span data-ttu-id="acd47-138">C#</span><span class="sxs-lookup"><span data-stu-id="acd47-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acd47-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acd47-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acd47-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acd47-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="acd47-141">Java</span><span class="sxs-lookup"><span data-stu-id="acd47-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="acd47-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="acd47-142">Response</span></span>
><span data-ttu-id="acd47-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="acd47-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

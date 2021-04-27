---
title: Список соглашений
description: Извлечение списка объектов соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: b356e0fb945ca7cfe5d4aebe769cbc905b85d3d6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048219"
---
# <a name="list-agreements"></a><span data-ttu-id="a2d13-103">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="a2d13-103">List agreements</span></span>

<span data-ttu-id="a2d13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2d13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2d13-105">Извлечение списка [объектов](../resources/agreement.md) соглашения.</span><span class="sxs-lookup"><span data-stu-id="a2d13-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a2d13-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2d13-106">Permissions</span></span>
<span data-ttu-id="a2d13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2d13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2d13-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2d13-109">Permission type</span></span>                        | <span data-ttu-id="a2d13-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2d13-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2d13-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2d13-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2d13-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2d13-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="a2d13-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2d13-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2d13-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2d13-114">Not supported.</span></span> |
|<span data-ttu-id="a2d13-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2d13-115">Application</span></span>                            | <span data-ttu-id="a2d13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2d13-116">Not supported.</span></span> |

<span data-ttu-id="a2d13-117">При вызове от имени пользователя пользователю необходимо принадлежать к одной из следующих ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="a2d13-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="a2d13-118">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="a2d13-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="a2d13-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a2d13-119">Global Administrator</span></span>
+ <span data-ttu-id="a2d13-120">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="a2d13-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="a2d13-121">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="a2d13-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a2d13-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2d13-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="a2d13-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2d13-123">Request headers</span></span>
| <span data-ttu-id="a2d13-124">Имя</span><span class="sxs-lookup"><span data-stu-id="a2d13-124">Name</span></span>         | <span data-ttu-id="a2d13-125">Тип</span><span class="sxs-lookup"><span data-stu-id="a2d13-125">Type</span></span>        | <span data-ttu-id="a2d13-126">Описание</span><span class="sxs-lookup"><span data-stu-id="a2d13-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a2d13-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2d13-127">Authorization</span></span> | <span data-ttu-id="a2d13-128">string</span><span class="sxs-lookup"><span data-stu-id="a2d13-128">string</span></span> | <span data-ttu-id="a2d13-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2d13-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2d13-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2d13-131">Request body</span></span>
<span data-ttu-id="a2d13-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2d13-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a2d13-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2d13-133">Response</span></span>
<span data-ttu-id="a2d13-134">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` соглашения в тексте отклика. [](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="a2d13-134">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a2d13-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a2d13-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2d13-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2d13-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a2d13-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2d13-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements
```
# <a name="c"></a>[<span data-ttu-id="a2d13-138">C#</span><span class="sxs-lookup"><span data-stu-id="a2d13-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2d13-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2d13-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2d13-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2d13-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2d13-141">Java</span><span class="sxs-lookup"><span data-stu-id="a2d13-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a2d13-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2d13-142">Response</span></span>
><span data-ttu-id="a2d13-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a2d13-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

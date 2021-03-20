---
title: Список соглашений
description: Извлечение списка объектов соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 8d636cab5663633ba78e76057dc9ba3d555fbdc4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942897"
---
# <a name="list-agreements"></a><span data-ttu-id="ab540-103">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="ab540-103">List agreements</span></span>

<span data-ttu-id="ab540-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab540-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab540-105">Извлечение списка [объектов](../resources/agreement.md) соглашения.</span><span class="sxs-lookup"><span data-stu-id="ab540-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab540-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab540-106">Permissions</span></span>
<span data-ttu-id="ab540-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab540-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab540-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab540-109">Permission type</span></span>                        | <span data-ttu-id="ab540-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab540-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab540-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab540-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab540-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab540-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="ab540-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab540-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab540-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab540-114">Not supported.</span></span> |
|<span data-ttu-id="ab540-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab540-115">Application</span></span>                            | <span data-ttu-id="ab540-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab540-116">Not supported.</span></span> |

<span data-ttu-id="ab540-117">При вызове от имени пользователя пользователю необходимо принадлежать к одной из следующих ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="ab540-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="ab540-118">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="ab540-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="ab540-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ab540-119">Global Administrator</span></span>
+ <span data-ttu-id="ab540-120">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="ab540-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="ab540-121">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="ab540-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ab540-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab540-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="ab540-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab540-123">Request headers</span></span>
| <span data-ttu-id="ab540-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ab540-124">Name</span></span>         | <span data-ttu-id="ab540-125">Тип</span><span class="sxs-lookup"><span data-stu-id="ab540-125">Type</span></span>        | <span data-ttu-id="ab540-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ab540-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ab540-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab540-127">Authorization</span></span> | <span data-ttu-id="ab540-128">string</span><span class="sxs-lookup"><span data-stu-id="ab540-128">string</span></span> | <span data-ttu-id="ab540-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab540-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab540-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab540-131">Request body</span></span>
<span data-ttu-id="ab540-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab540-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ab540-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab540-133">Response</span></span>
<span data-ttu-id="ab540-134">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` соглашения в тексте отклика. [](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="ab540-134">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab540-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ab540-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab540-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab540-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ab540-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab540-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements
```
# <a name="c"></a>[<span data-ttu-id="ab540-138">C#</span><span class="sxs-lookup"><span data-stu-id="ab540-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab540-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab540-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab540-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab540-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab540-141">Java</span><span class="sxs-lookup"><span data-stu-id="ab540-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ab540-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab540-142">Response</span></span>
><span data-ttu-id="ab540-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab540-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

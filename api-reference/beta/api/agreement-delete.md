---
title: Удаление соглашения
description: Удаление объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 0e997d3b720ee56e756e067c2e181f909f7dd539
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048227"
---
# <a name="delete-agreement"></a><span data-ttu-id="e3bfe-103">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="e3bfe-103">Delete agreement</span></span>

<span data-ttu-id="e3bfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3bfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3bfe-105">Удаление объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="e3bfe-105">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3bfe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3bfe-106">Permissions</span></span>
<span data-ttu-id="e3bfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3bfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3bfe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3bfe-109">Permission type</span></span>                        | <span data-ttu-id="e3bfe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3bfe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3bfe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3bfe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3bfe-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3bfe-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="e3bfe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3bfe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3bfe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-114">Not supported.</span></span> |
|<span data-ttu-id="e3bfe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3bfe-115">Application</span></span>                            | <span data-ttu-id="e3bfe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-116">Not supported.</span></span> |

<span data-ttu-id="e3bfe-117">При вызове от имени пользователя пользователю необходимо принадлежать к одной из следующих ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="e3bfe-118">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="e3bfe-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="e3bfe-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e3bfe-119">Global Administrator</span></span>
+ <span data-ttu-id="e3bfe-120">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="e3bfe-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="e3bfe-121">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="e3bfe-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e3bfe-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3bfe-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e3bfe-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3bfe-123">Request headers</span></span>
| <span data-ttu-id="e3bfe-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e3bfe-124">Name</span></span>         | <span data-ttu-id="e3bfe-125">Тип</span><span class="sxs-lookup"><span data-stu-id="e3bfe-125">Type</span></span>        | <span data-ttu-id="e3bfe-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e3bfe-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e3bfe-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3bfe-127">Authorization</span></span> | <span data-ttu-id="e3bfe-128">string</span><span class="sxs-lookup"><span data-stu-id="e3bfe-128">string</span></span> | <span data-ttu-id="e3bfe-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3bfe-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3bfe-131">Request body</span></span>
<span data-ttu-id="e3bfe-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e3bfe-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3bfe-133">Response</span></span>
<span data-ttu-id="e3bfe-p104">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3bfe-136">Пример</span><span class="sxs-lookup"><span data-stu-id="e3bfe-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3bfe-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3bfe-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e3bfe-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3bfe-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}
```
# <a name="c"></a>[<span data-ttu-id="e3bfe-139">C#</span><span class="sxs-lookup"><span data-stu-id="e3bfe-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3bfe-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3bfe-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3bfe-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3bfe-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3bfe-142">Java</span><span class="sxs-lookup"><span data-stu-id="e3bfe-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e3bfe-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3bfe-143">Response</span></span>
><span data-ttu-id="e3bfe-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



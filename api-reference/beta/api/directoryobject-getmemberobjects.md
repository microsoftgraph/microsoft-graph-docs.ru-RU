---
title: Вывод объектов элементов
description: " Возвращает все группы, административные единицы и роли каталога, в которые входит пользователь, группа, директоры служб или объект каталога. Это транзитивная функция. "
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a5f7ef92699cab5a7f39046e6ac5fe2fdab8585d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046848"
---
# <a name="get-member-objects"></a><span data-ttu-id="2eca4-104">Вывод объектов членства</span><span class="sxs-lookup"><span data-stu-id="2eca4-104">Get member objects</span></span>

<span data-ttu-id="2eca4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2eca4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 <span data-ttu-id="2eca4-106">Возвращает все группы, административные единицы и роли каталога, в которые входит пользователь, группа, директоры служб или объект каталога.</span><span class="sxs-lookup"><span data-stu-id="2eca4-106">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="2eca4-107">Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="2eca4-107">This function is transitive.</span></span> 
 > <span data-ttu-id="2eca4-108">Примечание. Участниками ролей каталога могут быть только пользователи.</span><span class="sxs-lookup"><span data-stu-id="2eca4-108">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="2eca4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2eca4-109">Permissions</span></span>
<span data-ttu-id="2eca4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2eca4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2eca4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2eca4-112">Permission type</span></span>      | <span data-ttu-id="2eca4-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2eca4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2eca4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2eca4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2eca4-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2eca4-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="2eca4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2eca4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2eca4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2eca4-117">Not supported.</span></span>    |
|<span data-ttu-id="2eca4-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2eca4-118">Application</span></span> | <span data-ttu-id="2eca4-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2eca4-119">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2eca4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2eca4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="2eca4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2eca4-121">Request headers</span></span>
| <span data-ttu-id="2eca4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2eca4-122">Name</span></span>       | <span data-ttu-id="2eca4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2eca4-123">Type</span></span> | <span data-ttu-id="2eca4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2eca4-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2eca4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2eca4-125">Authorization</span></span>  | <span data-ttu-id="2eca4-126">string</span><span class="sxs-lookup"><span data-stu-id="2eca4-126">string</span></span>  | <span data-ttu-id="2eca4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2eca4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2eca4-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2eca4-129">Content-Type</span></span>  | <span data-ttu-id="2eca4-130">application/json</span><span class="sxs-lookup"><span data-stu-id="2eca4-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2eca4-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2eca4-131">Request body</span></span>
<span data-ttu-id="2eca4-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2eca4-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2eca4-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="2eca4-133">Parameter</span></span>    | <span data-ttu-id="2eca4-134">Тип</span><span class="sxs-lookup"><span data-stu-id="2eca4-134">Type</span></span>   |<span data-ttu-id="2eca4-135">Описание</span><span class="sxs-lookup"><span data-stu-id="2eca4-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2eca4-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="2eca4-136">securityEnabledOnly</span></span>|<span data-ttu-id="2eca4-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="2eca4-137">Boolean</span></span>| <span data-ttu-id="2eca4-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="2eca4-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="2eca4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2eca4-140">Response</span></span>

<span data-ttu-id="2eca4-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2eca4-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2eca4-142">Пример</span><span class="sxs-lookup"><span data-stu-id="2eca4-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2eca4-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="2eca4-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2eca4-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="2eca4-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="2eca4-145">C#</span><span class="sxs-lookup"><span data-stu-id="2eca4-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2eca4-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2eca4-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2eca4-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2eca4-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2eca4-148">Java</span><span class="sxs-lookup"><span data-stu-id="2eca4-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2eca4-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="2eca4-149">Response</span></span>
<span data-ttu-id="2eca4-150">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2eca4-150">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



---
title: Вывод объектов элементов
description: " Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная функция. "
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3bd1d45833f0c164b554cc2350266f1a500216bb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448578"
---
# <a name="get-member-objects"></a><span data-ttu-id="41c0f-104">Вывод объектов членства</span><span class="sxs-lookup"><span data-stu-id="41c0f-104">Get member objects</span></span>

<span data-ttu-id="41c0f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41c0f-105">Namespace: microsoft.graph</span></span>

 <span data-ttu-id="41c0f-p102">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="41c0f-p102">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="41c0f-108">Примечание. Участниками ролей каталога могут быть только пользователи.</span><span class="sxs-lookup"><span data-stu-id="41c0f-108">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="41c0f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41c0f-109">Permissions</span></span>
<span data-ttu-id="41c0f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41c0f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41c0f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41c0f-112">Permission type</span></span>      | <span data-ttu-id="41c0f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41c0f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41c0f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41c0f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="41c0f-115">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41c0f-115">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="41c0f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41c0f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41c0f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41c0f-117">Not supported.</span></span>    |
|<span data-ttu-id="41c0f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41c0f-118">Application</span></span> | <span data-ttu-id="41c0f-119">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41c0f-119">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41c0f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41c0f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="41c0f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41c0f-121">Request headers</span></span>
| <span data-ttu-id="41c0f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="41c0f-122">Name</span></span>       | <span data-ttu-id="41c0f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="41c0f-123">Type</span></span> | <span data-ttu-id="41c0f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="41c0f-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="41c0f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="41c0f-125">Authorization</span></span>  | <span data-ttu-id="41c0f-126">string</span><span class="sxs-lookup"><span data-stu-id="41c0f-126">string</span></span>  | <span data-ttu-id="41c0f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41c0f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="41c0f-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41c0f-129">Content-Type</span></span>   | <span data-ttu-id="41c0f-130">string</span><span class="sxs-lookup"><span data-stu-id="41c0f-130">string</span></span>  | <span data-ttu-id="41c0f-131">application/json</span><span class="sxs-lookup"><span data-stu-id="41c0f-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="41c0f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41c0f-132">Request body</span></span>
<span data-ttu-id="41c0f-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="41c0f-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="41c0f-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="41c0f-134">Parameter</span></span>    | <span data-ttu-id="41c0f-135">Тип</span><span class="sxs-lookup"><span data-stu-id="41c0f-135">Type</span></span>   |<span data-ttu-id="41c0f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="41c0f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41c0f-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="41c0f-137">securityEnabledOnly</span></span>|<span data-ttu-id="41c0f-138">Логическое</span><span class="sxs-lookup"><span data-stu-id="41c0f-138">Boolean</span></span>| <span data-ttu-id="41c0f-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="41c0f-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="41c0f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="41c0f-141">Response</span></span>

<span data-ttu-id="41c0f-142">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41c0f-142">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41c0f-143">Пример</span><span class="sxs-lookup"><span data-stu-id="41c0f-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="41c0f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="41c0f-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="41c0f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="41c0f-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="41c0f-146">C#</span><span class="sxs-lookup"><span data-stu-id="41c0f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41c0f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41c0f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41c0f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41c0f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41c0f-149">Java</span><span class="sxs-lookup"><span data-stu-id="41c0f-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="41c0f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="41c0f-150">Response</span></span>
<span data-ttu-id="41c0f-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41c0f-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


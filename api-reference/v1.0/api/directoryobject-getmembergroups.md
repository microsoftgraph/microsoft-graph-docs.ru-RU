---
title: Вывод групп элементов
description: Возвращает все группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1ee6b8fa68802c9dddc49e444ead17c3003408de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016820"
---
# <a name="get-member-groups"></a><span data-ttu-id="57c97-104">Вывод групп элементов</span><span class="sxs-lookup"><span data-stu-id="57c97-104">Get member groups</span></span>

<span data-ttu-id="57c97-p102">Возвращает все группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="57c97-p102">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="57c97-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57c97-107">Permissions</span></span>
<span data-ttu-id="57c97-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57c97-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57c97-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57c97-110">Permission type</span></span>      | <span data-ttu-id="57c97-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57c97-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57c97-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57c97-112">Delegated (work or school account)</span></span> | <span data-ttu-id="57c97-113">User. ReadBasic. ALL и Group. Read. ALL, User. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="57c97-113">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="57c97-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57c97-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57c97-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57c97-115">Not supported.</span></span>    |
|<span data-ttu-id="57c97-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57c97-116">Application</span></span> | <span data-ttu-id="57c97-117">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="57c97-117">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="57c97-118">Используйте приведенные ниже рекомендации по сценариям, чтобы определить, какие типы разрешений следует использовать:</span><span class="sxs-lookup"><span data-stu-id="57c97-118">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="57c97-119">Используйте User. Read и Group. Read. ALL для получения сведений о членстве в группах для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="57c97-119">Use User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="57c97-120">Используйте User. ReadBasic. ALL и Group. Read. ALL или User. Read. ALL и Group. Read. ALL, чтобы получать сведения о членстве в группах для любого пользователя.</span><span class="sxs-lookup"><span data-stu-id="57c97-120">Use User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="57c97-121">Использование разрешения Group. Read. ALL для получения сведений о членстве в группах для группы.</span><span class="sxs-lookup"><span data-stu-id="57c97-121">Use Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="57c97-122">Используйте разрешение Directory. Read. ALL для получения сведений о членстве в группах для объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="57c97-122">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>


## <a name="http-request"></a><span data-ttu-id="57c97-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57c97-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="57c97-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57c97-124">Request headers</span></span>
| <span data-ttu-id="57c97-125">Имя</span><span class="sxs-lookup"><span data-stu-id="57c97-125">Name</span></span>       | <span data-ttu-id="57c97-126">Тип</span><span class="sxs-lookup"><span data-stu-id="57c97-126">Type</span></span> | <span data-ttu-id="57c97-127">Описание</span><span class="sxs-lookup"><span data-stu-id="57c97-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="57c97-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="57c97-128">Authorization</span></span>  | <span data-ttu-id="57c97-129">string</span><span class="sxs-lookup"><span data-stu-id="57c97-129">string</span></span>  | <span data-ttu-id="57c97-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57c97-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57c97-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57c97-132">Content-Type</span></span>   | <span data-ttu-id="57c97-133">string</span><span class="sxs-lookup"><span data-stu-id="57c97-133">string</span></span>  | <span data-ttu-id="57c97-134">application/json</span><span class="sxs-lookup"><span data-stu-id="57c97-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="57c97-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="57c97-135">Request body</span></span>
<span data-ttu-id="57c97-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="57c97-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="57c97-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="57c97-137">Parameter</span></span>    | <span data-ttu-id="57c97-138">Тип</span><span class="sxs-lookup"><span data-stu-id="57c97-138">Type</span></span>   |<span data-ttu-id="57c97-139">Описание</span><span class="sxs-lookup"><span data-stu-id="57c97-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57c97-140">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="57c97-140">securityEnabledOnly</span></span>|<span data-ttu-id="57c97-141">Логическое</span><span class="sxs-lookup"><span data-stu-id="57c97-141">Boolean</span></span>| <span data-ttu-id="57c97-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="57c97-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="57c97-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="57c97-144">Response</span></span>

<span data-ttu-id="57c97-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57c97-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57c97-146">Пример</span><span class="sxs-lookup"><span data-stu-id="57c97-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="57c97-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="57c97-147">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="57c97-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="57c97-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="57c97-149">C#</span><span class="sxs-lookup"><span data-stu-id="57c97-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57c97-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="57c97-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="57c97-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="57c97-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="57c97-152">Java</span><span class="sxs-lookup"><span data-stu-id="57c97-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="57c97-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="57c97-153">Response</span></span>
<span data-ttu-id="57c97-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57c97-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

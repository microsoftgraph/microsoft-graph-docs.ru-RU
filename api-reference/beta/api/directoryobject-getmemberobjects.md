---
title: Вывод объектов элементов
description: " Возвращает все группы, административные единицы и роли каталогов, членом которых является пользователь, группа, субъект-служба или объект каталога. Это транзитивная функция. "
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 04ca36fc0c4c2c932f7f4def46dda8b83b007528
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957775"
---
# <a name="get-member-objects"></a><span data-ttu-id="1d397-104">Вывод объектов членства</span><span class="sxs-lookup"><span data-stu-id="1d397-104">Get member objects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 <span data-ttu-id="1d397-105">Возвращает все группы, административные единицы и роли каталогов, членом которых является пользователь, группа, субъект-служба или объект каталога.</span><span class="sxs-lookup"><span data-stu-id="1d397-105">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="1d397-106">Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="1d397-106">This function is transitive.</span></span> 
 > <span data-ttu-id="1d397-107">Примечание. Участниками ролей каталога могут быть только пользователи.</span><span class="sxs-lookup"><span data-stu-id="1d397-107">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d397-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d397-108">Permissions</span></span>
<span data-ttu-id="1d397-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d397-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1d397-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d397-111">Permission type</span></span>      | <span data-ttu-id="1d397-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d397-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d397-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d397-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1d397-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d397-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="1d397-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d397-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d397-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d397-116">Not supported.</span></span>    |
|<span data-ttu-id="1d397-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d397-117">Application</span></span> | <span data-ttu-id="1d397-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d397-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d397-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d397-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="1d397-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d397-120">Request headers</span></span>
| <span data-ttu-id="1d397-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1d397-121">Name</span></span>       | <span data-ttu-id="1d397-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1d397-122">Type</span></span> | <span data-ttu-id="1d397-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1d397-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d397-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d397-124">Authorization</span></span>  | <span data-ttu-id="1d397-125">string</span><span class="sxs-lookup"><span data-stu-id="1d397-125">string</span></span>  | <span data-ttu-id="1d397-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d397-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d397-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d397-128">Content-Type</span></span>  | <span data-ttu-id="1d397-129">application/json</span><span class="sxs-lookup"><span data-stu-id="1d397-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d397-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d397-130">Request body</span></span>
<span data-ttu-id="1d397-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1d397-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1d397-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="1d397-132">Parameter</span></span>    | <span data-ttu-id="1d397-133">Тип</span><span class="sxs-lookup"><span data-stu-id="1d397-133">Type</span></span>   |<span data-ttu-id="1d397-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1d397-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d397-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="1d397-135">securityEnabledOnly</span></span>|<span data-ttu-id="1d397-136">Логическое</span><span class="sxs-lookup"><span data-stu-id="1d397-136">Boolean</span></span>| <span data-ttu-id="1d397-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="1d397-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="1d397-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d397-139">Response</span></span>

<span data-ttu-id="1d397-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d397-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d397-141">Пример</span><span class="sxs-lookup"><span data-stu-id="1d397-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1d397-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d397-142">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1d397-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d397-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1d397-144">C#</span><span class="sxs-lookup"><span data-stu-id="1d397-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1d397-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="1d397-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1d397-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1d397-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1d397-147">Java</span><span class="sxs-lookup"><span data-stu-id="1d397-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1d397-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d397-148">Response</span></span>
<span data-ttu-id="1d397-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d397-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

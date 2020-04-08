---
title: Вывод объектов элементов
description: " Возвращает все группы, административные единицы и роли каталогов, членом которых является пользователь, группа, субъект-служба или объект каталога. Это транзитивная функция. "
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 254287569da163b66fb58e9a0be292c3c6d22a64
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180939"
---
# <a name="get-member-objects"></a><span data-ttu-id="439eb-104">Вывод объектов членства</span><span class="sxs-lookup"><span data-stu-id="439eb-104">Get member objects</span></span>

<span data-ttu-id="439eb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="439eb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 <span data-ttu-id="439eb-106">Возвращает все группы, административные единицы и роли каталогов, членом которых является пользователь, группа, субъект-служба или объект каталога.</span><span class="sxs-lookup"><span data-stu-id="439eb-106">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="439eb-107">Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="439eb-107">This function is transitive.</span></span> 
 > <span data-ttu-id="439eb-108">Примечание. Участниками ролей каталога могут быть только пользователи.</span><span class="sxs-lookup"><span data-stu-id="439eb-108">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="439eb-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="439eb-109">Permissions</span></span>
<span data-ttu-id="439eb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="439eb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="439eb-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="439eb-112">Permission type</span></span>      | <span data-ttu-id="439eb-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="439eb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="439eb-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="439eb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="439eb-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="439eb-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="439eb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="439eb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="439eb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="439eb-117">Not supported.</span></span>    |
|<span data-ttu-id="439eb-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="439eb-118">Application</span></span> | <span data-ttu-id="439eb-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="439eb-119">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="439eb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="439eb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="439eb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="439eb-121">Request headers</span></span>
| <span data-ttu-id="439eb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="439eb-122">Name</span></span>       | <span data-ttu-id="439eb-123">Тип</span><span class="sxs-lookup"><span data-stu-id="439eb-123">Type</span></span> | <span data-ttu-id="439eb-124">Описание</span><span class="sxs-lookup"><span data-stu-id="439eb-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="439eb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="439eb-125">Authorization</span></span>  | <span data-ttu-id="439eb-126">string</span><span class="sxs-lookup"><span data-stu-id="439eb-126">string</span></span>  | <span data-ttu-id="439eb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="439eb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="439eb-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="439eb-129">Content-Type</span></span>  | <span data-ttu-id="439eb-130">application/json</span><span class="sxs-lookup"><span data-stu-id="439eb-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="439eb-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="439eb-131">Request body</span></span>
<span data-ttu-id="439eb-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="439eb-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="439eb-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="439eb-133">Parameter</span></span>    | <span data-ttu-id="439eb-134">Тип</span><span class="sxs-lookup"><span data-stu-id="439eb-134">Type</span></span>   |<span data-ttu-id="439eb-135">Описание</span><span class="sxs-lookup"><span data-stu-id="439eb-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="439eb-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="439eb-136">securityEnabledOnly</span></span>|<span data-ttu-id="439eb-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="439eb-137">Boolean</span></span>| <span data-ttu-id="439eb-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="439eb-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="439eb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="439eb-140">Response</span></span>

<span data-ttu-id="439eb-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="439eb-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="439eb-142">Пример</span><span class="sxs-lookup"><span data-stu-id="439eb-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="439eb-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="439eb-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="439eb-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="439eb-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="439eb-145">C#</span><span class="sxs-lookup"><span data-stu-id="439eb-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="439eb-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="439eb-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="439eb-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="439eb-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="439eb-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="439eb-148">Response</span></span>
<span data-ttu-id="439eb-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="439eb-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

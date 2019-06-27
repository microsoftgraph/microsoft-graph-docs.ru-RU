---
title: Вывод объектов элементов
description: " Возвращает все группы, административные единицы и роли каталогов, членом которых является пользователь, группа, субъект-служба или объект каталога. Это транзитивная функция. "
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1a7517d013e30e294c324f06b37954f1bd64c932
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260745"
---
# <a name="get-member-objects"></a><span data-ttu-id="5b382-104">Вывод объектов членства</span><span class="sxs-lookup"><span data-stu-id="5b382-104">Get member objects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 <span data-ttu-id="5b382-105">Возвращает все группы, административные единицы и роли каталогов, членом которых является пользователь, группа, субъект-служба или объект каталога.</span><span class="sxs-lookup"><span data-stu-id="5b382-105">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="5b382-106">Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="5b382-106">This function is transitive.</span></span> 
 > <span data-ttu-id="5b382-107">Примечание. Участниками ролей каталога могут быть только пользователи.</span><span class="sxs-lookup"><span data-stu-id="5b382-107">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b382-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b382-108">Permissions</span></span>
<span data-ttu-id="5b382-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b382-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5b382-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b382-111">Permission type</span></span>      | <span data-ttu-id="5b382-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b382-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b382-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b382-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5b382-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b382-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="5b382-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b382-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b382-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b382-116">Not supported.</span></span>    |
|<span data-ttu-id="5b382-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b382-117">Application</span></span> | <span data-ttu-id="5b382-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b382-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b382-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b382-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="5b382-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b382-120">Request headers</span></span>
| <span data-ttu-id="5b382-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5b382-121">Name</span></span>       | <span data-ttu-id="5b382-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5b382-122">Type</span></span> | <span data-ttu-id="5b382-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5b382-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5b382-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b382-124">Authorization</span></span>  | <span data-ttu-id="5b382-125">string</span><span class="sxs-lookup"><span data-stu-id="5b382-125">string</span></span>  | <span data-ttu-id="5b382-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b382-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b382-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b382-128">Content-Type</span></span>  | <span data-ttu-id="5b382-129">application/json</span><span class="sxs-lookup"><span data-stu-id="5b382-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5b382-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b382-130">Request body</span></span>
<span data-ttu-id="5b382-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5b382-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5b382-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="5b382-132">Parameter</span></span>    | <span data-ttu-id="5b382-133">Тип</span><span class="sxs-lookup"><span data-stu-id="5b382-133">Type</span></span>   |<span data-ttu-id="5b382-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5b382-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b382-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="5b382-135">securityEnabledOnly</span></span>|<span data-ttu-id="5b382-136">Логическое</span><span class="sxs-lookup"><span data-stu-id="5b382-136">Boolean</span></span>| <span data-ttu-id="5b382-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="5b382-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="5b382-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b382-139">Response</span></span>

<span data-ttu-id="5b382-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b382-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b382-141">Пример</span><span class="sxs-lookup"><span data-stu-id="5b382-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5b382-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b382-142">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="5b382-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b382-143">Response</span></span>
<span data-ttu-id="5b382-p106">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b382-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5b382-146">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5b382-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5b382-147">C#</span><span class="sxs-lookup"><span data-stu-id="5b382-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_getmemberobjects-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b382-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="5b382-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_getmemberobjects-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5b382-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5b382-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/directoryobject_getmemberobjects-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directoryobject-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directoryobject-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryobject-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

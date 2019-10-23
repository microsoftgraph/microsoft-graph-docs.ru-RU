---
title: 'orgContact: getMemberGroups'
description: Возврат всех групп, членом которых является контактное лицо.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bfff689d075fc874c3ce31b2992cf90286af3049
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633970"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="4084f-103">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="4084f-103">orgContact: getMemberGroups</span></span>

<span data-ttu-id="4084f-104">Возврат всех групп, членом которых является [Контактное лицо](../resources/orgcontact.md) .</span><span class="sxs-lookup"><span data-stu-id="4084f-104">Return all the groups that the [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="4084f-105">Проверка промежуточная, в отличие от считывания свойства навигации **memberOf** (возвращаются только группы, для которых пользователь является непосредственным членом).</span><span class="sxs-lookup"><span data-stu-id="4084f-105">The check is transitive, unlike reading the **memberOf** navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="4084f-106">Эта функция поддерживает Office 365 и другие типы групп, подготовленные в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="4084f-106">This function supports Office 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="4084f-107">Максимальное количество групп, которые может вернуть каждый запрос, — 2046.</span><span class="sxs-lookup"><span data-stu-id="4084f-107">The maximum number of groups each request can return is 2046.</span></span> 

>[!NOTE]
><span data-ttu-id="4084f-108">Группы Office 365 не могут содержать группы.</span><span class="sxs-lookup"><span data-stu-id="4084f-108">Office 365 groups cannot contain groups.</span></span> <span data-ttu-id="4084f-109">Членство в группе Office 365 всегда является прямым.</span><span class="sxs-lookup"><span data-stu-id="4084f-109">Membership in an Office 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="4084f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4084f-110">Permissions</span></span>
<span data-ttu-id="4084f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4084f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4084f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4084f-113">Permission type</span></span>      | <span data-ttu-id="4084f-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4084f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4084f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4084f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4084f-116">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4084f-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="4084f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4084f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4084f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4084f-118">Not supported.</span></span>    |
|<span data-ttu-id="4084f-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4084f-119">Application</span></span> | <span data-ttu-id="4084f-120">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4084f-120">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4084f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4084f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="4084f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4084f-122">Request headers</span></span>
| <span data-ttu-id="4084f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4084f-123">Header</span></span>       | <span data-ttu-id="4084f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4084f-124">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4084f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4084f-125">Authorization</span></span>  |  <span data-ttu-id="4084f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4084f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4084f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4084f-128">Content-type</span></span>   | <span data-ttu-id="4084f-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4084f-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4084f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4084f-131">Request body</span></span>
<span data-ttu-id="4084f-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4084f-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4084f-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="4084f-133">Parameter</span></span>    | <span data-ttu-id="4084f-134">Тип</span><span class="sxs-lookup"><span data-stu-id="4084f-134">Type</span></span>   |<span data-ttu-id="4084f-135">Описание</span><span class="sxs-lookup"><span data-stu-id="4084f-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4084f-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="4084f-136">securityEnabledOnly</span></span>|<span data-ttu-id="4084f-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="4084f-137">Boolean</span></span>|<span data-ttu-id="4084f-138">Значение `false`.</span><span class="sxs-lookup"><span data-stu-id="4084f-138">Set to `false`.</span></span> <span data-ttu-id="4084f-139">Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="4084f-139">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="4084f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4084f-140">Response</span></span>

<span data-ttu-id="4084f-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4084f-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4084f-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4084f-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4084f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4084f-143">Request</span></span>
<span data-ttu-id="4084f-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4084f-144">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4084f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4084f-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4084f-146">C#</span><span class="sxs-lookup"><span data-stu-id="4084f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4084f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4084f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4084f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4084f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4084f-149">Java</span><span class="sxs-lookup"><span data-stu-id="4084f-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4084f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4084f-150">Response</span></span>
<span data-ttu-id="4084f-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4084f-151">The following is an example of the response.</span></span>
><span data-ttu-id="4084f-152">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4084f-152">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "groupId-value1",
    "groupId-value2"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

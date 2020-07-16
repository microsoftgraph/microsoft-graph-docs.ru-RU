---
title: 'orgContact: getMemberGroups'
description: Возврат всех групп, членом которых является контактное лицо.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 431f5e01f9e74f5c9c8d5adf9b9cc2ffa8473b04
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897185"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="990cc-103">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="990cc-103">orgContact: getMemberGroups</span></span>

<span data-ttu-id="990cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="990cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="990cc-105">Возврат всех групп, членом которых является [Контактное лицо](../resources/orgcontact.md) .</span><span class="sxs-lookup"><span data-stu-id="990cc-105">Return all the groups that the [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="990cc-106">Проверка промежуточная, в отличие от считывания свойства навигации **memberOf** (возвращаются только группы, для которых пользователь является непосредственным членом).</span><span class="sxs-lookup"><span data-stu-id="990cc-106">The check is transitive, unlike reading the **memberOf** navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="990cc-107">Эта функция поддерживает Microsoft 365 и другие типы групп, подготовленные в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="990cc-107">This function supports Microsoft 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="990cc-108">Максимальное количество групп, которые может вернуть каждый запрос, — 2046.</span><span class="sxs-lookup"><span data-stu-id="990cc-108">The maximum number of groups each request can return is 2046.</span></span> 

>[!NOTE]
><span data-ttu-id="990cc-109">Группы Microsoft 365 не могут содержать группы.</span><span class="sxs-lookup"><span data-stu-id="990cc-109">Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="990cc-110">Членство в группе Microsoft 365 всегда является прямым.</span><span class="sxs-lookup"><span data-stu-id="990cc-110">Membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="990cc-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="990cc-111">Permissions</span></span>
<span data-ttu-id="990cc-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="990cc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="990cc-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="990cc-114">Permission type</span></span>      | <span data-ttu-id="990cc-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="990cc-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="990cc-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="990cc-116">Delegated (work or school account)</span></span> | <span data-ttu-id="990cc-117">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="990cc-117">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="990cc-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="990cc-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="990cc-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="990cc-119">Not supported.</span></span>    |
|<span data-ttu-id="990cc-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="990cc-120">Application</span></span> | <span data-ttu-id="990cc-121">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="990cc-121">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="990cc-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="990cc-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="990cc-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="990cc-123">Request headers</span></span>
| <span data-ttu-id="990cc-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="990cc-124">Header</span></span>       | <span data-ttu-id="990cc-125">Значение</span><span class="sxs-lookup"><span data-stu-id="990cc-125">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="990cc-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="990cc-126">Authorization</span></span>  |  <span data-ttu-id="990cc-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="990cc-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="990cc-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="990cc-129">Content-type</span></span>   | <span data-ttu-id="990cc-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="990cc-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="990cc-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="990cc-132">Request body</span></span>
<span data-ttu-id="990cc-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="990cc-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="990cc-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="990cc-134">Parameter</span></span>    | <span data-ttu-id="990cc-135">Тип</span><span class="sxs-lookup"><span data-stu-id="990cc-135">Type</span></span>   |<span data-ttu-id="990cc-136">Описание</span><span class="sxs-lookup"><span data-stu-id="990cc-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="990cc-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="990cc-137">securityEnabledOnly</span></span>|<span data-ttu-id="990cc-138">Логическое</span><span class="sxs-lookup"><span data-stu-id="990cc-138">Boolean</span></span>|<span data-ttu-id="990cc-139">Значение `false` .</span><span class="sxs-lookup"><span data-stu-id="990cc-139">Set to `false`.</span></span> <span data-ttu-id="990cc-140">Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="990cc-140">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="990cc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="990cc-141">Response</span></span>

<span data-ttu-id="990cc-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="990cc-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="990cc-143">Пример</span><span class="sxs-lookup"><span data-stu-id="990cc-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="990cc-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="990cc-144">Request</span></span>
<span data-ttu-id="990cc-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="990cc-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="990cc-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="990cc-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="990cc-147">C#</span><span class="sxs-lookup"><span data-stu-id="990cc-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="990cc-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="990cc-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="990cc-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="990cc-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="990cc-150">Java</span><span class="sxs-lookup"><span data-stu-id="990cc-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="990cc-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="990cc-151">Response</span></span>
<span data-ttu-id="990cc-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="990cc-152">The following is an example of the response.</span></span>
><span data-ttu-id="990cc-153">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="990cc-153">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

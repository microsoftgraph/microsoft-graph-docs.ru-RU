---
title: 'orgContact: getMemberGroups'
description: Возврат всех групп, членом которых является контактное лицо.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7fa053f38ffc641bdf4549c078a55bfc004e5b17
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511196"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="0646a-103">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="0646a-103">orgContact: getMemberGroups</span></span>

<span data-ttu-id="0646a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0646a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0646a-105">Возврат всех групп, членом которых является [Контактное лицо](../resources/orgcontact.md) .</span><span class="sxs-lookup"><span data-stu-id="0646a-105">Return all the groups that the [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="0646a-106">Проверка промежуточная, в отличие от считывания свойства навигации **memberOf** (возвращаются только группы, для которых пользователь является непосредственным членом).</span><span class="sxs-lookup"><span data-stu-id="0646a-106">The check is transitive, unlike reading the **memberOf** navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="0646a-107">Эта функция поддерживает Office 365 и другие типы групп, подготовленные в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0646a-107">This function supports Office 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="0646a-108">Максимальное количество групп, которые может вернуть каждый запрос, — 2046.</span><span class="sxs-lookup"><span data-stu-id="0646a-108">The maximum number of groups each request can return is 2046.</span></span> 

>[!NOTE]
><span data-ttu-id="0646a-109">Группы Office 365 не могут содержать группы.</span><span class="sxs-lookup"><span data-stu-id="0646a-109">Office 365 groups cannot contain groups.</span></span> <span data-ttu-id="0646a-110">Членство в группе Office 365 всегда является прямым.</span><span class="sxs-lookup"><span data-stu-id="0646a-110">Membership in an Office 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="0646a-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0646a-111">Permissions</span></span>
<span data-ttu-id="0646a-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0646a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0646a-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0646a-114">Permission type</span></span>      | <span data-ttu-id="0646a-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0646a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0646a-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0646a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="0646a-117">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="0646a-117">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="0646a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0646a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0646a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0646a-119">Not supported.</span></span>    |
|<span data-ttu-id="0646a-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0646a-120">Application</span></span> | <span data-ttu-id="0646a-121">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="0646a-121">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0646a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0646a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="0646a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0646a-123">Request headers</span></span>
| <span data-ttu-id="0646a-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0646a-124">Header</span></span>       | <span data-ttu-id="0646a-125">Значение</span><span class="sxs-lookup"><span data-stu-id="0646a-125">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="0646a-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0646a-126">Authorization</span></span>  |  <span data-ttu-id="0646a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0646a-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0646a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0646a-129">Content-type</span></span>   | <span data-ttu-id="0646a-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0646a-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0646a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0646a-132">Request body</span></span>
<span data-ttu-id="0646a-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0646a-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0646a-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="0646a-134">Parameter</span></span>    | <span data-ttu-id="0646a-135">Тип</span><span class="sxs-lookup"><span data-stu-id="0646a-135">Type</span></span>   |<span data-ttu-id="0646a-136">Описание</span><span class="sxs-lookup"><span data-stu-id="0646a-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0646a-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="0646a-137">securityEnabledOnly</span></span>|<span data-ttu-id="0646a-138">Логическое</span><span class="sxs-lookup"><span data-stu-id="0646a-138">Boolean</span></span>|<span data-ttu-id="0646a-139">Значение `false`.</span><span class="sxs-lookup"><span data-stu-id="0646a-139">Set to `false`.</span></span> <span data-ttu-id="0646a-140">Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="0646a-140">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="0646a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0646a-141">Response</span></span>

<span data-ttu-id="0646a-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0646a-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0646a-143">Пример</span><span class="sxs-lookup"><span data-stu-id="0646a-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0646a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="0646a-144">Request</span></span>
<span data-ttu-id="0646a-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0646a-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0646a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="0646a-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0646a-147">C#</span><span class="sxs-lookup"><span data-stu-id="0646a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0646a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0646a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0646a-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0646a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0646a-150">Java</span><span class="sxs-lookup"><span data-stu-id="0646a-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0646a-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="0646a-151">Response</span></span>
<span data-ttu-id="0646a-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0646a-152">The following is an example of the response.</span></span>
><span data-ttu-id="0646a-153">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0646a-153">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

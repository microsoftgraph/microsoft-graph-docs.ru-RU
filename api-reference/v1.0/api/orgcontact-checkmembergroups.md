---
title: 'orgContact: checkMemberGroups'
description: Проверка участия в указанном списке групп. Возвращает из списка те групповые ИД, у которых организационный контакт имеет прямое или транзитное членство.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5bdafc5ecaf7e2f95017267bf35ff140994bfb1d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761362"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="061ad-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="061ad-104">orgContact: checkMemberGroups</span></span>

<span data-ttu-id="061ad-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="061ad-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="061ad-106">Проверка участия в указанном списке групп.</span><span class="sxs-lookup"><span data-stu-id="061ad-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="061ad-107">Возвращает из списка те групповые ИД, у которых организационный контакт [имеет](../resources/orgcontact.md) прямое или транзитное членство.</span><span class="sxs-lookup"><span data-stu-id="061ad-107">Returns from the list those group IDs of which the [organizational contact](../resources/orgcontact.md) has a direct or transitive membership.</span></span>

<span data-ttu-id="061ad-108">В одном запросе можно проверять до 20 групп.</span><span class="sxs-lookup"><span data-stu-id="061ad-108">You can check up to a maximum of 20 groups per request.</span></span> <span data-ttu-id="061ad-109">Эта функция поддерживает Microsoft 365 и другие типы групп, которые предусмотрены в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="061ad-109">This function supports Microsoft 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span>

>[!NOTE]
><span data-ttu-id="061ad-110">Группы Microsoft 365 не могут содержать группы.</span><span class="sxs-lookup"><span data-stu-id="061ad-110">Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="061ad-111">Членство в группе Microsoft 365 всегда является прямым.</span><span class="sxs-lookup"><span data-stu-id="061ad-111">Membership in a Microsoft 365 group is always direct.</span></span>


## <a name="permissions"></a><span data-ttu-id="061ad-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="061ad-112">Permissions</span></span>
<span data-ttu-id="061ad-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="061ad-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="061ad-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="061ad-115">Permission type</span></span>      | <span data-ttu-id="061ad-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="061ad-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="061ad-117">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="061ad-117">Delegated (work or school account)</span></span> | <span data-ttu-id="061ad-118">OrgContact.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="061ad-118">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="061ad-119">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="061ad-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="061ad-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="061ad-120">Not supported.</span></span>    |
|<span data-ttu-id="061ad-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="061ad-121">Application</span></span> | <span data-ttu-id="061ad-122">OrgContact.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="061ad-122">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="061ad-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="061ad-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="061ad-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="061ad-124">Request headers</span></span>
| <span data-ttu-id="061ad-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="061ad-125">Header</span></span>       | <span data-ttu-id="061ad-126">Значение</span><span class="sxs-lookup"><span data-stu-id="061ad-126">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="061ad-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="061ad-127">Authorization</span></span>  | <span data-ttu-id="061ad-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="061ad-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="061ad-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="061ad-130">Content-type</span></span>   | <span data-ttu-id="061ad-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="061ad-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="061ad-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="061ad-133">Request body</span></span>
<span data-ttu-id="061ad-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="061ad-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="061ad-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="061ad-135">Parameter</span></span>    | <span data-ttu-id="061ad-136">Тип</span><span class="sxs-lookup"><span data-stu-id="061ad-136">Type</span></span>   |<span data-ttu-id="061ad-137">Описание</span><span class="sxs-lookup"><span data-stu-id="061ad-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="061ad-138">groupIds</span><span class="sxs-lookup"><span data-stu-id="061ad-138">groupIds</span></span>|<span data-ttu-id="061ad-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="061ad-139">String collection</span></span> | <span data-ttu-id="061ad-140">Список групп, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="061ad-140">A list of group IDs to check.</span></span> |

## <a name="response"></a><span data-ttu-id="061ad-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="061ad-141">Response</span></span>

<span data-ttu-id="061ad-142">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции строк в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="061ad-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="061ad-143">Пример</span><span class="sxs-lookup"><span data-stu-id="061ad-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="061ad-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="061ad-144">Request</span></span>
<span data-ttu-id="061ad-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="061ad-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="061ad-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="061ad-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupId-value1", "groupId-value2" 
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="061ad-147">C#</span><span class="sxs-lookup"><span data-stu-id="061ad-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="061ad-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="061ad-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="061ad-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="061ad-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="061ad-150">Java</span><span class="sxs-lookup"><span data-stu-id="061ad-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="061ad-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="061ad-151">Response</span></span>
<span data-ttu-id="061ad-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="061ad-152">The following is an example of the response.</span></span>
><span data-ttu-id="061ad-153">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="061ad-153">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
    "groupId-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


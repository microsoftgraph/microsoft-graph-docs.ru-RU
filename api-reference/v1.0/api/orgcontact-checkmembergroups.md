---
title: 'orgContact: Чеккмемберграупс'
description: Проверка членства в указанном списке групп. Возвращает из списка идентификаторы групп, в которых Контактное лицо имеет прямое или транзитивное членство.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5694a48cb4669bbf0c81b22d48c6e90eb90b7301
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37634025"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="fae1f-104">orgContact: Чеккмемберграупс</span><span class="sxs-lookup"><span data-stu-id="fae1f-104">orgContact: checkMemberGroups</span></span>

<span data-ttu-id="fae1f-105">Проверка членства в указанном списке групп.</span><span class="sxs-lookup"><span data-stu-id="fae1f-105">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="fae1f-106">Возвращает из списка идентификаторы групп, в которых [Контактное лицо](../resources/orgcontact.md) имеет прямое или транзитивное членство.</span><span class="sxs-lookup"><span data-stu-id="fae1f-106">Returns from the list those group IDs of which the [organizational contact](../resources/orgcontact.md) has a direct or transitive membership.</span></span>

<span data-ttu-id="fae1f-107">В одном запросе можно проверять до 20 групп.</span><span class="sxs-lookup"><span data-stu-id="fae1f-107">You can check up to a maximum of 20 groups per request.</span></span> <span data-ttu-id="fae1f-108">Эта функция поддерживает Office 365 и другие типы групп, подготовленные в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="fae1f-108">This function supports Office 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span>

>[!NOTE]
><span data-ttu-id="fae1f-109">Группы Office 365 не могут содержать группы.</span><span class="sxs-lookup"><span data-stu-id="fae1f-109">Office 365 groups cannot contain groups.</span></span> <span data-ttu-id="fae1f-110">Членство в группе Office 365 всегда является прямым.</span><span class="sxs-lookup"><span data-stu-id="fae1f-110">Membership in an Office 365 group is always direct.</span></span>


## <a name="permissions"></a><span data-ttu-id="fae1f-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fae1f-111">Permissions</span></span>
<span data-ttu-id="fae1f-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fae1f-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fae1f-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fae1f-114">Permission type</span></span>      | <span data-ttu-id="fae1f-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fae1f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fae1f-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fae1f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="fae1f-117">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="fae1f-117">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="fae1f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fae1f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fae1f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fae1f-119">Not supported.</span></span>    |
|<span data-ttu-id="fae1f-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="fae1f-120">Application</span></span> | <span data-ttu-id="fae1f-121">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="fae1f-121">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fae1f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fae1f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="fae1f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fae1f-123">Request headers</span></span>
| <span data-ttu-id="fae1f-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fae1f-124">Header</span></span>       | <span data-ttu-id="fae1f-125">Значение</span><span class="sxs-lookup"><span data-stu-id="fae1f-125">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="fae1f-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fae1f-126">Authorization</span></span>  | <span data-ttu-id="fae1f-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fae1f-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fae1f-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fae1f-129">Content-type</span></span>   | <span data-ttu-id="fae1f-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fae1f-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fae1f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fae1f-132">Request body</span></span>
<span data-ttu-id="fae1f-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fae1f-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fae1f-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="fae1f-134">Parameter</span></span>    | <span data-ttu-id="fae1f-135">Тип</span><span class="sxs-lookup"><span data-stu-id="fae1f-135">Type</span></span>   |<span data-ttu-id="fae1f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="fae1f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fae1f-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="fae1f-137">groupIds</span></span>|<span data-ttu-id="fae1f-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fae1f-138">String collection</span></span> | <span data-ttu-id="fae1f-139">Список идентификаторов групп, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="fae1f-139">A list of group IDs to check.</span></span> |

## <a name="response"></a><span data-ttu-id="fae1f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fae1f-140">Response</span></span>

<span data-ttu-id="fae1f-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fae1f-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fae1f-142">Пример</span><span class="sxs-lookup"><span data-stu-id="fae1f-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fae1f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="fae1f-143">Request</span></span>
<span data-ttu-id="fae1f-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fae1f-144">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fae1f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="fae1f-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fae1f-146">C#</span><span class="sxs-lookup"><span data-stu-id="fae1f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fae1f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fae1f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fae1f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fae1f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fae1f-149">Java</span><span class="sxs-lookup"><span data-stu-id="fae1f-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fae1f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="fae1f-150">Response</span></span>
<span data-ttu-id="fae1f-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fae1f-151">The following is an example of the response.</span></span>
><span data-ttu-id="fae1f-152">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fae1f-152">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

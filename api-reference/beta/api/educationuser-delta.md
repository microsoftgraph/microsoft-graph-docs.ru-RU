---
title: 'educationUser: delta'
description: Получите новых или обновленных пользователей, не выполняя полное чтение всей коллекции пользователей.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7477bea6eeb01e74cb824a7d31b0cc5dba3161ef
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042928"
---
# <a name="educationuser-delta"></a><span data-ttu-id="8fce6-103">educationUser: delta</span><span class="sxs-lookup"><span data-stu-id="8fce6-103">educationUser: delta</span></span>

<span data-ttu-id="8fce6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fce6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fce6-105">Получите новый или обновленный [educationUser](../resources/educationuser.md) без выполнения полного чтения всей коллекции.</span><span class="sxs-lookup"><span data-stu-id="8fce6-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="8fce6-106">Подробные [сведения см. в запросе Use Delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="8fce6-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fce6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8fce6-107">Permissions</span></span>

<span data-ttu-id="8fce6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fce6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8fce6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fce6-110">Permission type</span></span>                        | <span data-ttu-id="8fce6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fce6-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="8fce6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fce6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8fce6-113">EduRoster.ReadBasic, EduRoster.Read или EduRoster.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8fce6-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="8fce6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fce6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fce6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fce6-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="8fce6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fce6-116">Application</span></span>                            | <span data-ttu-id="8fce6-117">EduRoster.ReadBasic.All, EduRoster.Read.All или EduRoster.WriteWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fce6-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fce6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fce6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/users/delta
```

## <a name="request-headers"></a><span data-ttu-id="8fce6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8fce6-119">Request headers</span></span>

| <span data-ttu-id="8fce6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8fce6-120">Name</span></span>          | <span data-ttu-id="8fce6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8fce6-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="8fce6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8fce6-122">Authorization</span></span> | <span data-ttu-id="8fce6-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8fce6-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fce6-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fce6-124">Request body</span></span>

<span data-ttu-id="8fce6-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8fce6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fce6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fce6-126">Response</span></span>

<span data-ttu-id="8fce6-127">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [коллекции educationUser](../resources/educationuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8fce6-127">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8fce6-128">дельты educationUser не включают удаленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="8fce6-128">educationUser deltas do not include deleted users.</span></span>

## <a name="example"></a><span data-ttu-id="8fce6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8fce6-129">Example</span></span>

<span data-ttu-id="8fce6-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8fce6-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8fce6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fce6-131">Request</span></span>

<span data-ttu-id="8fce6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fce6-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8fce6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8fce6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/delta
```
# <a name="c"></a>[<span data-ttu-id="8fce6-134">C#</span><span class="sxs-lookup"><span data-stu-id="8fce6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationuser-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8fce6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fce6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationuser-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8fce6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8fce6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationuser-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8fce6-137">Java</span><span class="sxs-lookup"><span data-stu-id="8fce6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationuser-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8fce6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fce6-138">Response</span></span>

<span data-ttu-id="8fce6-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8fce6-139">The following is an example of the response.</span></span>

> <span data-ttu-id="8fce6-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8fce6-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1039

{
  "value": [
    {
      "accountEnabled": true,
      "assignedLicenses": [{ "@odata.type": "microsoft.graph.assignedLicense" }],
      "assignedPlans": [{ "@odata.type": "microsoft.graph.assignedPlan" }],
      "businessPhones": ["String"],
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "department": "String",
      "displayName": "String",
      "externalSource": "string",
      "givenName": "String",
      "id": "String (identifier)",
      "mail": "String",
      "mailNickname": "String",
      "mailingAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
      "middleName": "String",
      "mobilePhone": "String",
      "officeLocation": "String",
      "onPremisesInfo": {
        "@odata.type": "microsoft.graph.educationOnPremisesInfo"
      },
      "passwordPolicies": "String",
      "passwordProfile": { "@odata.type": "microsoft.graph.passwordProfile" },
      "preferredLanguage": "String",
      "primaryRole": "string",
      "provisionedPlans": [{ "@odata.type": "microsoft.graph.provisionedPlan" }],
      "residenceAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
      "student": { "@odata.type": "microsoft.graph.educationStudent" },
      "surname": "String",
      "teacher": { "@odata.type": "microsoft.graph.educationTeacher" },
      "usageLocation": "String",
      "userPrincipalName": "String",
      "userType": "String"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



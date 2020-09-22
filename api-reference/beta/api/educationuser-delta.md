---
title: 'educationUser: Delta'
description: Получите новых или обновленных пользователей, не требуя полного прочтения всей коллекции пользователей.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 758942338cbe62ea254ae437bb3e70fd6d5ee465
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007131"
---
# <a name="educationuser-delta"></a><span data-ttu-id="8074a-103">educationUser: Delta</span><span class="sxs-lookup"><span data-stu-id="8074a-103">educationUser: delta</span></span>

<span data-ttu-id="8074a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8074a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8074a-105">Получите только что созданный или обновленный [educationUser](../resources/educationuser.md) , не требуя полного считывания всей коллекции.</span><span class="sxs-lookup"><span data-stu-id="8074a-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="8074a-106">Дополнительные сведения: [use Query Delta Query](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="8074a-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="8074a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8074a-107">Permissions</span></span>

<span data-ttu-id="8074a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8074a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8074a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8074a-110">Permission type</span></span>                        | <span data-ttu-id="8074a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8074a-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="8074a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8074a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8074a-113">EduRoster. ReadBasic, EduRoster. Read или EduRoster. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8074a-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="8074a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8074a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8074a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8074a-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="8074a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8074a-116">Application</span></span>                            | <span data-ttu-id="8074a-117">EduRoster. ReadBasic. ALL, EduRoster. Read. ALL или EduRoster. Вритеврите. ALL</span><span class="sxs-lookup"><span data-stu-id="8074a-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8074a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8074a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/users/delta
```

## <a name="request-headers"></a><span data-ttu-id="8074a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8074a-119">Request headers</span></span>

| <span data-ttu-id="8074a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8074a-120">Name</span></span>          | <span data-ttu-id="8074a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8074a-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="8074a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8074a-122">Authorization</span></span> | <span data-ttu-id="8074a-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8074a-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8074a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8074a-124">Request body</span></span>

<span data-ttu-id="8074a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8074a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8074a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8074a-126">Response</span></span>

<span data-ttu-id="8074a-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [educationUser](../resources/educationuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8074a-127">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8074a-128">разность educationUser не включает удаленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="8074a-128">educationUser deltas do not include deleted users.</span></span>

## <a name="example"></a><span data-ttu-id="8074a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8074a-129">Example</span></span>

<span data-ttu-id="8074a-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8074a-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8074a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8074a-131">Request</span></span>

<span data-ttu-id="8074a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8074a-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8074a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8074a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/delta
```
# <a name="c"></a>[<span data-ttu-id="8074a-134">C#</span><span class="sxs-lookup"><span data-stu-id="8074a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationuser-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8074a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8074a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationuser-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8074a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8074a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationuser-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8074a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8074a-137">Response</span></span>

<span data-ttu-id="8074a-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8074a-138">The following is an example of the response.</span></span>

> <span data-ttu-id="8074a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8074a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



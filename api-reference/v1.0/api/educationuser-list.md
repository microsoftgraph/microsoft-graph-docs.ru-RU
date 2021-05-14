---
title: List educationUser
description: Получите список объектов educationUser и их свойств.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6cf915d28369314d960ee4b868bafd2852819c7f
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475391"
---
# <a name="list-educationusers"></a><span data-ttu-id="82b8e-103">Перечисление EducationUsers</span><span class="sxs-lookup"><span data-stu-id="82b8e-103">List educationUsers</span></span>

<span data-ttu-id="82b8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82b8e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82b8e-105">Получите список объектов [educationUser](../resources/educationuser.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="82b8e-105">Get a list of the [educationUser](../resources/educationuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="82b8e-106">Разрешения:</span><span class="sxs-lookup"><span data-stu-id="82b8e-106">Permissions</span></span>

<span data-ttu-id="82b8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82b8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="82b8e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82b8e-109">Permission type</span></span>                        | <span data-ttu-id="82b8e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82b8e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="82b8e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82b8e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="82b8e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82b8e-112">Not supported.</span></span>                              |
| <span data-ttu-id="82b8e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82b8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82b8e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82b8e-114">Not supported.</span></span>                              |
| <span data-ttu-id="82b8e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="82b8e-115">Application</span></span>                            | <span data-ttu-id="82b8e-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82b8e-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82b8e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82b8e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82b8e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82b8e-118">Optional query parameters</span></span>

<span data-ttu-id="82b8e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="82b8e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span>

<span data-ttu-id="82b8e-120">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="82b8e-120">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="82b8e-121">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="82b8e-121">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="82b8e-122">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="82b8e-122">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="82b8e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82b8e-123">Request headers</span></span>

| <span data-ttu-id="82b8e-124">Имя</span><span class="sxs-lookup"><span data-stu-id="82b8e-124">Name</span></span>          | <span data-ttu-id="82b8e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="82b8e-125">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="82b8e-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82b8e-126">Authorization</span></span> | <span data-ttu-id="82b8e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82b8e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82b8e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82b8e-129">Request body</span></span>

<span data-ttu-id="82b8e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82b8e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82b8e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="82b8e-131">Response</span></span>

<span data-ttu-id="82b8e-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="82b8e-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82b8e-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="82b8e-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82b8e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="82b8e-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="82b8e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="82b8e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_educationuser"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/users
```
# <a name="c"></a>[<span data-ttu-id="82b8e-136">C#</span><span class="sxs-lookup"><span data-stu-id="82b8e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82b8e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82b8e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82b8e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82b8e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82b8e-139">Java</span><span class="sxs-lookup"><span data-stu-id="82b8e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="82b8e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="82b8e-140">Response</span></span>

> <span data-ttu-id="82b8e-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="82b8e-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationUser)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationUser",
      "id": "90eedea1-dea1-90ee-a1de-ee90a1deee90",
      "primaryRole": "String",
      "middleName": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "residenceAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "mailingAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "student": {
        "@odata.type": "microsoft.graph.educationStudent"
      },
      "teacher": {
        "@odata.type": "microsoft.graph.educationTeacher"
      },
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "accountEnabled": "Boolean",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan"
        }
      ],
      "businessPhones": [
        "String"
      ],
      "department": "String",
      "displayName": "String",
      "givenName": "String",
      "mail": "String",
      "mailNickname": "String",
      "mobilePhone": "String",
      "passwordPolicies": "String",
      "passwordProfile": {
        "@odata.type": "microsoft.graph.passwordProfile"
      },
      "officeLocation": "String",
      "preferredLanguage": "String",
      "provisionedPlans": [
        {
          "@odata.type": "microsoft.graph.provisionedPlan"
        }
      ],
      "refreshTokensValidFromDateTime": "String (timestamp)",
      "showInAddressList": "Boolean",
      "surname": "String",
      "usageLocation": "String",
      "userPrincipalName": "String",
      "userType": "String",
      "onPremisesInfo": {
        "@odata.type": "microsoft.graph.educationOnPremisesInfo"
      }
    }
  ]
}
```

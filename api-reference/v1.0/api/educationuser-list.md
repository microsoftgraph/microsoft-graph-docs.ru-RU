---
title: List educationUser
description: Получите список объектов educationUser и их свойств.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2fa8f0105257991ca5b7ea255d3ea3b534bb079b
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232265"
---
# <a name="list-educationusers"></a><span data-ttu-id="b8cb0-103">Перечисление EducationUsers</span><span class="sxs-lookup"><span data-stu-id="b8cb0-103">List educationUsers</span></span>

<span data-ttu-id="b8cb0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8cb0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8cb0-105">Получите список объектов [educationUser](../resources/educationuser.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="b8cb0-105">Get a list of the [educationUser](../resources/educationuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8cb0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8cb0-106">Permissions</span></span>

<span data-ttu-id="b8cb0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8cb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8cb0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8cb0-109">Permission type</span></span>                        | <span data-ttu-id="b8cb0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8cb0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="b8cb0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8cb0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8cb0-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8cb0-112">Not supported.</span></span>                              |
| <span data-ttu-id="b8cb0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8cb0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8cb0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8cb0-114">Not supported.</span></span>                              |
| <span data-ttu-id="b8cb0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b8cb0-115">Application</span></span>                            | <span data-ttu-id="b8cb0-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8cb0-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8cb0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8cb0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8cb0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b8cb0-118">Optional query parameters</span></span>

<span data-ttu-id="b8cb0-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="b8cb0-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span>

<span data-ttu-id="b8cb0-120">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="b8cb0-120">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="b8cb0-121">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="b8cb0-121">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="b8cb0-122">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b8cb0-122">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8cb0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8cb0-123">Request headers</span></span>

| <span data-ttu-id="b8cb0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b8cb0-124">Name</span></span>          | <span data-ttu-id="b8cb0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b8cb0-125">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b8cb0-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8cb0-126">Authorization</span></span> | <span data-ttu-id="b8cb0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8cb0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8cb0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8cb0-129">Request body</span></span>

<span data-ttu-id="b8cb0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8cb0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8cb0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8cb0-131">Response</span></span>

<span data-ttu-id="b8cb0-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b8cb0-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8cb0-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="b8cb0-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b8cb0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8cb0-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_educationuser"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/users
```

### <a name="response"></a><span data-ttu-id="b8cb0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8cb0-135">Response</span></span>

> <span data-ttu-id="b8cb0-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b8cb0-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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

---
title: 'educationUser: delta'
description: Получите новых или обновленных пользователей, не выполняя полное чтение всей коллекции пользователей.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eddf1656a9f1366276b89fd5b101768b45e2cca1
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232246"
---
# <a name="educationuser-delta"></a><span data-ttu-id="8c6b5-103">educationUser: delta</span><span class="sxs-lookup"><span data-stu-id="8c6b5-103">educationUser: delta</span></span>

<span data-ttu-id="8c6b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c6b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c6b5-105">Получите новый или обновленный [educationUser](../resources/educationuser.md) без выполнения полного чтения всей коллекции.</span><span class="sxs-lookup"><span data-stu-id="8c6b5-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="8c6b5-106">Подробные [сведения см. в запросе Use Delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="8c6b5-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c6b5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c6b5-107">Permissions</span></span>

<span data-ttu-id="8c6b5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c6b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c6b5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c6b5-110">Permission type</span></span>                        | <span data-ttu-id="8c6b5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c6b5-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="8c6b5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c6b5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c6b5-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="8c6b5-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="8c6b5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c6b5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c6b5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c6b5-115">Not supported.</span></span>                              |
| <span data-ttu-id="8c6b5-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8c6b5-116">Application</span></span>                            | <span data-ttu-id="8c6b5-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c6b5-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c6b5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c6b5-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/users/delta
```

## <a name="request-headers"></a><span data-ttu-id="8c6b5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c6b5-119">Request headers</span></span>

| <span data-ttu-id="8c6b5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8c6b5-120">Name</span></span>          | <span data-ttu-id="8c6b5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8c6b5-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8c6b5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c6b5-122">Authorization</span></span> | <span data-ttu-id="8c6b5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c6b5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c6b5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c6b5-125">Request body</span></span>

<span data-ttu-id="8c6b5-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c6b5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c6b5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c6b5-127">Response</span></span>

<span data-ttu-id="8c6b5-128">В случае успешной работы эта функция возвращает код ответа и `200 OK` [коллекцию educationUser](../resources/educationuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c6b5-128">If successful, this function returns a `200 OK` response code and a [educationUser](../resources/educationuser.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c6b5-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c6b5-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c6b5-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c6b5-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/users/delta
```

### <a name="response"></a><span data-ttu-id="8c6b5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c6b5-131">Response</span></span>

> <span data-ttu-id="8c6b5-132">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c6b5-132">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationUser)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/users/delta?$skiptoken=VwhMSQw1l1O5v2F1ZPm...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationUser",
      "id": "String (identifier)",
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

---
title: Получение educationSchool
description: Ознакомьтесь с свойствами и отношениями объекта educationSchool.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 21732795ec15c16a92563eccebdeb7e8d33d3793
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231265"
---
# <a name="get-educationschool"></a><span data-ttu-id="4afc4-103">Получение educationSchool</span><span class="sxs-lookup"><span data-stu-id="4afc4-103">Get educationSchool</span></span>

<span data-ttu-id="4afc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4afc4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4afc4-105">Ознакомьтесь с свойствами и отношениями объекта [educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="4afc4-105">Read the properties and relationships of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4afc4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4afc4-106">Permissions</span></span>

<span data-ttu-id="4afc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4afc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4afc4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4afc4-109">Permission type</span></span>                        | <span data-ttu-id="4afc4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4afc4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4afc4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4afc4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4afc4-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="4afc4-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="4afc4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4afc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4afc4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4afc4-114">Not supported.</span></span>                              |
| <span data-ttu-id="4afc4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4afc4-115">Application</span></span>                            | <span data-ttu-id="4afc4-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4afc4-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4afc4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4afc4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/{educationSchoolId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4afc4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4afc4-118">Optional query parameters</span></span>

<span data-ttu-id="4afc4-119">Этот метод поддерживает те же параметры запроса OData, что [и Get User.](../api/user-get.md#optional-query-parameters)</span><span class="sxs-lookup"><span data-stu-id="4afc4-119">This method supports the same OData query parameters as [Get User](../api/user-get.md#optional-query-parameters).</span></span> <span data-ttu-id="4afc4-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4afc4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4afc4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4afc4-121">Request headers</span></span>

| <span data-ttu-id="4afc4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4afc4-122">Name</span></span>          | <span data-ttu-id="4afc4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4afc4-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4afc4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4afc4-124">Authorization</span></span> | <span data-ttu-id="4afc4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4afc4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4afc4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4afc4-127">Request body</span></span>

<span data-ttu-id="4afc4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4afc4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4afc4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4afc4-129">Response</span></span>

<span data-ttu-id="4afc4-130">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4afc4-130">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4afc4-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="4afc4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4afc4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4afc4-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/schools/{educationSchoolId}
```

### <a name="response"></a><span data-ttu-id="4afc4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4afc4-133">Response</span></span>

><span data-ttu-id="4afc4-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4afc4-134">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationSchool",
    "id": "1c23c12e-c12e-1c23-2ec1-231c2ec1231c",
    "displayName": "String",
    "description": "String",
    "externalSource": "String",
    "externalSourceDetail": "String",
    "principalEmail": "String",
    "principalName": "String",
    "externalPrincipalId": "String",
    "lowestGrade": "String",
    "highestGrade": "String",
    "schoolNumber": "String",
    "externalId": "String",
    "phone": "String",
    "fax": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress"
    }
  }
}
```

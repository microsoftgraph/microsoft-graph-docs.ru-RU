---
title: Перечисление educationSchools
description: Получите список объектов educationSchool и их свойств.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 98602e535864f7c62c673af66b717758bebb2c97
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232266"
---
# <a name="list-educationschools"></a><span data-ttu-id="24252-103">Перечисление educationSchools</span><span class="sxs-lookup"><span data-stu-id="24252-103">List educationSchools</span></span>

<span data-ttu-id="24252-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24252-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24252-105">Получите список объектов [educationSchool](../resources/educationschool.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="24252-105">Get a list of the [educationSchool](../resources/educationschool.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="24252-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24252-106">Permissions</span></span>

<span data-ttu-id="24252-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24252-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24252-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24252-109">Permission type</span></span>                        | <span data-ttu-id="24252-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24252-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="24252-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24252-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="24252-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="24252-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="24252-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24252-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24252-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24252-114">Not supported.</span></span>                              |
| <span data-ttu-id="24252-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="24252-115">Application</span></span>                            | <span data-ttu-id="24252-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24252-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24252-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24252-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24252-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="24252-118">Optional query parameters</span></span>

<span data-ttu-id="24252-119">Этот метод поддерживает те же параметры запроса OData, что и [пользователи списка.](../api/user-list.md#optional-query-parameters)</span><span class="sxs-lookup"><span data-stu-id="24252-119">This method supports the same OData query parameters as [List Users](../api/user-list.md#optional-query-parameters).</span></span> <span data-ttu-id="24252-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="24252-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="24252-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24252-121">Request headers</span></span>

| <span data-ttu-id="24252-122">Имя</span><span class="sxs-lookup"><span data-stu-id="24252-122">Name</span></span>          | <span data-ttu-id="24252-123">Описание</span><span class="sxs-lookup"><span data-stu-id="24252-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="24252-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24252-124">Authorization</span></span> | <span data-ttu-id="24252-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24252-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24252-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24252-127">Request body</span></span>

<span data-ttu-id="24252-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24252-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24252-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="24252-129">Response</span></span>

<span data-ttu-id="24252-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="24252-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24252-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="24252-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24252-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="24252-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_educationschool"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/schools
```

### <a name="response"></a><span data-ttu-id="24252-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="24252-133">Response</span></span>

> <span data-ttu-id="24252-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="24252-134">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationSchool)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```

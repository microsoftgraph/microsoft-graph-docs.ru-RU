---
title: Список administrativeUnit an educationSchool
description: Получите список административных объектов, связанных с объектом educationSchool.
author: mmast
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5cd736b14be199f729556c619015ab5fee1e857b
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232289"
---
# <a name="list-administrativeunit-an-educationschool"></a><span data-ttu-id="91274-103">Список administrativeUnit an educationSchool</span><span class="sxs-lookup"><span data-stu-id="91274-103">List administrativeUnit an educationSchool</span></span>

<span data-ttu-id="91274-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91274-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91274-105">Получите список **административных объектов,** связанных с [объектом educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="91274-105">Get a list of **administrativeUnits** associated with an [educationSchool](../resources/educationschool.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="91274-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91274-106">Permissions</span></span>

<span data-ttu-id="91274-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91274-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91274-109">Permission type</span></span>                        | <span data-ttu-id="91274-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91274-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="91274-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91274-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="91274-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="91274-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="91274-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91274-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91274-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91274-114">Not supported.</span></span>                              |
| <span data-ttu-id="91274-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="91274-115">Application</span></span>                            | <span data-ttu-id="91274-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91274-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91274-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91274-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/{educationSchoolId}/administrativeUnit
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91274-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91274-118">Optional query parameters</span></span>

<span data-ttu-id="91274-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="91274-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="91274-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="91274-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="91274-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91274-121">Request headers</span></span>

| <span data-ttu-id="91274-122">Имя</span><span class="sxs-lookup"><span data-stu-id="91274-122">Name</span></span>          | <span data-ttu-id="91274-123">Описание</span><span class="sxs-lookup"><span data-stu-id="91274-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="91274-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91274-124">Authorization</span></span> | <span data-ttu-id="91274-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91274-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91274-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91274-127">Request body</span></span>

<span data-ttu-id="91274-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91274-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91274-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="91274-129">Response</span></span>

<span data-ttu-id="91274-130">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов administrativeUnit](../resources/administrativeunit.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="91274-130">If successful, this method returns a `200 OK` response code and a collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91274-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="91274-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91274-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="91274-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_administrativeunit"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit
```

### <a name="response"></a><span data-ttu-id="91274-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="91274-133">Response</span></span>

> <span data-ttu-id="91274-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="91274-134">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.administrativeUnit)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.administrativeUnit",
      "id": "03e281d6-81d6-03e2-d681-e203d681e203",
      "deletedDateTime": "String (timestamp)",
      "displayName": "String",
      "description": "String",
      "visibility": "String"
    }
  ]
}
```

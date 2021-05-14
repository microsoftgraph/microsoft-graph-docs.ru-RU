---
title: Список administrativeUnit an educationSchool
description: Получите список административных объектов, связанных с объектом educationSchool.
author: mmast
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a8ca5a51c6fb71c3cab0d6f0a7be239eb2101999
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474866"
---
# <a name="list-administrativeunit-an-educationschool"></a><span data-ttu-id="cece9-103">Список administrativeUnit an educationSchool</span><span class="sxs-lookup"><span data-stu-id="cece9-103">List administrativeUnit an educationSchool</span></span>

<span data-ttu-id="cece9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cece9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cece9-105">Получите список **административных объектов,** связанных с [объектом educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="cece9-105">Get a list of **administrativeUnits** associated with an [educationSchool](../resources/educationschool.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cece9-106">Разрешения:</span><span class="sxs-lookup"><span data-stu-id="cece9-106">Permissions</span></span>

<span data-ttu-id="cece9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cece9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cece9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cece9-109">Permission type</span></span>                        | <span data-ttu-id="cece9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cece9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="cece9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cece9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cece9-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="cece9-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="cece9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cece9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cece9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cece9-114">Not supported.</span></span>                              |
| <span data-ttu-id="cece9-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="cece9-115">Application</span></span>                            | <span data-ttu-id="cece9-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cece9-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cece9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cece9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/{educationSchoolId}/administrativeUnit
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cece9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cece9-118">Optional query parameters</span></span>

<span data-ttu-id="cece9-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cece9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cece9-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cece9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cece9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cece9-121">Request headers</span></span>

| <span data-ttu-id="cece9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cece9-122">Name</span></span>          | <span data-ttu-id="cece9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cece9-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cece9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cece9-124">Authorization</span></span> | <span data-ttu-id="cece9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cece9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cece9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cece9-127">Request body</span></span>

<span data-ttu-id="cece9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cece9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cece9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cece9-129">Response</span></span>

<span data-ttu-id="cece9-130">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов administrativeUnit](../resources/administrativeunit.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cece9-130">If successful, this method returns a `200 OK` response code and a collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cece9-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="cece9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cece9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cece9-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cece9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cece9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_administrativeunit"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit
```
# <a name="c"></a>[<span data-ttu-id="cece9-134">C#</span><span class="sxs-lookup"><span data-stu-id="cece9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cece9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cece9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cece9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cece9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cece9-137">Java</span><span class="sxs-lookup"><span data-stu-id="cece9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cece9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cece9-138">Response</span></span>

> <span data-ttu-id="cece9-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cece9-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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

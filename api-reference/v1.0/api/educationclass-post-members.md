---
title: Добавление учащегося
description: Добавление участника курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5fc2000b119d25e144079639909dbd7c4c9c9a10
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616008"
---
# <a name="add-a-student"></a><span data-ttu-id="7a1aa-103">Добавление учащегося</span><span class="sxs-lookup"><span data-stu-id="7a1aa-103">Add a student</span></span>

<span data-ttu-id="7a1aa-104">Добавление участника курса.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-104">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a1aa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a1aa-105">Permissions</span></span>
<span data-ttu-id="7a1aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a1aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a1aa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a1aa-108">Permission type</span></span>      | <span data-ttu-id="7a1aa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a1aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a1aa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a1aa-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7a1aa-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-111">Not supported.</span></span>  |
|<span data-ttu-id="7a1aa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a1aa-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7a1aa-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-113">Not supported.</span></span>  |
|<span data-ttu-id="7a1aa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a1aa-114">Application</span></span> | <span data-ttu-id="7a1aa-115">EduRoster. ReadWrite. ALL, Plus Member. Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="7a1aa-115">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7a1aa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a1aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7a1aa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a1aa-117">Request headers</span></span>
| <span data-ttu-id="7a1aa-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a1aa-118">Header</span></span>       | <span data-ttu-id="7a1aa-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7a1aa-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7a1aa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a1aa-120">Authorization</span></span>  | <span data-ttu-id="7a1aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7a1aa-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a1aa-123">Content-Type</span></span>  | <span data-ttu-id="7a1aa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7a1aa-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7a1aa-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a1aa-125">Request body</span></span>
<span data-ttu-id="7a1aa-126">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="7a1aa-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a1aa-127">Response</span></span>
<span data-ttu-id="7a1aa-128">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a1aa-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7a1aa-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a1aa-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a1aa-130">Request</span></span>
<span data-ttu-id="7a1aa-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/13015"
}
```

##### <a name="response"></a><span data-ttu-id="7a1aa-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a1aa-132">Response</span></span>
<span data-ttu-id="7a1aa-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-133">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7a1aa-134">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="7a1aa-134">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a1aa-135">Язык</span><span class="sxs-lookup"><span data-stu-id="7a1aa-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationuser_from_educationclass-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationclass-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

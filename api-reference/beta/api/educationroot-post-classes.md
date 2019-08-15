---
title: Создание educationClass
description: Создание курса. При этом будет также создана универсальная группа. При использовании этого API для создания класса он добавляет в группу специальные свойства, которые будут
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6ff566637bcf26e0caedb3bd16b3a7c8a56e583f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416270"
---
# <a name="create-educationclass"></a><span data-ttu-id="1f55b-105">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="1f55b-105">Create educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f55b-106">Создание курса.</span><span class="sxs-lookup"><span data-stu-id="1f55b-106">Create a new class.</span></span> <span data-ttu-id="1f55b-107">При этом будет также создана универсальная группа.</span><span class="sxs-lookup"><span data-stu-id="1f55b-107">This will also create a universal group.</span></span> <span data-ttu-id="1f55b-108">Если вы используете этот API для создания курса, он добавит специальные свойства в группу, что приведет к добавлению возможностей, таких как задания и специальная обработка в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1f55b-108">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f55b-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f55b-109">Permissions</span></span>
<span data-ttu-id="1f55b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f55b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f55b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f55b-112">Permission type</span></span>      | <span data-ttu-id="1f55b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f55b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f55b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f55b-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="1f55b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f55b-115">Not supported.</span></span>  |
|<span data-ttu-id="1f55b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f55b-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1f55b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f55b-117">Not supported.</span></span>  |
|<span data-ttu-id="1f55b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f55b-118">Application</span></span> | <span data-ttu-id="1f55b-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f55b-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1f55b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f55b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="1f55b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f55b-121">Request headers</span></span>
| <span data-ttu-id="1f55b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f55b-122">Header</span></span>       | <span data-ttu-id="1f55b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1f55b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1f55b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f55b-124">Authorization</span></span>  | <span data-ttu-id="1f55b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f55b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1f55b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f55b-127">Content-Type</span></span>  | <span data-ttu-id="1f55b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1f55b-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1f55b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f55b-129">Request body</span></span>
<span data-ttu-id="1f55b-130">В теле запроса предоставьте описание объекта [educationClass](../resources/educationclass.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f55b-130">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="1f55b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f55b-131">Response</span></span>
<span data-ttu-id="1f55b-132">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1f55b-132">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f55b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1f55b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f55b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f55b-134">Request</span></span>
<span data-ttu-id="1f55b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f55b-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1f55b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f55b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes
Content-type: application/json
Content-length: 224

{
  "description": "Health Level 1",
  "classCode": "Health 501",
  "displayName": "Health 1",
  "externalId": "11019",
  "externalName": "Health Level 1",
  "externalSource": "sis",
  "mailNickname": "fineartschool.net"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1f55b-137">C#</span><span class="sxs-lookup"><span data-stu-id="1f55b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f55b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f55b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1f55b-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1f55b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1f55b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f55b-140">Response</span></span>
<span data-ttu-id="1f55b-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f55b-141">The following is an example of the response.</span></span> 

><span data-ttu-id="1f55b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f55b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 224

{
    "id": "11019",
    "description": "Health Level 1",
    "classCode": "Health 501",
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012",
      }
    },
    "displayName": "Health 1",
    "externalId": "11019",
    "externalName": "Health Level 1",
    "externalSource": "sis",
    "mailNickname": "fineartschool.net"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

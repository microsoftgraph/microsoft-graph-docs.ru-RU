---
title: Создание educationClass
description: Создание курса. При этом будет также создана универсальная группа. При использовании этого API для создания класса он добавляет в группу специальные свойства, которые будут
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e07e5f24c45c4847c35af5999a8ed16bc470564d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517525"
---
# <a name="create-educationclass"></a><span data-ttu-id="fd560-105">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="fd560-105">Create educationClass</span></span>

<span data-ttu-id="fd560-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd560-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fd560-107">Создание курса.</span><span class="sxs-lookup"><span data-stu-id="fd560-107">Create a new class.</span></span> <span data-ttu-id="fd560-108">При этом будет также создана универсальная группа.</span><span class="sxs-lookup"><span data-stu-id="fd560-108">This will also create a universal group.</span></span> <span data-ttu-id="fd560-109">Если вы используете этот API для создания курса, он добавит специальные свойства в группу, что приведет к добавлению возможностей, таких как задания и специальная обработка в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="fd560-109">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd560-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd560-110">Permissions</span></span>
<span data-ttu-id="fd560-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd560-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd560-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd560-113">Permission type</span></span>      | <span data-ttu-id="fd560-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd560-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd560-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd560-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="fd560-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd560-116">Not supported.</span></span>  |
|<span data-ttu-id="fd560-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd560-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fd560-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd560-118">Not supported.</span></span>  |
|<span data-ttu-id="fd560-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd560-119">Application</span></span> | <span data-ttu-id="fd560-120">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd560-120">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fd560-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd560-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="fd560-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd560-122">Request headers</span></span>
| <span data-ttu-id="fd560-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd560-123">Header</span></span>       | <span data-ttu-id="fd560-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fd560-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd560-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd560-125">Authorization</span></span>  | <span data-ttu-id="fd560-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd560-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fd560-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd560-128">Content-Type</span></span>  | <span data-ttu-id="fd560-129">application/json</span><span class="sxs-lookup"><span data-stu-id="fd560-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd560-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd560-130">Request body</span></span>
<span data-ttu-id="fd560-131">В теле запроса предоставьте описание объекта [educationClass](../resources/educationclass.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd560-131">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="fd560-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd560-132">Response</span></span>
<span data-ttu-id="fd560-133">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fd560-133">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd560-134">Пример</span><span class="sxs-lookup"><span data-stu-id="fd560-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd560-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd560-135">Request</span></span>
<span data-ttu-id="fd560-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd560-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fd560-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd560-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes
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
# <a name="c"></a>[<span data-ttu-id="fd560-138">C#</span><span class="sxs-lookup"><span data-stu-id="fd560-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd560-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd560-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd560-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd560-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fd560-141">Java</span><span class="sxs-lookup"><span data-stu-id="fd560-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fd560-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd560-142">Response</span></span>
<span data-ttu-id="fd560-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fd560-143">The following is an example of the response.</span></span> 

><span data-ttu-id="fd560-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd560-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

---
title: Создание educationClass
description: Создание курса. При этом будет также создана универсальная группа. При использовании этого API для создания класса в группу будут добавлены специальные свойства, которые будут
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: df566e35dd2bed527ef36f181cd9c4c92791843e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043649"
---
# <a name="create-educationclass"></a><span data-ttu-id="cd05f-105">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="cd05f-105">Create educationClass</span></span>

<span data-ttu-id="cd05f-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd05f-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd05f-107">Создание курса.</span><span class="sxs-lookup"><span data-stu-id="cd05f-107">Create a new class.</span></span> <span data-ttu-id="cd05f-108">При этом будет также создана универсальная группа.</span><span class="sxs-lookup"><span data-stu-id="cd05f-108">This will also create a universal group.</span></span> <span data-ttu-id="cd05f-109">При использовании этого API для создания класса в группу будут добавлены специальные свойства, которые будут добавлять такие функции, как назначения и специальная обработка в Microsoft Teams при создании групп с помощью группы.</span><span class="sxs-lookup"><span data-stu-id="cd05f-109">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams when teams are created using the group.</span></span> <span data-ttu-id="cd05f-110">Обратите внимание, что этот API создает только универсальную группу и не создает команду.</span><span class="sxs-lookup"><span data-stu-id="cd05f-110">Please note that this API only creates the universal group and does not create a team.</span></span> <span data-ttu-id="cd05f-111">Microsoft Teams предоставляет пользовательский интерфейс для преподавателей для создания групп для своих классов с помощью групп, созданных этим API.</span><span class="sxs-lookup"><span data-stu-id="cd05f-111">Microsoft Teams provides a user interface for teachers to create teams for their own classes using the groups created by this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd05f-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd05f-112">Permissions</span></span>
<span data-ttu-id="cd05f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd05f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd05f-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd05f-115">Permission type</span></span>      | <span data-ttu-id="cd05f-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd05f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd05f-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd05f-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="cd05f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd05f-118">Not supported.</span></span>  |
|<span data-ttu-id="cd05f-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd05f-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cd05f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd05f-120">Not supported.</span></span>  |
|<span data-ttu-id="cd05f-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd05f-121">Application</span></span> | <span data-ttu-id="cd05f-122">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd05f-122">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cd05f-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd05f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="cd05f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd05f-124">Request headers</span></span>
| <span data-ttu-id="cd05f-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd05f-125">Header</span></span>       | <span data-ttu-id="cd05f-126">Значение</span><span class="sxs-lookup"><span data-stu-id="cd05f-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cd05f-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd05f-127">Authorization</span></span>  | <span data-ttu-id="cd05f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd05f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd05f-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd05f-130">Content-Type</span></span>  | <span data-ttu-id="cd05f-131">application/json</span><span class="sxs-lookup"><span data-stu-id="cd05f-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd05f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd05f-132">Request body</span></span>
<span data-ttu-id="cd05f-133">В теле запроса предоставьте описание объекта [educationClass](../resources/educationclass.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd05f-133">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="cd05f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd05f-134">Response</span></span>
<span data-ttu-id="cd05f-135">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cd05f-135">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd05f-136">Пример</span><span class="sxs-lookup"><span data-stu-id="cd05f-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd05f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd05f-137">Request</span></span>
<span data-ttu-id="cd05f-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd05f-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cd05f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd05f-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cd05f-140">C#</span><span class="sxs-lookup"><span data-stu-id="cd05f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd05f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd05f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd05f-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd05f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd05f-143">Java</span><span class="sxs-lookup"><span data-stu-id="cd05f-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cd05f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd05f-144">Response</span></span>
<span data-ttu-id="cd05f-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cd05f-145">The following is an example of the response.</span></span> 

><span data-ttu-id="cd05f-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cd05f-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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



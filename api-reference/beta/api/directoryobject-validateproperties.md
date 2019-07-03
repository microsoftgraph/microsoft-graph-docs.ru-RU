---
title: 'directoryObject: Валидатепропертиес'
description: Убедитесь, что отображаемое имя или псевдоним почты группы Office 365 соответствует политикам именования.  Клиенты могут использовать API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **создать** группу Office 365. Для проверки свойств существующей группы используйте функцию Валидатепропертиес для групп.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b9d8b5211628e017da2ecc35aaea5b28d77b3d5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436986"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="e19fe-105">directoryObject: Валидатепропертиес</span><span class="sxs-lookup"><span data-stu-id="e19fe-105">directoryObject: validateProperties</span></span>

<span data-ttu-id="e19fe-106">Убедитесь, что отображаемое имя или псевдоним почты группы Office 365 соответствует политикам именования.</span><span class="sxs-lookup"><span data-stu-id="e19fe-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="e19fe-107">Клиенты могут использовать API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **создать** группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="e19fe-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **create** an Office 365 group.</span></span> <span data-ttu-id="e19fe-108">Для проверки свойств существующей группы используйте [функцию валидатепропертиес](group-validateproperties.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="e19fe-108">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="e19fe-109">Для отображаемого имени и свойств псевдонима почты выполняются следующие проверки.</span><span class="sxs-lookup"><span data-stu-id="e19fe-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="e19fe-110">Проверка политики именования префиксов и суффиксов</span><span class="sxs-lookup"><span data-stu-id="e19fe-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="e19fe-111">Проверка политики нестандартных запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="e19fe-111">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="e19fe-112">Проверка уникальности псевдонима почты</span><span class="sxs-lookup"><span data-stu-id="e19fe-112">Validate the mail nickname is unique</span></span>

<span data-ttu-id="e19fe-113">Этот API возвращается при первом обнаружении ошибки.</span><span class="sxs-lookup"><span data-stu-id="e19fe-113">This API returns with the first failure encountered.</span></span> <span data-ttu-id="e19fe-114">Если одно или несколько свойств не прошли несколько проверок, возвращается только свойство с первой ошибкой проверки.</span><span class="sxs-lookup"><span data-stu-id="e19fe-114">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="e19fe-115">Тем не менее, вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяется только политика именования префиксов и суффиксов.</span><span class="sxs-lookup"><span data-stu-id="e19fe-115">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e19fe-116">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="e19fe-116">Prerequisites</span></span>

<span data-ttu-id="e19fe-117">Для выполнения этого API требуются следующие **разрешения** : *Group. Read. ALL*</span><span class="sxs-lookup"><span data-stu-id="e19fe-117">The following **permission** is required to execute this API: *Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="e19fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e19fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="e19fe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e19fe-119">Request headers</span></span>

| <span data-ttu-id="e19fe-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e19fe-120">Name</span></span>           | <span data-ttu-id="e19fe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e19fe-121">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="e19fe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e19fe-122">Authorization</span></span>  | <span data-ttu-id="e19fe-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e19fe-123">Bearer {code}</span></span>    |
| <span data-ttu-id="e19fe-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e19fe-124">Content-Type</span></span>   | <span data-ttu-id="e19fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e19fe-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e19fe-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e19fe-126">Request body</span></span>
<span data-ttu-id="e19fe-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e19fe-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e19fe-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="e19fe-128">Parameter</span></span>    | <span data-ttu-id="e19fe-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e19fe-129">Type</span></span>   |<span data-ttu-id="e19fe-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e19fe-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e19fe-131">Сущности</span><span class="sxs-lookup"><span data-stu-id="e19fe-131">entityType</span></span>|<span data-ttu-id="e19fe-132">String</span><span class="sxs-lookup"><span data-stu-id="e19fe-132">String</span></span>| <span data-ttu-id="e19fe-133">`Group`— единственный поддерживаемый тип объекта.</span><span class="sxs-lookup"><span data-stu-id="e19fe-133">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="e19fe-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e19fe-134">displayName</span></span>|<span data-ttu-id="e19fe-135">Строка</span><span class="sxs-lookup"><span data-stu-id="e19fe-135">String</span></span>| <span data-ttu-id="e19fe-136">Отображаемое имя группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="e19fe-136">The display name of the group to validate.</span></span> <span data-ttu-id="e19fe-137">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="e19fe-137">The property is not individually required.</span></span> <span data-ttu-id="e19fe-138">Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="e19fe-138">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="e19fe-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e19fe-139">mailNickname</span></span>|<span data-ttu-id="e19fe-140">String</span><span class="sxs-lookup"><span data-stu-id="e19fe-140">String</span></span>| <span data-ttu-id="e19fe-141">Псевдоним почты для группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="e19fe-141">The mail nickname of the group to validate.</span></span> <span data-ttu-id="e19fe-142">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="e19fe-142">The property is not individually required.</span></span> <span data-ttu-id="e19fe-143">Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="e19fe-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="e19fe-144">Онбехалфофусерид</span><span class="sxs-lookup"><span data-stu-id="e19fe-144">onBehalfOfUserId</span></span>|<span data-ttu-id="e19fe-145">GUID</span><span class="sxs-lookup"><span data-stu-id="e19fe-145">Guid</span></span>| <span data-ttu-id="e19fe-146">Идентификатор объекта пользователя, который олицетворяет при вызове API.</span><span class="sxs-lookup"><span data-stu-id="e19fe-146">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="e19fe-147">Результаты проверки предназначены для атрибутов и ролей Онбехалфофусерид.</span><span class="sxs-lookup"><span data-stu-id="e19fe-147">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="e19fe-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="e19fe-148">Response</span></span>

<span data-ttu-id="e19fe-149">При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="e19fe-149">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="e19fe-150">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e19fe-150">It does not return anything in the response body.</span></span>

<span data-ttu-id="e19fe-151">Если запрос является недопустимым, метод возвращает `400 Bad Request` код отклика.</span><span class="sxs-lookup"><span data-stu-id="e19fe-151">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="e19fe-152">В тексте отклика возвращается сообщение об ошибке со сведениями о недопустимом запросе.</span><span class="sxs-lookup"><span data-stu-id="e19fe-152">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="e19fe-153">При возникновении ошибки проверки метод возвращает `422 Unprocessable Entity` код отклика.</span><span class="sxs-lookup"><span data-stu-id="e19fe-153">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="e19fe-154">В тексте отклика возвращается сообщение об ошибке и коллекция сведений об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e19fe-154">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e19fe-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="e19fe-155">Examples</span></span>

<span data-ttu-id="e19fe-156">В этом примере показан успешный запрос на проверку.</span><span class="sxs-lookup"><span data-stu-id="e19fe-156">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="e19fe-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="e19fe-157">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e19fe-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="e19fe-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e19fe-159">C#</span><span class="sxs-lookup"><span data-stu-id="e19fe-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e19fe-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="e19fe-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e19fe-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e19fe-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e19fe-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="e19fe-162">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="e19fe-163">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="e19fe-163">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="e19fe-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="e19fe-164">Request</span></span>
```http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="e19fe-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="e19fe-165">Response</span></span>
```http
HTTP/1.1 422 
Content-Type: application/json

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "request-id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "displayName",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      },
      {
        "target": "mailNickname",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

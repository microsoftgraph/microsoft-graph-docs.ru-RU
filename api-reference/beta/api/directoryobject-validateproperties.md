---
title: 'directoryObject: Валидатепропертиес'
description: Убедитесь, что отображаемое имя или псевдоним почты группы Office 365 соответствует политикам именования.  Клиенты могут использовать API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **создать** группу Office 365. Для проверки свойств существующей группы используйте функцию Валидатепропертиес для групп.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3bb9ad8108d4adc9a2dcd2f11866ea90a75acfb4
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951642"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="ac15b-105">directoryObject: Валидатепропертиес</span><span class="sxs-lookup"><span data-stu-id="ac15b-105">directoryObject: validateProperties</span></span>

<span data-ttu-id="ac15b-106">Убедитесь, что отображаемое имя или псевдоним почты группы Office 365 соответствует политикам именования.</span><span class="sxs-lookup"><span data-stu-id="ac15b-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="ac15b-107">Клиенты могут использовать API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **создать** группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="ac15b-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **create** an Office 365 group.</span></span> <span data-ttu-id="ac15b-108">Для проверки свойств существующей группы используйте [функцию валидатепропертиес](group-validateproperties.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="ac15b-108">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="ac15b-109">Для отображаемого имени и свойств псевдонима почты выполняются следующие проверки.</span><span class="sxs-lookup"><span data-stu-id="ac15b-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="ac15b-110">Проверка политики именования префиксов и суффиксов</span><span class="sxs-lookup"><span data-stu-id="ac15b-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="ac15b-111">Проверка политики нестандартных запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="ac15b-111">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="ac15b-112">Проверка уникальности псевдонима почты</span><span class="sxs-lookup"><span data-stu-id="ac15b-112">Validate the mail nickname is unique</span></span>

<span data-ttu-id="ac15b-113">Этот API возвращается при первом обнаружении ошибки.</span><span class="sxs-lookup"><span data-stu-id="ac15b-113">This API returns with the first failure encountered.</span></span> <span data-ttu-id="ac15b-114">Если одно или несколько свойств не прошли несколько проверок, возвращается только свойство с первой ошибкой проверки.</span><span class="sxs-lookup"><span data-stu-id="ac15b-114">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="ac15b-115">Тем не менее, вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяется только политика именования префиксов и суффиксов.</span><span class="sxs-lookup"><span data-stu-id="ac15b-115">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac15b-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac15b-116">Permissions</span></span>
<span data-ttu-id="ac15b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac15b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac15b-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac15b-119">Permission type</span></span>      | <span data-ttu-id="ac15b-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac15b-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac15b-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac15b-121">Delegated (work or school account)</span></span> | <span data-ttu-id="ac15b-122">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ac15b-122">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ac15b-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac15b-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac15b-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac15b-124">Not supported.</span></span>    |
|<span data-ttu-id="ac15b-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac15b-125">Application</span></span> | <span data-ttu-id="ac15b-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac15b-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac15b-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac15b-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="ac15b-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac15b-128">Request headers</span></span>

| <span data-ttu-id="ac15b-129">Имя</span><span class="sxs-lookup"><span data-stu-id="ac15b-129">Name</span></span>           | <span data-ttu-id="ac15b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ac15b-130">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="ac15b-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac15b-131">Authorization</span></span>  | <span data-ttu-id="ac15b-132">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ac15b-132">Bearer {code}</span></span>    |
| <span data-ttu-id="ac15b-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac15b-133">Content-Type</span></span>   | <span data-ttu-id="ac15b-134">application/json</span><span class="sxs-lookup"><span data-stu-id="ac15b-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac15b-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac15b-135">Request body</span></span>
<span data-ttu-id="ac15b-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ac15b-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ac15b-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="ac15b-137">Parameter</span></span>    | <span data-ttu-id="ac15b-138">Тип</span><span class="sxs-lookup"><span data-stu-id="ac15b-138">Type</span></span>   |<span data-ttu-id="ac15b-139">Описание</span><span class="sxs-lookup"><span data-stu-id="ac15b-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac15b-140">Сущности</span><span class="sxs-lookup"><span data-stu-id="ac15b-140">entityType</span></span>|<span data-ttu-id="ac15b-141">String</span><span class="sxs-lookup"><span data-stu-id="ac15b-141">String</span></span>| <span data-ttu-id="ac15b-142">`Group`— единственный поддерживаемый тип объекта.</span><span class="sxs-lookup"><span data-stu-id="ac15b-142">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="ac15b-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ac15b-143">displayName</span></span>|<span data-ttu-id="ac15b-144">Строка</span><span class="sxs-lookup"><span data-stu-id="ac15b-144">String</span></span>| <span data-ttu-id="ac15b-145">Отображаемое имя группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="ac15b-145">The display name of the group to validate.</span></span> <span data-ttu-id="ac15b-146">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="ac15b-146">The property is not individually required.</span></span> <span data-ttu-id="ac15b-147">Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="ac15b-147">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="ac15b-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ac15b-148">mailNickname</span></span>|<span data-ttu-id="ac15b-149">String</span><span class="sxs-lookup"><span data-stu-id="ac15b-149">String</span></span>| <span data-ttu-id="ac15b-150">Псевдоним почты для группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="ac15b-150">The mail nickname of the group to validate.</span></span> <span data-ttu-id="ac15b-151">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="ac15b-151">The property is not individually required.</span></span> <span data-ttu-id="ac15b-152">Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="ac15b-152">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="ac15b-153">онбехалфофусерид</span><span class="sxs-lookup"><span data-stu-id="ac15b-153">onBehalfOfUserId</span></span>|<span data-ttu-id="ac15b-154">GUID</span><span class="sxs-lookup"><span data-stu-id="ac15b-154">Guid</span></span>| <span data-ttu-id="ac15b-155">Идентификатор объекта пользователя, который олицетворяет при вызове API.</span><span class="sxs-lookup"><span data-stu-id="ac15b-155">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="ac15b-156">Результаты проверки предназначены для атрибутов и ролей Онбехалфофусерид.</span><span class="sxs-lookup"><span data-stu-id="ac15b-156">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="ac15b-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac15b-157">Response</span></span>

<span data-ttu-id="ac15b-158">При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="ac15b-158">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="ac15b-159">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ac15b-159">It does not return anything in the response body.</span></span>

<span data-ttu-id="ac15b-160">Если запрос является недопустимым, метод возвращает `400 Bad Request` код отклика.</span><span class="sxs-lookup"><span data-stu-id="ac15b-160">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="ac15b-161">В тексте отклика возвращается сообщение об ошибке со сведениями о недопустимом запросе.</span><span class="sxs-lookup"><span data-stu-id="ac15b-161">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="ac15b-162">При возникновении ошибки проверки метод возвращает `422 Unprocessable Entity` код отклика.</span><span class="sxs-lookup"><span data-stu-id="ac15b-162">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="ac15b-163">В тексте отклика возвращается сообщение об ошибке и коллекция сведений об ошибке.</span><span class="sxs-lookup"><span data-stu-id="ac15b-163">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac15b-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="ac15b-164">Examples</span></span>

<span data-ttu-id="ac15b-165">В этом примере показан успешный запрос на проверку.</span><span class="sxs-lookup"><span data-stu-id="ac15b-165">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="ac15b-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac15b-166">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ac15b-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac15b-167">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ac15b-168">C#</span><span class="sxs-lookup"><span data-stu-id="ac15b-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac15b-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac15b-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ac15b-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac15b-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac15b-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac15b-171">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="ac15b-172">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="ac15b-172">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="ac15b-173">Запросить</span><span class="sxs-lookup"><span data-stu-id="ac15b-173">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="ac15b-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac15b-174">Response</span></span>
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

---
title: 'directoryObject: проверка Свойств'
description: Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 699175bfd3d51deb07d64722a7196fcf9dcc8880
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436836"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="db9f7-103">directoryObject: проверка Свойств</span><span class="sxs-lookup"><span data-stu-id="db9f7-103">directoryObject: validateProperties</span></span>

<span data-ttu-id="db9f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db9f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db9f7-105">Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="db9f7-105">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="db9f7-106">Клиенты могут использовать этот API, чтобы определить, допустимо  ли имя или псевдоним почты перед попыткой создать группу Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="db9f7-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to **create** a Microsoft 365 group.</span></span> <span data-ttu-id="db9f7-107">Для проверки свойств существующей группы используйте функцию [validateProperties](group-validateproperties.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="db9f7-107">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="db9f7-108">Следующие проверки выполняются для свойств отображения имени и ником почты:</span><span class="sxs-lookup"><span data-stu-id="db9f7-108">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="db9f7-109">Проверка политики имен префикса и суффикса</span><span class="sxs-lookup"><span data-stu-id="db9f7-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="db9f7-110">Проверка настраиваемой политики запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="db9f7-110">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="db9f7-111">Проверка уникального псевдонима почты</span><span class="sxs-lookup"><span data-stu-id="db9f7-111">Validate the mail nickname is unique</span></span>

<span data-ttu-id="db9f7-112">Этот API возвращается с первым сбоем.</span><span class="sxs-lookup"><span data-stu-id="db9f7-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="db9f7-113">Если одно или несколько свойств не удается несколько проверки, возвращается только свойство с первым сбоем проверки.</span><span class="sxs-lookup"><span data-stu-id="db9f7-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="db9f7-114">Однако вы можете проверить как имя почты, так и имя дисплея и получить коллекцию ошибок проверки, если вы только проверяете политику именования префикса и суффикса.</span><span class="sxs-lookup"><span data-stu-id="db9f7-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="db9f7-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db9f7-115">Permissions</span></span>
<span data-ttu-id="db9f7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db9f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db9f7-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db9f7-118">Permission type</span></span>      | <span data-ttu-id="db9f7-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db9f7-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db9f7-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db9f7-120">Delegated (work or school account)</span></span> | <span data-ttu-id="db9f7-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="db9f7-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="db9f7-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db9f7-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db9f7-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db9f7-123">Not supported.</span></span>    |
|<span data-ttu-id="db9f7-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db9f7-124">Application</span></span> | <span data-ttu-id="db9f7-125">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db9f7-125">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db9f7-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db9f7-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="db9f7-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db9f7-127">Request headers</span></span>

| <span data-ttu-id="db9f7-128">Имя</span><span class="sxs-lookup"><span data-stu-id="db9f7-128">Name</span></span>           | <span data-ttu-id="db9f7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="db9f7-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="db9f7-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db9f7-130">Authorization</span></span>  | <span data-ttu-id="db9f7-131">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="db9f7-131">Bearer {code}.</span></span> <span data-ttu-id="db9f7-132">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="db9f7-132">Required.</span></span>   |
| <span data-ttu-id="db9f7-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db9f7-133">Content-Type</span></span>   | <span data-ttu-id="db9f7-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db9f7-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db9f7-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db9f7-136">Request body</span></span>
<span data-ttu-id="db9f7-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="db9f7-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="db9f7-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="db9f7-138">Parameter</span></span>    | <span data-ttu-id="db9f7-139">Тип</span><span class="sxs-lookup"><span data-stu-id="db9f7-139">Type</span></span>   |<span data-ttu-id="db9f7-140">Описание</span><span class="sxs-lookup"><span data-stu-id="db9f7-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db9f7-141">entityType</span><span class="sxs-lookup"><span data-stu-id="db9f7-141">entityType</span></span>|<span data-ttu-id="db9f7-142">String</span><span class="sxs-lookup"><span data-stu-id="db9f7-142">String</span></span>| <span data-ttu-id="db9f7-143">`Group` это единственный поддерживаемый тип сущности.</span><span class="sxs-lookup"><span data-stu-id="db9f7-143">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="db9f7-144">displayName</span><span class="sxs-lookup"><span data-stu-id="db9f7-144">displayName</span></span>|<span data-ttu-id="db9f7-145">String</span><span class="sxs-lookup"><span data-stu-id="db9f7-145">String</span></span>| <span data-ttu-id="db9f7-146">Отображаемого имени группы для проверки.</span><span class="sxs-lookup"><span data-stu-id="db9f7-146">The display name of the group to validate.</span></span> <span data-ttu-id="db9f7-147">Свойство не требуется по отдельности.</span><span class="sxs-lookup"><span data-stu-id="db9f7-147">The property is not individually required.</span></span> <span data-ttu-id="db9f7-148">Однако требуется по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="db9f7-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="db9f7-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="db9f7-149">mailNickname</span></span>|<span data-ttu-id="db9f7-150">String</span><span class="sxs-lookup"><span data-stu-id="db9f7-150">String</span></span>| <span data-ttu-id="db9f7-151">Имя почты группы для проверки.</span><span class="sxs-lookup"><span data-stu-id="db9f7-151">The mail nickname of the group to validate.</span></span> <span data-ttu-id="db9f7-152">Свойство не требуется по отдельности.</span><span class="sxs-lookup"><span data-stu-id="db9f7-152">The property is not individually required.</span></span> <span data-ttu-id="db9f7-153">Однако требуется по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="db9f7-153">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="db9f7-154">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="db9f7-154">onBehalfOfUserId</span></span>|<span data-ttu-id="db9f7-155">Guid</span><span class="sxs-lookup"><span data-stu-id="db9f7-155">Guid</span></span>| <span data-ttu-id="db9f7-156">ID объекта пользователя, который должен выдать себя при вызове API.</span><span class="sxs-lookup"><span data-stu-id="db9f7-156">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="db9f7-157">Результаты проверки для атрибутов и ролей onBehalfOfUserId.</span><span class="sxs-lookup"><span data-stu-id="db9f7-157">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="db9f7-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="db9f7-158">Response</span></span>

<span data-ttu-id="db9f7-159">В случае успешной проверки и без ошибок проверки метод возвращает `204 No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="db9f7-159">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="db9f7-160">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="db9f7-160">It does not return anything in the response body.</span></span>

<span data-ttu-id="db9f7-161">Если запрос недействителен, метод возвращает `400 Bad Request` код ответа.</span><span class="sxs-lookup"><span data-stu-id="db9f7-161">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="db9f7-162">Сообщение об ошибке с сведениями о недействительности запроса возвращается в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="db9f7-162">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="db9f7-163">При ошибке проверки метод возвращает `422 Unprocessable Entity` код ответа.</span><span class="sxs-lookup"><span data-stu-id="db9f7-163">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="db9f7-164">Сообщение об ошибке и коллекция сведений об ошибках возвращаются в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="db9f7-164">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db9f7-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="db9f7-165">Examples</span></span>

<span data-ttu-id="db9f7-166">Это пример успешного запроса на проверку.</span><span class="sxs-lookup"><span data-stu-id="db9f7-166">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="db9f7-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="db9f7-167">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="db9f7-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="db9f7-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="db9f7-169">C#</span><span class="sxs-lookup"><span data-stu-id="db9f7-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db9f7-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db9f7-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db9f7-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db9f7-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db9f7-172">Java</span><span class="sxs-lookup"><span data-stu-id="db9f7-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db9f7-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="db9f7-173">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="db9f7-174">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="db9f7-174">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="db9f7-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="db9f7-175">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="db9f7-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="db9f7-176">Response</span></span>
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



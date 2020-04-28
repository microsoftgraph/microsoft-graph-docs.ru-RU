---
title: 'directoryObject: Валидатепропертиес'
description: Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fcdaa24b874b30db52e737ed048618b6cf6d4377
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180925"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="dd7f6-103">directoryObject: Валидатепропертиес</span><span class="sxs-lookup"><span data-stu-id="dd7f6-103">directoryObject: validateProperties</span></span>

<span data-ttu-id="dd7f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd7f6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd7f6-105">Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-105">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="dd7f6-106">Клиенты могут использовать этот API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **создать** группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to **create** an Office 365 group.</span></span> <span data-ttu-id="dd7f6-107">Для проверки свойств существующей группы используйте [функцию валидатепропертиес](group-validateproperties.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-107">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="dd7f6-108">Для отображаемого имени и свойств псевдонима почты выполняются следующие проверки.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-108">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="dd7f6-109">Проверка политики именования префиксов и суффиксов</span><span class="sxs-lookup"><span data-stu-id="dd7f6-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="dd7f6-110">Проверка политики нестандартных запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="dd7f6-110">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="dd7f6-111">Проверка уникальности псевдонима почты</span><span class="sxs-lookup"><span data-stu-id="dd7f6-111">Validate the mail nickname is unique</span></span>

<span data-ttu-id="dd7f6-112">Этот API возвращается при первом обнаружении ошибки.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="dd7f6-113">Если одно или несколько свойств не прошли несколько проверок, возвращается только свойство с первой ошибкой проверки.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="dd7f6-114">Тем не менее, вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяется только политика именования префиксов и суффиксов.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd7f6-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd7f6-115">Permissions</span></span>
<span data-ttu-id="dd7f6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd7f6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd7f6-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd7f6-118">Permission type</span></span>      | <span data-ttu-id="dd7f6-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd7f6-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd7f6-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd7f6-120">Delegated (work or school account)</span></span> | <span data-ttu-id="dd7f6-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd7f6-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="dd7f6-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd7f6-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd7f6-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-123">Not supported.</span></span>    |
|<span data-ttu-id="dd7f6-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd7f6-124">Application</span></span> | <span data-ttu-id="dd7f6-125">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd7f6-125">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd7f6-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd7f6-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="dd7f6-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd7f6-127">Request headers</span></span>

| <span data-ttu-id="dd7f6-128">Имя</span><span class="sxs-lookup"><span data-stu-id="dd7f6-128">Name</span></span>           | <span data-ttu-id="dd7f6-129">Описание</span><span class="sxs-lookup"><span data-stu-id="dd7f6-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="dd7f6-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd7f6-130">Authorization</span></span>  | <span data-ttu-id="dd7f6-131">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-131">Bearer {code}.</span></span> <span data-ttu-id="dd7f6-132">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-132">Required.</span></span>   |
| <span data-ttu-id="dd7f6-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd7f6-133">Content-Type</span></span>   | <span data-ttu-id="dd7f6-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd7f6-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd7f6-136">Request body</span></span>
<span data-ttu-id="dd7f6-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dd7f6-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="dd7f6-138">Parameter</span></span>    | <span data-ttu-id="dd7f6-139">Тип</span><span class="sxs-lookup"><span data-stu-id="dd7f6-139">Type</span></span>   |<span data-ttu-id="dd7f6-140">Описание</span><span class="sxs-lookup"><span data-stu-id="dd7f6-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd7f6-141">Сущности</span><span class="sxs-lookup"><span data-stu-id="dd7f6-141">entityType</span></span>|<span data-ttu-id="dd7f6-142">String</span><span class="sxs-lookup"><span data-stu-id="dd7f6-142">String</span></span>| <span data-ttu-id="dd7f6-143">`Group`— единственный поддерживаемый тип объекта.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-143">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="dd7f6-144">displayName</span><span class="sxs-lookup"><span data-stu-id="dd7f6-144">displayName</span></span>|<span data-ttu-id="dd7f6-145">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7f6-145">String</span></span>| <span data-ttu-id="dd7f6-146">Отображаемое имя группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-146">The display name of the group to validate.</span></span> <span data-ttu-id="dd7f6-147">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-147">The property is not individually required.</span></span> <span data-ttu-id="dd7f6-148">Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="dd7f6-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="dd7f6-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="dd7f6-149">mailNickname</span></span>|<span data-ttu-id="dd7f6-150">String</span><span class="sxs-lookup"><span data-stu-id="dd7f6-150">String</span></span>| <span data-ttu-id="dd7f6-151">Псевдоним почты для группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-151">The mail nickname of the group to validate.</span></span> <span data-ttu-id="dd7f6-152">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-152">The property is not individually required.</span></span> <span data-ttu-id="dd7f6-153">Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="dd7f6-153">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="dd7f6-154">онбехалфофусерид</span><span class="sxs-lookup"><span data-stu-id="dd7f6-154">onBehalfOfUserId</span></span>|<span data-ttu-id="dd7f6-155">GUID</span><span class="sxs-lookup"><span data-stu-id="dd7f6-155">Guid</span></span>| <span data-ttu-id="dd7f6-156">Идентификатор объекта пользователя, который олицетворяет при вызове API.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-156">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="dd7f6-157">Результаты проверки предназначены для атрибутов и ролей Онбехалфофусерид.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-157">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="dd7f6-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd7f6-158">Response</span></span>

<span data-ttu-id="dd7f6-159">При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-159">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="dd7f6-160">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-160">It does not return anything in the response body.</span></span>

<span data-ttu-id="dd7f6-161">Если запрос является недопустимым, метод возвращает `400 Bad Request` код отклика.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-161">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="dd7f6-162">В тексте отклика возвращается сообщение об ошибке со сведениями о недопустимом запросе.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-162">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="dd7f6-163">При возникновении ошибки проверки метод возвращает `422 Unprocessable Entity` код отклика.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-163">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="dd7f6-164">В тексте отклика возвращается сообщение об ошибке и коллекция сведений об ошибке.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-164">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd7f6-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="dd7f6-165">Examples</span></span>

<span data-ttu-id="dd7f6-166">В этом примере показан успешный запрос на проверку.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-166">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="dd7f6-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd7f6-167">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="dd7f6-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd7f6-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dd7f6-169">C#</span><span class="sxs-lookup"><span data-stu-id="dd7f6-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd7f6-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd7f6-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd7f6-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd7f6-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dd7f6-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd7f6-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="dd7f6-173">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="dd7f6-173">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="dd7f6-174">Запросить</span><span class="sxs-lookup"><span data-stu-id="dd7f6-174">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="dd7f6-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd7f6-175">Response</span></span>
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

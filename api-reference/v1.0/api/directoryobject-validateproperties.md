---
title: 'directoryObject: Валидатепропертиес'
description: Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 38943c87509c99f2287729ea3d3f688731b46f24
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181911"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="65d02-103">directoryObject: Валидатепропертиес</span><span class="sxs-lookup"><span data-stu-id="65d02-103">directoryObject: validateProperties</span></span>

<span data-ttu-id="65d02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65d02-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65d02-105">Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="65d02-105">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="65d02-106">Клиенты могут использовать этот API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться [создать](group-post-groups.md) группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="65d02-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [create](group-post-groups.md) an Office 365 group.</span></span> <span data-ttu-id="65d02-107">Чтобы проверить свойства существующей группы, используйте функцию [Group: валидатепропертиес](group-validateproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="65d02-107">To validate the properties of an existing group, use the [group: validateProperties](group-validateproperties.md) function.</span></span>

<span data-ttu-id="65d02-108">Для отображаемого имени и свойств псевдонима почты выполняются следующие проверки политик:</span><span class="sxs-lookup"><span data-stu-id="65d02-108">The following policy validations are performed for the display name and mail nickname properties:</span></span>
1. <span data-ttu-id="65d02-109">Проверка политики именования префиксов и суффиксов</span><span class="sxs-lookup"><span data-stu-id="65d02-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="65d02-110">Проверка политики нестандартных запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="65d02-110">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="65d02-111">Проверка уникальности псевдонима почты</span><span class="sxs-lookup"><span data-stu-id="65d02-111">Validate that the mail nickname is unique</span></span>

<span data-ttu-id="65d02-112">Этот API возвращает только первую обнаруженную ошибку проверки.</span><span class="sxs-lookup"><span data-stu-id="65d02-112">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="65d02-113">Если свойства не прошли несколько проверок, возвращается только первый сбой проверки.</span><span class="sxs-lookup"><span data-stu-id="65d02-113">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="65d02-114">Тем не менее, вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяется только политика именования префиксов и суффиксов.</span><span class="sxs-lookup"><span data-stu-id="65d02-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="65d02-115">Чтобы узнать больше о настройке политик именования, ознакомьтесь со статьей [Настройка политики именования](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span><span class="sxs-lookup"><span data-stu-id="65d02-115">To learn more about configuring naming policies, see [Configure naming policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="65d02-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65d02-116">Permissions</span></span>
<span data-ttu-id="65d02-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65d02-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65d02-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65d02-119">Permission type</span></span>      | <span data-ttu-id="65d02-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65d02-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65d02-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65d02-121">Delegated (work or school account)</span></span> | <span data-ttu-id="65d02-122">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65d02-122">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="65d02-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65d02-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65d02-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65d02-124">Not supported.</span></span>    |
|<span data-ttu-id="65d02-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65d02-125">Application</span></span> | <span data-ttu-id="65d02-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65d02-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65d02-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65d02-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="65d02-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65d02-128">Request headers</span></span>

| <span data-ttu-id="65d02-129">Имя</span><span class="sxs-lookup"><span data-stu-id="65d02-129">Name</span></span>           | <span data-ttu-id="65d02-130">Описание</span><span class="sxs-lookup"><span data-stu-id="65d02-130">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="65d02-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65d02-131">Authorization</span></span>  | <span data-ttu-id="65d02-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65d02-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="65d02-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65d02-134">Content-Type</span></span>   | <span data-ttu-id="65d02-135">application/json</span><span class="sxs-lookup"><span data-stu-id="65d02-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="65d02-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65d02-136">Request body</span></span>
<span data-ttu-id="65d02-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="65d02-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="65d02-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="65d02-138">Parameter</span></span>    | <span data-ttu-id="65d02-139">Тип</span><span class="sxs-lookup"><span data-stu-id="65d02-139">Type</span></span>   |<span data-ttu-id="65d02-140">Описание</span><span class="sxs-lookup"><span data-stu-id="65d02-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65d02-141">Сущности</span><span class="sxs-lookup"><span data-stu-id="65d02-141">entityType</span></span>|<span data-ttu-id="65d02-142">String</span><span class="sxs-lookup"><span data-stu-id="65d02-142">String</span></span>| <span data-ttu-id="65d02-143">Group — единственный поддерживаемый тип объекта.</span><span class="sxs-lookup"><span data-stu-id="65d02-143">Group is the only supported entity type.</span></span> |
|<span data-ttu-id="65d02-144">displayName</span><span class="sxs-lookup"><span data-stu-id="65d02-144">displayName</span></span>|<span data-ttu-id="65d02-145">Строка</span><span class="sxs-lookup"><span data-stu-id="65d02-145">String</span></span>| <span data-ttu-id="65d02-146">Отображаемое имя группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="65d02-146">The display name of the group to validate.</span></span> <span data-ttu-id="65d02-147">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="65d02-147">The property is not individually required.</span></span> <span data-ttu-id="65d02-148">Однако необходимо указать по крайней мере одно свойство (**DisplayName** или **mailNickname**).</span><span class="sxs-lookup"><span data-stu-id="65d02-148">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="65d02-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="65d02-149">mailNickname</span></span>|<span data-ttu-id="65d02-150">String</span><span class="sxs-lookup"><span data-stu-id="65d02-150">String</span></span>| <span data-ttu-id="65d02-151">Псевдоним почты для группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="65d02-151">The mail nickname of the group to validate.</span></span> <span data-ttu-id="65d02-152">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="65d02-152">The property is not individually required.</span></span> <span data-ttu-id="65d02-153">Однако необходимо указать по крайней мере одно свойство (**DisplayName** или **mailNickname**).</span><span class="sxs-lookup"><span data-stu-id="65d02-153">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="65d02-154">онбехалфофусерид</span><span class="sxs-lookup"><span data-stu-id="65d02-154">onBehalfOfUserId</span></span>|<span data-ttu-id="65d02-155">GUID</span><span class="sxs-lookup"><span data-stu-id="65d02-155">Guid</span></span>| <span data-ttu-id="65d02-156">Идентификатор пользователя, который олицетворяет при вызове API.</span><span class="sxs-lookup"><span data-stu-id="65d02-156">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="65d02-157">Результаты проверки предназначены для атрибутов и ролей **онбехалфофусерид** .</span><span class="sxs-lookup"><span data-stu-id="65d02-157">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="65d02-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="65d02-158">Response</span></span>

<span data-ttu-id="65d02-159">При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="65d02-159">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="65d02-160">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="65d02-160">It does not return anything in the response body.</span></span>

<span data-ttu-id="65d02-161">Если запрос является недопустимым, метод возвращает `400 Bad Request` код отклика.</span><span class="sxs-lookup"><span data-stu-id="65d02-161">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="65d02-162">В тексте отклика возвращается сообщение об ошибке со сведениями о недопустимом запросе.</span><span class="sxs-lookup"><span data-stu-id="65d02-162">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="65d02-163">При возникновении ошибки проверки метод возвращает `422 Unprocessable Entity` код отклика.</span><span class="sxs-lookup"><span data-stu-id="65d02-163">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="65d02-164">В тексте отклика возвращается сообщение об ошибке и коллекция сведений об ошибке.</span><span class="sxs-lookup"><span data-stu-id="65d02-164">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65d02-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="65d02-165">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="65d02-166">Пример 1: успешный запрос на проверку</span><span class="sxs-lookup"><span data-stu-id="65d02-166">Example 1: Successful validation request</span></span>
<span data-ttu-id="65d02-167">В этом примере показан успешный запрос на проверку.</span><span class="sxs-lookup"><span data-stu-id="65d02-167">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="65d02-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="65d02-168">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="65d02-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="65d02-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="65d02-170">C#</span><span class="sxs-lookup"><span data-stu-id="65d02-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65d02-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65d02-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65d02-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65d02-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65d02-173">Java</span><span class="sxs-lookup"><span data-stu-id="65d02-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65d02-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="65d02-174">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="65d02-175">Пример 2: запрос с ошибками проверки</span><span class="sxs-lookup"><span data-stu-id="65d02-175">Example 2: Request with validation errors</span></span>
<span data-ttu-id="65d02-176">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="65d02-176">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="65d02-177">Запросить</span><span class="sxs-lookup"><span data-stu-id="65d02-177">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

#### <a name="response"></a><span data-ttu-id="65d02-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="65d02-178">Response</span></span>
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

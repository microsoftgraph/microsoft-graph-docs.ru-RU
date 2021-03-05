---
title: 'directoryObject: проверка Свойств'
description: Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 41734da2f35e364df34088d220fdd54e287c2926
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448571"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="c9244-103">directoryObject: проверка Свойств</span><span class="sxs-lookup"><span data-stu-id="c9244-103">directoryObject: validateProperties</span></span>

<span data-ttu-id="c9244-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9244-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c9244-105">Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="c9244-105">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="c9244-106">Клиенты могут использовать этот API, чтобы определить, допустимо [](group-post-groups.md) ли имя или псевдоним почты перед попыткой создать группу Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c9244-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [create](group-post-groups.md) a Microsoft 365 group.</span></span> <span data-ttu-id="c9244-107">Чтобы проверить свойства существующей группы, используйте функцию [группы: validateProperties.](group-validateproperties.md)</span><span class="sxs-lookup"><span data-stu-id="c9244-107">To validate the properties of an existing group, use the [group: validateProperties](group-validateproperties.md) function.</span></span>

<span data-ttu-id="c9244-108">Для свойств отображаемого имени и ником почты выполняются следующие проверки политики:</span><span class="sxs-lookup"><span data-stu-id="c9244-108">The following policy validations are performed for the display name and mail nickname properties:</span></span>
1. <span data-ttu-id="c9244-109">Проверка политики имен префикса и суффикса</span><span class="sxs-lookup"><span data-stu-id="c9244-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="c9244-110">Проверка настраиваемой политики запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="c9244-110">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="c9244-111">Проверка уникальности псевдонима почты</span><span class="sxs-lookup"><span data-stu-id="c9244-111">Validate that the mail nickname is unique</span></span>

<span data-ttu-id="c9244-112">Этот API возвращает только первый сбой проверки, с которым столкнулся.</span><span class="sxs-lookup"><span data-stu-id="c9244-112">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="c9244-113">Если свойства не удается несколько проверки, возвращается только первая ошибка проверки.</span><span class="sxs-lookup"><span data-stu-id="c9244-113">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="c9244-114">Однако вы можете проверить как имя почты, так и имя дисплея и получить коллекцию ошибок проверки, если вы только проверяете политику именования префикса и суффикса.</span><span class="sxs-lookup"><span data-stu-id="c9244-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="c9244-115">Дополнительные новости о настройке политик имен см. в дополнительных подробной информации о политике [настройки имен.](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell)</span><span class="sxs-lookup"><span data-stu-id="c9244-115">To learn more about configuring naming policies, see [Configure naming policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="c9244-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9244-116">Permissions</span></span>
<span data-ttu-id="c9244-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9244-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9244-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9244-119">Permission type</span></span>      | <span data-ttu-id="c9244-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9244-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9244-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9244-121">Delegated (work or school account)</span></span> | <span data-ttu-id="c9244-122">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c9244-122">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c9244-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9244-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9244-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9244-124">Not supported.</span></span>    |
|<span data-ttu-id="c9244-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9244-125">Application</span></span> | <span data-ttu-id="c9244-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9244-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9244-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9244-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="c9244-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9244-128">Request headers</span></span>

| <span data-ttu-id="c9244-129">Имя</span><span class="sxs-lookup"><span data-stu-id="c9244-129">Name</span></span>           | <span data-ttu-id="c9244-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c9244-130">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="c9244-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9244-131">Authorization</span></span>  | <span data-ttu-id="c9244-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9244-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="c9244-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c9244-134">Content-Type</span></span>   | <span data-ttu-id="c9244-135">application/json</span><span class="sxs-lookup"><span data-stu-id="c9244-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9244-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9244-136">Request body</span></span>
<span data-ttu-id="c9244-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c9244-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c9244-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="c9244-138">Parameter</span></span>    | <span data-ttu-id="c9244-139">Тип</span><span class="sxs-lookup"><span data-stu-id="c9244-139">Type</span></span>   |<span data-ttu-id="c9244-140">Описание</span><span class="sxs-lookup"><span data-stu-id="c9244-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9244-141">entityType</span><span class="sxs-lookup"><span data-stu-id="c9244-141">entityType</span></span>|<span data-ttu-id="c9244-142">String</span><span class="sxs-lookup"><span data-stu-id="c9244-142">String</span></span>| <span data-ttu-id="c9244-143">Группа — это единственный поддерживаемый тип сущности.</span><span class="sxs-lookup"><span data-stu-id="c9244-143">Group is the only supported entity type.</span></span> |
|<span data-ttu-id="c9244-144">displayName</span><span class="sxs-lookup"><span data-stu-id="c9244-144">displayName</span></span>|<span data-ttu-id="c9244-145">String</span><span class="sxs-lookup"><span data-stu-id="c9244-145">String</span></span>| <span data-ttu-id="c9244-146">Отображаемого имени группы для проверки.</span><span class="sxs-lookup"><span data-stu-id="c9244-146">The display name of the group to validate.</span></span> <span data-ttu-id="c9244-147">Свойство не требуется по отдельности.</span><span class="sxs-lookup"><span data-stu-id="c9244-147">The property is not individually required.</span></span> <span data-ttu-id="c9244-148">Однако требуется по крайней мере одно свойство **(displayName** или **mailNickname).**</span><span class="sxs-lookup"><span data-stu-id="c9244-148">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="c9244-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c9244-149">mailNickname</span></span>|<span data-ttu-id="c9244-150">String</span><span class="sxs-lookup"><span data-stu-id="c9244-150">String</span></span>| <span data-ttu-id="c9244-151">Имя почты группы для проверки.</span><span class="sxs-lookup"><span data-stu-id="c9244-151">The mail nickname of the group to validate.</span></span> <span data-ttu-id="c9244-152">Свойство не требуется по отдельности.</span><span class="sxs-lookup"><span data-stu-id="c9244-152">The property is not individually required.</span></span> <span data-ttu-id="c9244-153">Однако требуется по крайней мере одно свойство **(displayName** или **mailNickname).**</span><span class="sxs-lookup"><span data-stu-id="c9244-153">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="c9244-154">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="c9244-154">onBehalfOfUserId</span></span>|<span data-ttu-id="c9244-155">Guid</span><span class="sxs-lookup"><span data-stu-id="c9244-155">Guid</span></span>| <span data-ttu-id="c9244-156">ID пользователя, который должен выдать себя при вызове API.</span><span class="sxs-lookup"><span data-stu-id="c9244-156">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="c9244-157">Результаты проверки для **атрибутов и ролей onBehalfOfUserId.**</span><span class="sxs-lookup"><span data-stu-id="c9244-157">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="c9244-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9244-158">Response</span></span>

<span data-ttu-id="c9244-159">В случае успешной проверки и без ошибок проверки метод возвращает `204 No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="c9244-159">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="c9244-160">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c9244-160">It does not return anything in the response body.</span></span>

<span data-ttu-id="c9244-161">Если запрос недействителен, метод возвращает `400 Bad Request` код ответа.</span><span class="sxs-lookup"><span data-stu-id="c9244-161">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="c9244-162">Сообщение об ошибке с сведениями о недействительности запроса возвращается в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c9244-162">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="c9244-163">При ошибке проверки метод возвращает `422 Unprocessable Entity` код ответа.</span><span class="sxs-lookup"><span data-stu-id="c9244-163">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="c9244-164">Сообщение об ошибке и коллекция сведений об ошибках возвращаются в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c9244-164">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9244-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="c9244-165">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="c9244-166">Пример 1. Успешный запрос на проверку</span><span class="sxs-lookup"><span data-stu-id="c9244-166">Example 1: Successful validation request</span></span>
<span data-ttu-id="c9244-167">Это пример успешного запроса на проверку.</span><span class="sxs-lookup"><span data-stu-id="c9244-167">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="c9244-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9244-168">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c9244-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9244-169">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c9244-170">C#</span><span class="sxs-lookup"><span data-stu-id="c9244-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9244-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9244-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9244-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9244-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9244-173">Java</span><span class="sxs-lookup"><span data-stu-id="c9244-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c9244-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9244-174">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="c9244-175">Пример 2. Запрос с ошибками проверки</span><span class="sxs-lookup"><span data-stu-id="c9244-175">Example 2: Request with validation errors</span></span>
<span data-ttu-id="c9244-176">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="c9244-176">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="c9244-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9244-177">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="c9244-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9244-178">Response</span></span>
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


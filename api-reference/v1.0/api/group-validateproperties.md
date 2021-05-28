---
title: 'группа: проверкаProperties'
description: Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a9d39c99e63607ded7ecaa194c7002f32cf36890
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680530"
---
# <a name="group-validateproperties"></a><span data-ttu-id="01063-103">группа: проверкаProperties</span><span class="sxs-lookup"><span data-stu-id="01063-103">group: validateProperties</span></span>

<span data-ttu-id="01063-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01063-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="01063-105">Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="01063-105">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="01063-106">Клиенты могут использовать этот API, чтобы определить, допустимо [](group-update.md) ли имя или псевдоним почты перед обновлением Microsoft 365 группы.</span><span class="sxs-lookup"><span data-stu-id="01063-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [update](group-update.md) a Microsoft 365 group.</span></span> <span data-ttu-id="01063-107">Чтобы проверить свойства перед созданием группы, используйте функцию [directoryobject:validateProperties.](directoryobject-validateproperties.md)</span><span class="sxs-lookup"><span data-stu-id="01063-107">To validate the properties before creating a group, use the [directoryobject:validateProperties](directoryobject-validateproperties.md) function.</span></span>

<span data-ttu-id="01063-108">Для свойств отображаемого имени и ником почты выполняются следующие проверки политики:</span><span class="sxs-lookup"><span data-stu-id="01063-108">The following policy validations are performed for the display name and mail nickname properties:</span></span>
1. <span data-ttu-id="01063-109">Проверка политики имен префикса и суффикса</span><span class="sxs-lookup"><span data-stu-id="01063-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="01063-110">Проверка настраиваемой политики запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="01063-110">Validate the custom banned words policy</span></span>

<span data-ttu-id="01063-111">Этот API возвращает только первый сбой проверки, с которым столкнулся.</span><span class="sxs-lookup"><span data-stu-id="01063-111">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="01063-112">Если свойства не удается несколько проверки, возвращается только первая ошибка проверки.</span><span class="sxs-lookup"><span data-stu-id="01063-112">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="01063-113">Однако вы можете проверить как имя почты, так и имя дисплея и получить коллекцию ошибок проверки, если вы только проверяете политику именования префикса и суффикса.</span><span class="sxs-lookup"><span data-stu-id="01063-113">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="01063-114">Дополнительные новости о настройке политик имен см. в дополнительных подробной информации о политике [настройки имен.](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell)</span><span class="sxs-lookup"><span data-stu-id="01063-114">To learn more about configuring naming policies, see [Configure naming policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="01063-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01063-115">Permissions</span></span>

<span data-ttu-id="01063-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01063-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01063-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01063-118">Permission type</span></span>      | <span data-ttu-id="01063-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01063-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01063-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01063-120">Delegated (work or school account)</span></span> | <span data-ttu-id="01063-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01063-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="01063-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01063-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01063-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01063-123">Not supported.</span></span>    |
|<span data-ttu-id="01063-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01063-124">Application</span></span> | <span data-ttu-id="01063-125">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01063-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01063-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01063-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="01063-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01063-127">Request headers</span></span>

| <span data-ttu-id="01063-128">Имя</span><span class="sxs-lookup"><span data-stu-id="01063-128">Name</span></span>           | <span data-ttu-id="01063-129">Описание</span><span class="sxs-lookup"><span data-stu-id="01063-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="01063-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01063-130">Authorization</span></span>  | <span data-ttu-id="01063-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01063-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="01063-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01063-133">Content-Type</span></span>   | <span data-ttu-id="01063-134">application/json</span><span class="sxs-lookup"><span data-stu-id="01063-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="01063-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01063-135">Request body</span></span>

<span data-ttu-id="01063-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="01063-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="01063-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="01063-137">Parameter</span></span>    | <span data-ttu-id="01063-138">Тип</span><span class="sxs-lookup"><span data-stu-id="01063-138">Type</span></span>   |<span data-ttu-id="01063-139">Описание</span><span class="sxs-lookup"><span data-stu-id="01063-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01063-140">displayName</span><span class="sxs-lookup"><span data-stu-id="01063-140">displayName</span></span>|<span data-ttu-id="01063-141">String</span><span class="sxs-lookup"><span data-stu-id="01063-141">String</span></span>| <span data-ttu-id="01063-142">Отображаемого имени группы для проверки.</span><span class="sxs-lookup"><span data-stu-id="01063-142">The display name of the group to validate.</span></span> <span data-ttu-id="01063-143">Свойство не требуется по отдельности.</span><span class="sxs-lookup"><span data-stu-id="01063-143">The property is not individually required.</span></span> <span data-ttu-id="01063-144">Однако требуется по крайней мере одно свойство **(displayName** или **mailNickname).**</span><span class="sxs-lookup"><span data-stu-id="01063-144">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="01063-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="01063-145">mailNickname</span></span>|<span data-ttu-id="01063-146">String</span><span class="sxs-lookup"><span data-stu-id="01063-146">String</span></span>| <span data-ttu-id="01063-147">Имя почты группы для проверки.</span><span class="sxs-lookup"><span data-stu-id="01063-147">The mail nickname of the group to validate.</span></span> <span data-ttu-id="01063-148">Свойство не требуется по отдельности.</span><span class="sxs-lookup"><span data-stu-id="01063-148">The property is not individually required.</span></span> <span data-ttu-id="01063-149">Однако требуется по крайней мере одно свойство **(displayName** или **mailNickname).**</span><span class="sxs-lookup"><span data-stu-id="01063-149">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="01063-150">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="01063-150">onBehalfOfUserId</span></span>|<span data-ttu-id="01063-151">Guid</span><span class="sxs-lookup"><span data-stu-id="01063-151">Guid</span></span>| <span data-ttu-id="01063-152">ID пользователя, который должен выдать себя при вызове API.</span><span class="sxs-lookup"><span data-stu-id="01063-152">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="01063-153">Результаты проверки для **атрибутов и ролей onBehalfOfUserId.**</span><span class="sxs-lookup"><span data-stu-id="01063-153">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="01063-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="01063-154">Response</span></span>
<span data-ttu-id="01063-155">В случае успешной проверки и без ошибок проверки метод возвращает `204 No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="01063-155">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="01063-156">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01063-156">It does not return anything in the response body.</span></span>

<span data-ttu-id="01063-157">Если запрос недействителен, метод возвращает `400 Bad Request` код ответа.</span><span class="sxs-lookup"><span data-stu-id="01063-157">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="01063-158">Сообщение об ошибке с сведениями о недействительности запроса возвращается в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="01063-158">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="01063-159">При ошибке проверки.</span><span class="sxs-lookup"><span data-stu-id="01063-159">If there is a validation error.</span></span> <span data-ttu-id="01063-160">Метод возвращает код `422 Unprocessable Entity` ответа.</span><span class="sxs-lookup"><span data-stu-id="01063-160">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="01063-161">Сообщение об ошибке и коллекция сведений об ошибках возвращаются в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="01063-161">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01063-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="01063-162">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="01063-163">Пример 1. Успешный запрос на проверку</span><span class="sxs-lookup"><span data-stu-id="01063-163">Example 1: Successful validation request</span></span>
<span data-ttu-id="01063-164">Это пример успешного запроса на проверку.</span><span class="sxs-lookup"><span data-stu-id="01063-164">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="01063-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="01063-165">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="01063-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="01063-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="01063-167">C#</span><span class="sxs-lookup"><span data-stu-id="01063-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01063-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01063-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01063-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01063-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01063-170">Java</span><span class="sxs-lookup"><span data-stu-id="01063-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="01063-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="01063-171">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="01063-172">Пример 2. Запрос с ошибками проверки</span><span class="sxs-lookup"><span data-stu-id="01063-172">Example 2: Request with validation errors</span></span>
<span data-ttu-id="01063-173">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="01063-173">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="01063-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="01063-174">Request</span></span>
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a><span data-ttu-id="01063-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="01063-175">Response</span></span>
```http
HTTP/1.1 422
Content-type: application/json
Content-length: 223

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "mailNickname",
        "code": "PropertyConflict",
        "message": "Another object with the same value for property mailNickname already exists."
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


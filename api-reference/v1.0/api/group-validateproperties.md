---
title: 'Группа: Валидатепропертиес'
description: Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 53705781c8e9465b06199ba3c7714d29a416ee47
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864721"
---
# <a name="group-validateproperties"></a><span data-ttu-id="70021-103">Группа: Валидатепропертиес</span><span class="sxs-lookup"><span data-stu-id="70021-103">group: validateProperties</span></span>

<span data-ttu-id="70021-104">Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="70021-104">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="70021-105">Клиенты могут использовать этот API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться [Обновить](group-update.md) группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="70021-105">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [update](group-update.md) an Office 365 group.</span></span> <span data-ttu-id="70021-106">Чтобы проверить свойства перед созданием группы, используйте функцию [directoryobject: валидатепропертиес](directoryobject-validateproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="70021-106">To validate the properties before creating a group, use the [directoryobject:validateProperties](directoryobject-validateproperties.md) function.</span></span>

<span data-ttu-id="70021-107">Для отображаемого имени и свойств псевдонима почты выполняются следующие проверки политик:</span><span class="sxs-lookup"><span data-stu-id="70021-107">The following policy validations are performed for the display name and mail nickname properties:</span></span>
1. <span data-ttu-id="70021-108">Проверка политики именования префиксов и суффиксов</span><span class="sxs-lookup"><span data-stu-id="70021-108">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="70021-109">Проверка политики нестандартных запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="70021-109">Validate the custom banned words policy</span></span>

<span data-ttu-id="70021-110">Этот API возвращает только первую обнаруженную ошибку проверки.</span><span class="sxs-lookup"><span data-stu-id="70021-110">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="70021-111">Если свойства не прошли несколько проверок, возвращается только первый сбой проверки.</span><span class="sxs-lookup"><span data-stu-id="70021-111">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="70021-112">Тем не менее, вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяется только политика именования префиксов и суффиксов.</span><span class="sxs-lookup"><span data-stu-id="70021-112">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="70021-113">Чтобы узнать больше о настройке политик именования, ознакомьтесь со статьей [Настройка политики именования](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span><span class="sxs-lookup"><span data-stu-id="70021-113">To learn more about configuring naming policies, see [Configure naming policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="70021-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70021-114">Permissions</span></span>

<span data-ttu-id="70021-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70021-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70021-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70021-117">Permission type</span></span>      | <span data-ttu-id="70021-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70021-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70021-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70021-119">Delegated (work or school account)</span></span> | <span data-ttu-id="70021-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70021-120">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="70021-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70021-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70021-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70021-122">Not supported.</span></span>    |
|<span data-ttu-id="70021-123">Приложение</span><span class="sxs-lookup"><span data-stu-id="70021-123">Application</span></span> | <span data-ttu-id="70021-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70021-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70021-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70021-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="70021-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70021-126">Request headers</span></span>

| <span data-ttu-id="70021-127">Имя</span><span class="sxs-lookup"><span data-stu-id="70021-127">Name</span></span>           | <span data-ttu-id="70021-128">Описание</span><span class="sxs-lookup"><span data-stu-id="70021-128">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="70021-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70021-129">Authorization</span></span>  | <span data-ttu-id="70021-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70021-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="70021-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70021-132">Content-Type</span></span>   | <span data-ttu-id="70021-133">application/json</span><span class="sxs-lookup"><span data-stu-id="70021-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="70021-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70021-134">Request body</span></span>

<span data-ttu-id="70021-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="70021-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="70021-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="70021-136">Parameter</span></span>    | <span data-ttu-id="70021-137">Тип</span><span class="sxs-lookup"><span data-stu-id="70021-137">Type</span></span>   |<span data-ttu-id="70021-138">Описание</span><span class="sxs-lookup"><span data-stu-id="70021-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70021-139">displayName</span><span class="sxs-lookup"><span data-stu-id="70021-139">displayName</span></span>|<span data-ttu-id="70021-140">Строка</span><span class="sxs-lookup"><span data-stu-id="70021-140">String</span></span>| <span data-ttu-id="70021-141">Отображаемое имя группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="70021-141">The display name of the group to validate.</span></span> <span data-ttu-id="70021-142">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="70021-142">The property is not individually required.</span></span> <span data-ttu-id="70021-143">Однако необходимо указать по крайней мере одно свойство (**DisplayName** или **mailNickname**).</span><span class="sxs-lookup"><span data-stu-id="70021-143">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="70021-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="70021-144">mailNickname</span></span>|<span data-ttu-id="70021-145">String</span><span class="sxs-lookup"><span data-stu-id="70021-145">String</span></span>| <span data-ttu-id="70021-146">Псевдоним почты для группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="70021-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="70021-147">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="70021-147">The property is not individually required.</span></span> <span data-ttu-id="70021-148">Однако необходимо указать по крайней мере одно свойство (**DisplayName** или **mailNickname**).</span><span class="sxs-lookup"><span data-stu-id="70021-148">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="70021-149">онбехалфофусерид</span><span class="sxs-lookup"><span data-stu-id="70021-149">onBehalfOfUserId</span></span>|<span data-ttu-id="70021-150">GUID</span><span class="sxs-lookup"><span data-stu-id="70021-150">Guid</span></span>| <span data-ttu-id="70021-151">Идентификатор пользователя, который олицетворяет при вызове API.</span><span class="sxs-lookup"><span data-stu-id="70021-151">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="70021-152">Результаты проверки предназначены для атрибутов и ролей **онбехалфофусерид** .</span><span class="sxs-lookup"><span data-stu-id="70021-152">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="70021-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="70021-153">Response</span></span>
<span data-ttu-id="70021-154">При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="70021-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="70021-155">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="70021-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="70021-156">Если запрос является недопустимым, метод возвращает `400 Bad Request` код отклика.</span><span class="sxs-lookup"><span data-stu-id="70021-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="70021-157">В тексте отклика возвращается сообщение об ошибке со сведениями о недопустимом запросе.</span><span class="sxs-lookup"><span data-stu-id="70021-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="70021-158">При возникновении ошибки проверки.</span><span class="sxs-lookup"><span data-stu-id="70021-158">If there is a validation error.</span></span> <span data-ttu-id="70021-159">Метод возвращает `422 Unprocessable Entity` код отклика.</span><span class="sxs-lookup"><span data-stu-id="70021-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="70021-160">В тексте отклика возвращается сообщение об ошибке и коллекция сведений об ошибке.</span><span class="sxs-lookup"><span data-stu-id="70021-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70021-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="70021-161">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="70021-162">Пример 1: успешный запрос на проверку</span><span class="sxs-lookup"><span data-stu-id="70021-162">Example 1: Successful validation request</span></span>
<span data-ttu-id="70021-163">В этом примере показан успешный запрос на проверку.</span><span class="sxs-lookup"><span data-stu-id="70021-163">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="70021-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="70021-164">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="70021-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="70021-165">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="70021-166">C#</span><span class="sxs-lookup"><span data-stu-id="70021-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70021-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70021-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70021-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70021-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="70021-169">Java</span><span class="sxs-lookup"><span data-stu-id="70021-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="70021-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="70021-170">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="70021-171">Пример 2: запрос с ошибками проверки</span><span class="sxs-lookup"><span data-stu-id="70021-171">Example 2: Request with validation errors</span></span>
<span data-ttu-id="70021-172">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="70021-172">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="70021-173">Запросить</span><span class="sxs-lookup"><span data-stu-id="70021-173">Request</span></span>
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a><span data-ttu-id="70021-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="70021-174">Response</span></span>
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

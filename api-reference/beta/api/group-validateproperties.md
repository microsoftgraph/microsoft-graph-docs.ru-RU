---
title: 'Группа: Валидатепропертиес'
description: Убедитесь, что отображаемое имя или псевдоним почты группы Office 365 соответствует политикам именования. Клиенты могут использовать API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **Обновить** группу Office 365. Для проверки свойств перед созданием группы используйте функцию Валидатепропертиес для объектов Directory.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ecf5be372cb00df26bf6ae14fdba933782040bc6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262806"
---
# <a name="group-validateproperties"></a><span data-ttu-id="5a37c-105">Группа: Валидатепропертиес</span><span class="sxs-lookup"><span data-stu-id="5a37c-105">group: validateProperties</span></span>

<span data-ttu-id="5a37c-106">Убедитесь, что отображаемое имя или псевдоним почты группы Office 365 соответствует политикам именования.</span><span class="sxs-lookup"><span data-stu-id="5a37c-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="5a37c-107">Клиенты могут использовать API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **Обновить** группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="5a37c-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="5a37c-108">Для проверки свойств перед созданием группы используйте [функцию валидатепропертиес](directoryobject-validateproperties.md) для объектов Directory.</span><span class="sxs-lookup"><span data-stu-id="5a37c-108">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="5a37c-109">Для отображаемого имени и свойств псевдонима почты выполняются следующие проверки.</span><span class="sxs-lookup"><span data-stu-id="5a37c-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="5a37c-110">Проверка политики именования префиксов и суффиксов</span><span class="sxs-lookup"><span data-stu-id="5a37c-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="5a37c-111">Проверка политики нестандартных запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="5a37c-111">Validate the custom banned words policy</span></span>

<span data-ttu-id="5a37c-112">Этот API возвращается при первом обнаружении ошибки.</span><span class="sxs-lookup"><span data-stu-id="5a37c-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="5a37c-113">Если одно или несколько свойств не прошли несколько проверок, возвращается только свойство с первой ошибкой проверки.</span><span class="sxs-lookup"><span data-stu-id="5a37c-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="5a37c-114">Тем не менее, вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяется только политика именования префиксов и суффиксов.</span><span class="sxs-lookup"><span data-stu-id="5a37c-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a37c-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a37c-115">Permissions</span></span>

<span data-ttu-id="5a37c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a37c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a37c-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a37c-118">Permission type</span></span>      | <span data-ttu-id="5a37c-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a37c-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a37c-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a37c-120">Delegated (work or school account)</span></span> | <span data-ttu-id="5a37c-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a37c-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5a37c-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a37c-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a37c-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a37c-123">Not supported.</span></span>    |
|<span data-ttu-id="5a37c-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a37c-124">Application</span></span> | <span data-ttu-id="5a37c-125">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a37c-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a37c-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a37c-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="5a37c-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a37c-127">Request headers</span></span>

| <span data-ttu-id="5a37c-128">Имя</span><span class="sxs-lookup"><span data-stu-id="5a37c-128">Name</span></span>           | <span data-ttu-id="5a37c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="5a37c-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="5a37c-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a37c-130">Authorization</span></span>  | <span data-ttu-id="5a37c-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5a37c-131">Bearer {code}</span></span>    |
| <span data-ttu-id="5a37c-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a37c-132">Content-Type</span></span>   | <span data-ttu-id="5a37c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="5a37c-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a37c-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5a37c-134">Request body</span></span>

<span data-ttu-id="5a37c-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5a37c-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5a37c-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="5a37c-136">Parameter</span></span>    | <span data-ttu-id="5a37c-137">Тип</span><span class="sxs-lookup"><span data-stu-id="5a37c-137">Type</span></span>   |<span data-ttu-id="5a37c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="5a37c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a37c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="5a37c-139">displayName</span></span>|<span data-ttu-id="5a37c-140">Строка</span><span class="sxs-lookup"><span data-stu-id="5a37c-140">String</span></span>| <span data-ttu-id="5a37c-141">Отображаемое имя группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="5a37c-141">The display name of the group to validate.</span></span> <span data-ttu-id="5a37c-142">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="5a37c-142">The property is not individually required.</span></span> <span data-ttu-id="5a37c-143">Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="5a37c-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="5a37c-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="5a37c-144">mailNickname</span></span>|<span data-ttu-id="5a37c-145">String</span><span class="sxs-lookup"><span data-stu-id="5a37c-145">String</span></span>| <span data-ttu-id="5a37c-146">Псевдоним почты для группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="5a37c-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="5a37c-147">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="5a37c-147">The property is not individually required.</span></span> <span data-ttu-id="5a37c-148">Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="5a37c-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="5a37c-149">Онбехалфофусерид</span><span class="sxs-lookup"><span data-stu-id="5a37c-149">onBehalfOfUserId</span></span>|<span data-ttu-id="5a37c-150">GUID</span><span class="sxs-lookup"><span data-stu-id="5a37c-150">Guid</span></span>| <span data-ttu-id="5a37c-151">Идентификатор объекта пользователя, который олицетворяет при вызове API.</span><span class="sxs-lookup"><span data-stu-id="5a37c-151">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="5a37c-152">Результаты проверки предназначены для атрибутов и ролей Онбехалфофусерид.</span><span class="sxs-lookup"><span data-stu-id="5a37c-152">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="5a37c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a37c-153">Response</span></span>
<span data-ttu-id="5a37c-154">При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="5a37c-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="5a37c-155">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5a37c-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="5a37c-156">Если запрос является недопустимым, метод возвращает `400 Bad Request` код отклика.</span><span class="sxs-lookup"><span data-stu-id="5a37c-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="5a37c-157">В тексте отклика возвращается сообщение об ошибке со сведениями о недопустимом запросе.</span><span class="sxs-lookup"><span data-stu-id="5a37c-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="5a37c-158">При возникновении ошибки проверки.</span><span class="sxs-lookup"><span data-stu-id="5a37c-158">If there is a validation error.</span></span> <span data-ttu-id="5a37c-159">Метод возвращает `422 Unprocessable Entity` код отклика.</span><span class="sxs-lookup"><span data-stu-id="5a37c-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="5a37c-160">В тексте отклика возвращается сообщение об ошибке и коллекция сведений об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5a37c-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5a37c-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="5a37c-161">Examples</span></span>

<span data-ttu-id="5a37c-162">В этом примере показан успешный запрос на проверку.</span><span class="sxs-lookup"><span data-stu-id="5a37c-162">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="5a37c-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a37c-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="5a37c-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a37c-164">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5a37c-165">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5a37c-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5a37c-166">C#</span><span class="sxs-lookup"><span data-stu-id="5a37c-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_validateproperties-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a37c-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="5a37c-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_validateproperties-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5a37c-168">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5a37c-168">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_validateproperties-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="5a37c-169">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="5a37c-169">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="5a37c-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a37c-170">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="5a37c-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a37c-171">Response</span></span>
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
    "Error: /api-reference/beta/api/group-validateproperties.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-validateproperties.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-validateproperties.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

---
title: 'Группа: Валидатепропертиес'
description: Убедитесь, что отображаемое имя или псевдоним почты группы Office 365 соответствует политикам именования. Клиенты могут использовать API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **Обновить** группу Office 365. Для проверки свойств перед созданием группы используйте функцию Валидатепропертиес для объектов Directory.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: cb0d6ca17a7c6bb9d48919235dfc8c3a9cec1059
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446676"
---
# <a name="group-validateproperties"></a><span data-ttu-id="3ba64-105">Группа: Валидатепропертиес</span><span class="sxs-lookup"><span data-stu-id="3ba64-105">group: validateProperties</span></span>

<span data-ttu-id="3ba64-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3ba64-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ba64-107">Убедитесь, что отображаемое имя или псевдоним почты группы Office 365 соответствует политикам именования.</span><span class="sxs-lookup"><span data-stu-id="3ba64-107">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="3ba64-108">Клиенты могут использовать API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **Обновить** группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="3ba64-108">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="3ba64-109">Для проверки свойств перед созданием группы используйте [функцию валидатепропертиес](directoryobject-validateproperties.md) для объектов Directory.</span><span class="sxs-lookup"><span data-stu-id="3ba64-109">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="3ba64-110">Для отображаемого имени и свойств псевдонима почты выполняются следующие проверки.</span><span class="sxs-lookup"><span data-stu-id="3ba64-110">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="3ba64-111">Проверка политики именования префиксов и суффиксов</span><span class="sxs-lookup"><span data-stu-id="3ba64-111">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="3ba64-112">Проверка политики нестандартных запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="3ba64-112">Validate the custom banned words policy</span></span>

<span data-ttu-id="3ba64-113">Этот API возвращается при первом обнаружении ошибки.</span><span class="sxs-lookup"><span data-stu-id="3ba64-113">This API returns with the first failure encountered.</span></span> <span data-ttu-id="3ba64-114">Если одно или несколько свойств не прошли несколько проверок, возвращается только свойство с первой ошибкой проверки.</span><span class="sxs-lookup"><span data-stu-id="3ba64-114">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="3ba64-115">Тем не менее, вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяется только политика именования префиксов и суффиксов.</span><span class="sxs-lookup"><span data-stu-id="3ba64-115">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ba64-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ba64-116">Permissions</span></span>

<span data-ttu-id="3ba64-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ba64-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ba64-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ba64-119">Permission type</span></span>      | <span data-ttu-id="3ba64-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ba64-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ba64-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ba64-121">Delegated (work or school account)</span></span> | <span data-ttu-id="3ba64-122">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ba64-122">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3ba64-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ba64-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ba64-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ba64-124">Not supported.</span></span>    |
|<span data-ttu-id="3ba64-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ba64-125">Application</span></span> | <span data-ttu-id="3ba64-126">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ba64-126">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ba64-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ba64-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="3ba64-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ba64-128">Request headers</span></span>

| <span data-ttu-id="3ba64-129">Имя</span><span class="sxs-lookup"><span data-stu-id="3ba64-129">Name</span></span>           | <span data-ttu-id="3ba64-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3ba64-130">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="3ba64-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ba64-131">Authorization</span></span>  | <span data-ttu-id="3ba64-132">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3ba64-132">Bearer {code}</span></span>    |
| <span data-ttu-id="3ba64-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ba64-133">Content-Type</span></span>   | <span data-ttu-id="3ba64-134">application/json</span><span class="sxs-lookup"><span data-stu-id="3ba64-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ba64-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ba64-135">Request body</span></span>

<span data-ttu-id="3ba64-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3ba64-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3ba64-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="3ba64-137">Parameter</span></span>    | <span data-ttu-id="3ba64-138">Тип</span><span class="sxs-lookup"><span data-stu-id="3ba64-138">Type</span></span>   |<span data-ttu-id="3ba64-139">Описание</span><span class="sxs-lookup"><span data-stu-id="3ba64-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ba64-140">displayName</span><span class="sxs-lookup"><span data-stu-id="3ba64-140">displayName</span></span>|<span data-ttu-id="3ba64-141">Строка</span><span class="sxs-lookup"><span data-stu-id="3ba64-141">String</span></span>| <span data-ttu-id="3ba64-142">Отображаемое имя группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="3ba64-142">The display name of the group to validate.</span></span> <span data-ttu-id="3ba64-143">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="3ba64-143">The property is not individually required.</span></span> <span data-ttu-id="3ba64-144">Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="3ba64-144">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="3ba64-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="3ba64-145">mailNickname</span></span>|<span data-ttu-id="3ba64-146">String</span><span class="sxs-lookup"><span data-stu-id="3ba64-146">String</span></span>| <span data-ttu-id="3ba64-147">Псевдоним почты для группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="3ba64-147">The mail nickname of the group to validate.</span></span> <span data-ttu-id="3ba64-148">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="3ba64-148">The property is not individually required.</span></span> <span data-ttu-id="3ba64-149">Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="3ba64-149">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="3ba64-150">онбехалфофусерид</span><span class="sxs-lookup"><span data-stu-id="3ba64-150">onBehalfOfUserId</span></span>|<span data-ttu-id="3ba64-151">GUID</span><span class="sxs-lookup"><span data-stu-id="3ba64-151">Guid</span></span>| <span data-ttu-id="3ba64-152">Идентификатор объекта пользователя, который олицетворяет при вызове API.</span><span class="sxs-lookup"><span data-stu-id="3ba64-152">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="3ba64-153">Результаты проверки предназначены для атрибутов и ролей Онбехалфофусерид.</span><span class="sxs-lookup"><span data-stu-id="3ba64-153">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="3ba64-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ba64-154">Response</span></span>
<span data-ttu-id="3ba64-155">При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="3ba64-155">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="3ba64-156">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3ba64-156">It does not return anything in the response body.</span></span>

<span data-ttu-id="3ba64-157">Если запрос является недопустимым, метод возвращает `400 Bad Request` код отклика.</span><span class="sxs-lookup"><span data-stu-id="3ba64-157">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="3ba64-158">В тексте отклика возвращается сообщение об ошибке со сведениями о недопустимом запросе.</span><span class="sxs-lookup"><span data-stu-id="3ba64-158">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="3ba64-159">При возникновении ошибки проверки.</span><span class="sxs-lookup"><span data-stu-id="3ba64-159">If there is a validation error.</span></span> <span data-ttu-id="3ba64-160">Метод возвращает `422 Unprocessable Entity` код отклика.</span><span class="sxs-lookup"><span data-stu-id="3ba64-160">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="3ba64-161">В тексте отклика возвращается сообщение об ошибке и коллекция сведений об ошибке.</span><span class="sxs-lookup"><span data-stu-id="3ba64-161">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ba64-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="3ba64-162">Examples</span></span>

<span data-ttu-id="3ba64-163">В этом примере показан успешный запрос на проверку.</span><span class="sxs-lookup"><span data-stu-id="3ba64-163">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="3ba64-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ba64-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3ba64-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ba64-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3ba64-166">C#</span><span class="sxs-lookup"><span data-stu-id="3ba64-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ba64-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ba64-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ba64-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ba64-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3ba64-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ba64-169">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="3ba64-170">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="3ba64-170">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="3ba64-171">Запросить</span><span class="sxs-lookup"><span data-stu-id="3ba64-171">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="3ba64-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ba64-172">Response</span></span>
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

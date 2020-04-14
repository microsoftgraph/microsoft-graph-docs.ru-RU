---
title: 'Группа: Валидатепропертиес'
description: Убедитесь, что отображаемое имя или псевдоним почты группы Office 365 соответствует политикам именования.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b77ccc5fc22ffa9a0829d825a434b32070701a0b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396020"
---
# <a name="group-validateproperties"></a><span data-ttu-id="95b1c-103">Группа: Валидатепропертиес</span><span class="sxs-lookup"><span data-stu-id="95b1c-103">group: validateProperties</span></span>

<span data-ttu-id="95b1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95b1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95b1c-105">Убедитесь, что отображаемое имя или псевдоним почты группы Office 365 соответствует политикам именования.</span><span class="sxs-lookup"><span data-stu-id="95b1c-105">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="95b1c-106">Клиенты могут использовать API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **Обновить** группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="95b1c-106">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="95b1c-107">Для проверки свойств перед созданием группы используйте [функцию валидатепропертиес](directoryobject-validateproperties.md) для объектов Directory.</span><span class="sxs-lookup"><span data-stu-id="95b1c-107">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="95b1c-108">Для отображаемого имени и свойств псевдонима почты выполняются следующие проверки.</span><span class="sxs-lookup"><span data-stu-id="95b1c-108">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="95b1c-109">Проверка политики именования префиксов и суффиксов</span><span class="sxs-lookup"><span data-stu-id="95b1c-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="95b1c-110">Проверка политики нестандартных запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="95b1c-110">Validate the custom banned words policy</span></span>

<span data-ttu-id="95b1c-111">Этот API возвращается при первом обнаружении ошибки.</span><span class="sxs-lookup"><span data-stu-id="95b1c-111">This API returns with the first failure encountered.</span></span> <span data-ttu-id="95b1c-112">Если одно или несколько свойств не прошли несколько проверок, возвращается только свойство с первой ошибкой проверки.</span><span class="sxs-lookup"><span data-stu-id="95b1c-112">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="95b1c-113">Тем не менее, вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяется только политика именования префиксов и суффиксов.</span><span class="sxs-lookup"><span data-stu-id="95b1c-113">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="95b1c-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95b1c-114">Permissions</span></span>

<span data-ttu-id="95b1c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95b1c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95b1c-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95b1c-117">Permission type</span></span>      | <span data-ttu-id="95b1c-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95b1c-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95b1c-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95b1c-119">Delegated (work or school account)</span></span> | <span data-ttu-id="95b1c-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b1c-120">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="95b1c-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95b1c-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95b1c-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95b1c-122">Not supported.</span></span>    |
|<span data-ttu-id="95b1c-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95b1c-123">Application</span></span> | <span data-ttu-id="95b1c-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b1c-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95b1c-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95b1c-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="95b1c-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95b1c-126">Request headers</span></span>

| <span data-ttu-id="95b1c-127">Имя</span><span class="sxs-lookup"><span data-stu-id="95b1c-127">Name</span></span>           | <span data-ttu-id="95b1c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="95b1c-128">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="95b1c-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95b1c-129">Authorization</span></span>  | <span data-ttu-id="95b1c-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="95b1c-130">Bearer {code}</span></span>    |
| <span data-ttu-id="95b1c-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95b1c-131">Content-Type</span></span>   | <span data-ttu-id="95b1c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="95b1c-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="95b1c-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95b1c-133">Request body</span></span>

<span data-ttu-id="95b1c-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="95b1c-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="95b1c-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="95b1c-135">Parameter</span></span>    | <span data-ttu-id="95b1c-136">Тип</span><span class="sxs-lookup"><span data-stu-id="95b1c-136">Type</span></span>   |<span data-ttu-id="95b1c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="95b1c-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95b1c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="95b1c-138">displayName</span></span>|<span data-ttu-id="95b1c-139">Строка</span><span class="sxs-lookup"><span data-stu-id="95b1c-139">String</span></span>| <span data-ttu-id="95b1c-140">Отображаемое имя группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="95b1c-140">The display name of the group to validate.</span></span> <span data-ttu-id="95b1c-141">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="95b1c-141">The property is not individually required.</span></span> <span data-ttu-id="95b1c-142">Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="95b1c-142">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="95b1c-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="95b1c-143">mailNickname</span></span>|<span data-ttu-id="95b1c-144">String</span><span class="sxs-lookup"><span data-stu-id="95b1c-144">String</span></span>| <span data-ttu-id="95b1c-145">Псевдоним почты для группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="95b1c-145">The mail nickname of the group to validate.</span></span> <span data-ttu-id="95b1c-146">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="95b1c-146">The property is not individually required.</span></span> <span data-ttu-id="95b1c-147">Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="95b1c-147">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="95b1c-148">онбехалфофусерид</span><span class="sxs-lookup"><span data-stu-id="95b1c-148">onBehalfOfUserId</span></span>|<span data-ttu-id="95b1c-149">GUID</span><span class="sxs-lookup"><span data-stu-id="95b1c-149">Guid</span></span>| <span data-ttu-id="95b1c-150">Идентификатор объекта пользователя, который олицетворяет при вызове API.</span><span class="sxs-lookup"><span data-stu-id="95b1c-150">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="95b1c-151">Результаты проверки предназначены для атрибутов и ролей Онбехалфофусерид.</span><span class="sxs-lookup"><span data-stu-id="95b1c-151">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="95b1c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="95b1c-152">Response</span></span>
<span data-ttu-id="95b1c-153">При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="95b1c-153">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="95b1c-154">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="95b1c-154">It does not return anything in the response body.</span></span>

<span data-ttu-id="95b1c-155">Если запрос является недопустимым, метод возвращает `400 Bad Request` код отклика.</span><span class="sxs-lookup"><span data-stu-id="95b1c-155">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="95b1c-156">В тексте отклика возвращается сообщение об ошибке со сведениями о недопустимом запросе.</span><span class="sxs-lookup"><span data-stu-id="95b1c-156">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="95b1c-157">При возникновении ошибки проверки.</span><span class="sxs-lookup"><span data-stu-id="95b1c-157">If there is a validation error.</span></span> <span data-ttu-id="95b1c-158">Метод возвращает `422 Unprocessable Entity` код отклика.</span><span class="sxs-lookup"><span data-stu-id="95b1c-158">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="95b1c-159">В тексте отклика возвращается сообщение об ошибке и коллекция сведений об ошибке.</span><span class="sxs-lookup"><span data-stu-id="95b1c-159">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="95b1c-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="95b1c-160">Examples</span></span>

<span data-ttu-id="95b1c-161">В этом примере показан успешный запрос на проверку.</span><span class="sxs-lookup"><span data-stu-id="95b1c-161">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="95b1c-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="95b1c-162">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="95b1c-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="95b1c-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="95b1c-164">C#</span><span class="sxs-lookup"><span data-stu-id="95b1c-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95b1c-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95b1c-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95b1c-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95b1c-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="95b1c-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="95b1c-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="95b1c-168">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="95b1c-168">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="95b1c-169">Запросить</span><span class="sxs-lookup"><span data-stu-id="95b1c-169">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="95b1c-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="95b1c-170">Response</span></span>
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

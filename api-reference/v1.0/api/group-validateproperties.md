---
title: 'Группа: Валидатепропертиес'
description: Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5b245c242f0c34f2aaf89a3a4987700ae4eaa532
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124660"
---
# <a name="group-validateproperties"></a><span data-ttu-id="4c9b4-103">Группа: Валидатепропертиес</span><span class="sxs-lookup"><span data-stu-id="4c9b4-103">group: validateProperties</span></span>

<span data-ttu-id="4c9b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c9b4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c9b4-105">Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-105">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="4c9b4-106">Клиенты могут использовать этот API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться [Обновить](group-update.md) группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [update](group-update.md) an Office 365 group.</span></span> <span data-ttu-id="4c9b4-107">Чтобы проверить свойства перед созданием группы, используйте функцию [directoryobject: валидатепропертиес](directoryobject-validateproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="4c9b4-107">To validate the properties before creating a group, use the [directoryobject:validateProperties](directoryobject-validateproperties.md) function.</span></span>

<span data-ttu-id="4c9b4-108">Для отображаемого имени и свойств псевдонима почты выполняются следующие проверки политик:</span><span class="sxs-lookup"><span data-stu-id="4c9b4-108">The following policy validations are performed for the display name and mail nickname properties:</span></span>
1. <span data-ttu-id="4c9b4-109">Проверка политики именования префиксов и суффиксов</span><span class="sxs-lookup"><span data-stu-id="4c9b4-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="4c9b4-110">Проверка политики нестандартных запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="4c9b4-110">Validate the custom banned words policy</span></span>

<span data-ttu-id="4c9b4-111">Этот API возвращает только первую обнаруженную ошибку проверки.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-111">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="4c9b4-112">Если свойства не прошли несколько проверок, возвращается только первый сбой проверки.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-112">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="4c9b4-113">Тем не менее, вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяется только политика именования префиксов и суффиксов.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-113">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="4c9b4-114">Чтобы узнать больше о настройке политик именования, ознакомьтесь со статьей [Настройка политики именования](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span><span class="sxs-lookup"><span data-stu-id="4c9b4-114">To learn more about configuring naming policies, see [Configure naming policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c9b4-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c9b4-115">Permissions</span></span>

<span data-ttu-id="4c9b4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c9b4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c9b4-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c9b4-118">Permission type</span></span>      | <span data-ttu-id="4c9b4-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c9b4-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c9b4-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c9b4-120">Delegated (work or school account)</span></span> | <span data-ttu-id="4c9b4-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c9b4-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c9b4-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c9b4-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c9b4-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-123">Not supported.</span></span>    |
|<span data-ttu-id="4c9b4-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c9b4-124">Application</span></span> | <span data-ttu-id="4c9b4-125">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c9b4-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c9b4-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c9b4-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="4c9b4-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c9b4-127">Request headers</span></span>

| <span data-ttu-id="4c9b4-128">Имя</span><span class="sxs-lookup"><span data-stu-id="4c9b4-128">Name</span></span>           | <span data-ttu-id="4c9b4-129">Описание</span><span class="sxs-lookup"><span data-stu-id="4c9b4-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="4c9b4-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c9b4-130">Authorization</span></span>  | <span data-ttu-id="4c9b4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="4c9b4-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c9b4-133">Content-Type</span></span>   | <span data-ttu-id="4c9b4-134">application/json</span><span class="sxs-lookup"><span data-stu-id="4c9b4-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c9b4-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c9b4-135">Request body</span></span>

<span data-ttu-id="4c9b4-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4c9b4-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c9b4-137">Parameter</span></span>    | <span data-ttu-id="4c9b4-138">Тип</span><span class="sxs-lookup"><span data-stu-id="4c9b4-138">Type</span></span>   |<span data-ttu-id="4c9b4-139">Описание</span><span class="sxs-lookup"><span data-stu-id="4c9b4-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c9b4-140">displayName</span><span class="sxs-lookup"><span data-stu-id="4c9b4-140">displayName</span></span>|<span data-ttu-id="4c9b4-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4c9b4-141">String</span></span>| <span data-ttu-id="4c9b4-142">Отображаемое имя группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-142">The display name of the group to validate.</span></span> <span data-ttu-id="4c9b4-143">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-143">The property is not individually required.</span></span> <span data-ttu-id="4c9b4-144">Однако необходимо указать по крайней мере одно свойство (**DisplayName** или **mailNickname**).</span><span class="sxs-lookup"><span data-stu-id="4c9b4-144">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="4c9b4-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="4c9b4-145">mailNickname</span></span>|<span data-ttu-id="4c9b4-146">String</span><span class="sxs-lookup"><span data-stu-id="4c9b4-146">String</span></span>| <span data-ttu-id="4c9b4-147">Псевдоним почты для группы, которую требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-147">The mail nickname of the group to validate.</span></span> <span data-ttu-id="4c9b4-148">Свойство не обязательно должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-148">The property is not individually required.</span></span> <span data-ttu-id="4c9b4-149">Однако необходимо указать по крайней мере одно свойство (**DisplayName** или **mailNickname**).</span><span class="sxs-lookup"><span data-stu-id="4c9b4-149">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="4c9b4-150">онбехалфофусерид</span><span class="sxs-lookup"><span data-stu-id="4c9b4-150">onBehalfOfUserId</span></span>|<span data-ttu-id="4c9b4-151">GUID</span><span class="sxs-lookup"><span data-stu-id="4c9b4-151">Guid</span></span>| <span data-ttu-id="4c9b4-152">Идентификатор пользователя, который олицетворяет при вызове API.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-152">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="4c9b4-153">Результаты проверки предназначены для атрибутов и ролей **онбехалфофусерид** .</span><span class="sxs-lookup"><span data-stu-id="4c9b4-153">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="4c9b4-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c9b4-154">Response</span></span>
<span data-ttu-id="4c9b4-155">При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-155">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="4c9b4-156">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-156">It does not return anything in the response body.</span></span>

<span data-ttu-id="4c9b4-157">Если запрос является недопустимым, метод возвращает `400 Bad Request` код отклика.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-157">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="4c9b4-158">В тексте отклика возвращается сообщение об ошибке со сведениями о недопустимом запросе.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-158">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="4c9b4-159">При возникновении ошибки проверки.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-159">If there is a validation error.</span></span> <span data-ttu-id="4c9b4-160">Метод возвращает `422 Unprocessable Entity` код отклика.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-160">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="4c9b4-161">В тексте отклика возвращается сообщение об ошибке и коллекция сведений об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-161">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c9b4-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c9b4-162">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="4c9b4-163">Пример 1: успешный запрос на проверку</span><span class="sxs-lookup"><span data-stu-id="4c9b4-163">Example 1: Successful validation request</span></span>
<span data-ttu-id="4c9b4-164">В этом примере показан успешный запрос на проверку.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-164">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="4c9b4-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c9b4-165">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4c9b4-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c9b4-166">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4c9b4-167">C#</span><span class="sxs-lookup"><span data-stu-id="4c9b4-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c9b4-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c9b4-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c9b4-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c9b4-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c9b4-170">Java</span><span class="sxs-lookup"><span data-stu-id="4c9b4-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4c9b4-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c9b4-171">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="4c9b4-172">Пример 2: запрос с ошибками проверки</span><span class="sxs-lookup"><span data-stu-id="4c9b4-172">Example 2: Request with validation errors</span></span>
<span data-ttu-id="4c9b4-173">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="4c9b4-173">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="4c9b4-174">Запросить</span><span class="sxs-lookup"><span data-stu-id="4c9b4-174">Request</span></span>
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a><span data-ttu-id="4c9b4-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c9b4-175">Response</span></span>
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

---
title: 'Группа: validateProperties'
description: Проверьте, если группу Office 365 отображаемое имя или почты псевдонимов стандарту именования политик. Клиенты могут использовать API-Интерфейс для определения отображаемое имя или псевдоним почты является допустимым перед попыткой **обновления** группы с Office 365. Для проверки свойства перед созданием группы, используйте функцию validateProperties для объектов каталога.
ms.openlocfilehash: d7f2767908e6cbf9116bec769a1abc32731e4758
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075613"
---
# <a name="group-validateproperties"></a><span data-ttu-id="db843-105">Группа: validateProperties</span><span class="sxs-lookup"><span data-stu-id="db843-105">group: validateProperties</span></span>

<span data-ttu-id="db843-106">Проверьте, если группу Office 365 отображаемое имя или почты псевдонимов стандарту именования политик.</span><span class="sxs-lookup"><span data-stu-id="db843-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="db843-107">Клиенты могут использовать API-Интерфейс для определения отображаемое имя или псевдоним почты является допустимым перед попыткой **обновления** группы с Office 365.</span><span class="sxs-lookup"><span data-stu-id="db843-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="db843-108">Для проверки свойства перед созданием группы, используйте [функцию validateProperties](directoryobject-validateproperties.md) для объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="db843-108">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="db843-109">Для свойства отображаемое имя и почты псевдонимов выполняются следующие проверки:</span><span class="sxs-lookup"><span data-stu-id="db843-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="db843-110">Проверка префикс и суффикс, политика именования</span><span class="sxs-lookup"><span data-stu-id="db843-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="db843-111">Проверка настраиваемых запрещенных словах политики</span><span class="sxs-lookup"><span data-stu-id="db843-111">Validate the custom banned words policy</span></span>

<span data-ttu-id="db843-112">Этот интерфейс API возвращает с первого ошибка.</span><span class="sxs-lookup"><span data-stu-id="db843-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="db843-113">Если одно или несколько свойств с ошибкой нескольких проверок, возвращается только свойства с первого сбой проверки.</span><span class="sxs-lookup"><span data-stu-id="db843-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="db843-114">Тем не менее можно проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если выполняется только проверка префикс и суффикс, политика именования.</span><span class="sxs-lookup"><span data-stu-id="db843-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="db843-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db843-115">Permissions</span></span>

<span data-ttu-id="db843-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db843-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db843-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db843-118">Permission type</span></span>      | <span data-ttu-id="db843-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db843-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db843-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db843-120">Delegated (work or school account)</span></span> | <span data-ttu-id="db843-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db843-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="db843-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db843-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db843-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db843-123">Not supported.</span></span>    |
|<span data-ttu-id="db843-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db843-124">Application</span></span> | <span data-ttu-id="db843-125">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db843-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db843-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db843-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="db843-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db843-127">Request headers</span></span>

| <span data-ttu-id="db843-128">Имя</span><span class="sxs-lookup"><span data-stu-id="db843-128">Name</span></span>           | <span data-ttu-id="db843-129">Описание</span><span class="sxs-lookup"><span data-stu-id="db843-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="db843-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="db843-130">Authorization</span></span>  | <span data-ttu-id="db843-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="db843-131">Bearer {code}</span></span>    |
| <span data-ttu-id="db843-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db843-132">Content-Type</span></span>   | <span data-ttu-id="db843-133">application/json</span><span class="sxs-lookup"><span data-stu-id="db843-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="db843-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db843-134">Request body</span></span>

<span data-ttu-id="db843-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="db843-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="db843-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="db843-136">Parameter</span></span>    | <span data-ttu-id="db843-137">Тип</span><span class="sxs-lookup"><span data-stu-id="db843-137">Type</span></span>   |<span data-ttu-id="db843-138">Описание</span><span class="sxs-lookup"><span data-stu-id="db843-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db843-139">displayName</span><span class="sxs-lookup"><span data-stu-id="db843-139">displayName</span></span>|<span data-ttu-id="db843-140">String</span><span class="sxs-lookup"><span data-stu-id="db843-140">String</span></span>| <span data-ttu-id="db843-141">Отображаемое имя группы, чтобы проверить.</span><span class="sxs-lookup"><span data-stu-id="db843-141">The display name of the group to validate.</span></span> <span data-ttu-id="db843-142">Свойство не требуется по отдельности.</span><span class="sxs-lookup"><span data-stu-id="db843-142">The property is not individually required.</span></span> <span data-ttu-id="db843-143">Тем не менее по крайней мере одно свойство (отображаемое имя или mailNickname) является обязательным.</span><span class="sxs-lookup"><span data-stu-id="db843-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="db843-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="db843-144">mailNickname</span></span>|<span data-ttu-id="db843-145">String</span><span class="sxs-lookup"><span data-stu-id="db843-145">String</span></span>| <span data-ttu-id="db843-146">Псевдоним почты группы для проверки.</span><span class="sxs-lookup"><span data-stu-id="db843-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="db843-147">Свойство не требуется по отдельности.</span><span class="sxs-lookup"><span data-stu-id="db843-147">The property is not individually required.</span></span> <span data-ttu-id="db843-148">Тем не менее по крайней мере одно свойство (отображаемое имя или mailNickname) является обязательным.</span><span class="sxs-lookup"><span data-stu-id="db843-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="db843-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="db843-149">onBehalfOfUserId</span></span>|<span data-ttu-id="db843-150">Guid</span><span class="sxs-lookup"><span data-stu-id="db843-150">Guid</span></span>| <span data-ttu-id="db843-151">Идентификатор объекта пользователя для олицетворения при вызове API.</span><span class="sxs-lookup"><span data-stu-id="db843-151">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="db843-152">Результаты проверки используются атрибуты onBehalfOfUserId и роли.</span><span class="sxs-lookup"><span data-stu-id="db843-152">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="db843-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="db843-153">Response</span></span>
<span data-ttu-id="db843-154">В случае успешного выполнения и нет ошибок проверки, метод возвращает `204 No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="db843-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="db843-155">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="db843-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="db843-156">Если запрос является недопустимым, метод возвращает `400 Bad Request` код ответа.</span><span class="sxs-lookup"><span data-stu-id="db843-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="db843-157">Сообщение об ошибке с подробными сведениями о недопустимый запрос возвращается в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="db843-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="db843-158">В случае ошибки проверки.</span><span class="sxs-lookup"><span data-stu-id="db843-158">If there is a validation error.</span></span> <span data-ttu-id="db843-159">Метод возвращает `422 Unprocessable Entity` код ответа.</span><span class="sxs-lookup"><span data-stu-id="db843-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="db843-160">Сообщение об ошибке и коллекцию сведений об ошибках, возвращается в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="db843-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db843-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="db843-161">Examples</span></span>

<span data-ttu-id="db843-162">Это пример успешной проверки запроса.</span><span class="sxs-lookup"><span data-stu-id="db843-162">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="db843-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="db843-163">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="db843-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="db843-164">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="db843-165">Это пример запроса с ошибок проверки.</span><span class="sxs-lookup"><span data-stu-id="db843-165">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="db843-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="db843-166">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="db843-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="db843-167">Response</span></span>
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
  "tocPath": ""
}-->

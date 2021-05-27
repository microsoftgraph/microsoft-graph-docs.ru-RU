---
title: 'группа: проверкаProperties'
description: Проверка того, Microsoft 365 или псевдоним почты группы соответствует политикам именования.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6f41ee4f9ae52133d3c7611b52b42997480dfc40
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681223"
---
# <a name="group-validateproperties"></a><span data-ttu-id="60a23-103">группа: проверкаProperties</span><span class="sxs-lookup"><span data-stu-id="60a23-103">group: validateProperties</span></span>

<span data-ttu-id="60a23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60a23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60a23-105">Проверка того, Microsoft 365 или псевдоним почты группы соответствует политикам именования.</span><span class="sxs-lookup"><span data-stu-id="60a23-105">Validate if a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="60a23-106">Клиенты могут использовать API, чтобы определить, допустимо ли  имя или псевдоним почты перед тем, как обновить Microsoft 365 группу.</span><span class="sxs-lookup"><span data-stu-id="60a23-106">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** a Microsoft 365 group.</span></span> <span data-ttu-id="60a23-107">Для проверки свойств перед созданием группы используйте функцию [validateProperties](directoryobject-validateproperties.md) для объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="60a23-107">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="60a23-108">Следующие проверки выполняются для свойств отображения имени и ником почты:</span><span class="sxs-lookup"><span data-stu-id="60a23-108">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="60a23-109">Проверка политики имен префикса и суффикса</span><span class="sxs-lookup"><span data-stu-id="60a23-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="60a23-110">Проверка настраиваемой политики запрещенных слов</span><span class="sxs-lookup"><span data-stu-id="60a23-110">Validate the custom banned words policy</span></span>

<span data-ttu-id="60a23-111">Этот API возвращается с первым сбоем.</span><span class="sxs-lookup"><span data-stu-id="60a23-111">This API returns with the first failure encountered.</span></span> <span data-ttu-id="60a23-112">Если одно или несколько свойств не удается несколько проверки, возвращается только свойство с первым сбоем проверки.</span><span class="sxs-lookup"><span data-stu-id="60a23-112">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="60a23-113">Однако вы можете проверить как имя почты, так и имя дисплея и получить коллекцию ошибок проверки, если вы только проверяете политику именования префикса и суффикса.</span><span class="sxs-lookup"><span data-stu-id="60a23-113">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="60a23-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60a23-114">Permissions</span></span>

<span data-ttu-id="60a23-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60a23-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60a23-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60a23-117">Permission type</span></span>      | <span data-ttu-id="60a23-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60a23-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60a23-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60a23-119">Delegated (work or school account)</span></span> | <span data-ttu-id="60a23-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60a23-120">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="60a23-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60a23-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60a23-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60a23-122">Not supported.</span></span>    |
|<span data-ttu-id="60a23-123">Приложение</span><span class="sxs-lookup"><span data-stu-id="60a23-123">Application</span></span> | <span data-ttu-id="60a23-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60a23-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60a23-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60a23-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="60a23-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60a23-126">Request headers</span></span>

| <span data-ttu-id="60a23-127">Имя</span><span class="sxs-lookup"><span data-stu-id="60a23-127">Name</span></span>           | <span data-ttu-id="60a23-128">Описание</span><span class="sxs-lookup"><span data-stu-id="60a23-128">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="60a23-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60a23-129">Authorization</span></span>  | <span data-ttu-id="60a23-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="60a23-130">Bearer {code}</span></span>    |
| <span data-ttu-id="60a23-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60a23-131">Content-Type</span></span>   | <span data-ttu-id="60a23-132">application/json</span><span class="sxs-lookup"><span data-stu-id="60a23-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="60a23-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60a23-133">Request body</span></span>

<span data-ttu-id="60a23-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="60a23-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60a23-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="60a23-135">Parameter</span></span>    | <span data-ttu-id="60a23-136">Тип</span><span class="sxs-lookup"><span data-stu-id="60a23-136">Type</span></span>   |<span data-ttu-id="60a23-137">Описание</span><span class="sxs-lookup"><span data-stu-id="60a23-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60a23-138">displayName</span><span class="sxs-lookup"><span data-stu-id="60a23-138">displayName</span></span>|<span data-ttu-id="60a23-139">String</span><span class="sxs-lookup"><span data-stu-id="60a23-139">String</span></span>| <span data-ttu-id="60a23-140">Отображаемого имени группы для проверки.</span><span class="sxs-lookup"><span data-stu-id="60a23-140">The display name of the group to validate.</span></span> <span data-ttu-id="60a23-141">Свойство не требуется по отдельности.</span><span class="sxs-lookup"><span data-stu-id="60a23-141">The property is not individually required.</span></span> <span data-ttu-id="60a23-142">Однако требуется по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="60a23-142">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="60a23-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="60a23-143">mailNickname</span></span>|<span data-ttu-id="60a23-144">String</span><span class="sxs-lookup"><span data-stu-id="60a23-144">String</span></span>| <span data-ttu-id="60a23-145">Имя почты группы для проверки.</span><span class="sxs-lookup"><span data-stu-id="60a23-145">The mail nickname of the group to validate.</span></span> <span data-ttu-id="60a23-146">Свойство не требуется по отдельности.</span><span class="sxs-lookup"><span data-stu-id="60a23-146">The property is not individually required.</span></span> <span data-ttu-id="60a23-147">Однако требуется по крайней мере одно свойство (displayName или mailNickname).</span><span class="sxs-lookup"><span data-stu-id="60a23-147">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="60a23-148">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="60a23-148">onBehalfOfUserId</span></span>|<span data-ttu-id="60a23-149">Guid</span><span class="sxs-lookup"><span data-stu-id="60a23-149">Guid</span></span>| <span data-ttu-id="60a23-150">ID объекта пользователя, который должен выдать себя при вызове API.</span><span class="sxs-lookup"><span data-stu-id="60a23-150">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="60a23-151">Результаты проверки для атрибутов и ролей onBehalfOfUserId.</span><span class="sxs-lookup"><span data-stu-id="60a23-151">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="60a23-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="60a23-152">Response</span></span>
<span data-ttu-id="60a23-153">В случае успешной проверки и без ошибок проверки метод возвращает `204 No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="60a23-153">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="60a23-154">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="60a23-154">It does not return anything in the response body.</span></span>

<span data-ttu-id="60a23-155">Если запрос недействителен, метод возвращает `400 Bad Request` код ответа.</span><span class="sxs-lookup"><span data-stu-id="60a23-155">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="60a23-156">Сообщение об ошибке с сведениями о недействительности запроса возвращается в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="60a23-156">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="60a23-157">При ошибке проверки.</span><span class="sxs-lookup"><span data-stu-id="60a23-157">If there is a validation error.</span></span> <span data-ttu-id="60a23-158">Метод возвращает код `422 Unprocessable Entity` ответа.</span><span class="sxs-lookup"><span data-stu-id="60a23-158">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="60a23-159">Сообщение об ошибке и коллекция сведений об ошибках возвращаются в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="60a23-159">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60a23-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="60a23-160">Examples</span></span>

<span data-ttu-id="60a23-161">Это пример успешного запроса на проверку.</span><span class="sxs-lookup"><span data-stu-id="60a23-161">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="60a23-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="60a23-162">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="60a23-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="60a23-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="60a23-164">C#</span><span class="sxs-lookup"><span data-stu-id="60a23-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60a23-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60a23-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60a23-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60a23-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60a23-167">Java</span><span class="sxs-lookup"><span data-stu-id="60a23-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="60a23-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="60a23-168">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="60a23-169">Это пример запроса с ошибками проверки.</span><span class="sxs-lookup"><span data-stu-id="60a23-169">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="60a23-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="60a23-170">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="60a23-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="60a23-171">Response</span></span>
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



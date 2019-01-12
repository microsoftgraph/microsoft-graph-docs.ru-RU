---
title: 'directoryObject: validateProperties'
description: Проверьте, если группу Office 365 отображаемое имя или почты псевдонимов стандарту именования политик.  Клиенты могут использовать API-Интерфейс для определения отображаемое имя или псевдоним почты является допустимым перед попыткой **Создать** группу Office 365. Для проверки правильности свойств существующей группы, используйте функцию validateProperties для групп.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 515acb022150d091e7dcbbdecc1fb1adef849a88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921320"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="776d3-105">directoryObject: validateProperties</span><span class="sxs-lookup"><span data-stu-id="776d3-105">directoryObject: validateProperties</span></span>

<span data-ttu-id="776d3-106">Проверьте, если группу Office 365 отображаемое имя или почты псевдонимов стандарту именования политик.</span><span class="sxs-lookup"><span data-stu-id="776d3-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="776d3-107">Клиенты могут использовать API-Интерфейс для определения отображаемое имя или псевдоним почты является допустимым перед попыткой **Создать** группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="776d3-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **create** an Office 365 group.</span></span> <span data-ttu-id="776d3-108">Для проверки правильности свойств существующей группы, используйте [функцию validateProperties](group-validateproperties.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="776d3-108">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="776d3-109">Для свойства отображаемое имя и почты псевдонимов выполняются следующие проверки:</span><span class="sxs-lookup"><span data-stu-id="776d3-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="776d3-110">Проверка префикс и суффикс, политика именования</span><span class="sxs-lookup"><span data-stu-id="776d3-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="776d3-111">Проверка настраиваемых запрещенных словах политики</span><span class="sxs-lookup"><span data-stu-id="776d3-111">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="776d3-112">Проверка почты псевдонимов является уникальным</span><span class="sxs-lookup"><span data-stu-id="776d3-112">Validate the mail nickname is unique</span></span>

<span data-ttu-id="776d3-113">Этот интерфейс API возвращает с первого ошибка.</span><span class="sxs-lookup"><span data-stu-id="776d3-113">This API returns with the first failure encountered.</span></span> <span data-ttu-id="776d3-114">Если одно или несколько свойств с ошибкой нескольких проверок, возвращается только свойства с первого сбой проверки.</span><span class="sxs-lookup"><span data-stu-id="776d3-114">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="776d3-115">Тем не менее можно проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если выполняется только проверка префикс и суффикс, политика именования.</span><span class="sxs-lookup"><span data-stu-id="776d3-115">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="776d3-116">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="776d3-116">Prerequisites</span></span>

<span data-ttu-id="776d3-117">Для выполнения этот интерфейс API требуется следующее **разрешение** : *Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="776d3-117">The following **permission** is required to execute this API: *Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="776d3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="776d3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="776d3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="776d3-119">Request headers</span></span>

| <span data-ttu-id="776d3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="776d3-120">Name</span></span>           | <span data-ttu-id="776d3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="776d3-121">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="776d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="776d3-122">Authorization</span></span>  | <span data-ttu-id="776d3-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="776d3-123">Bearer {code}</span></span>    |
| <span data-ttu-id="776d3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="776d3-124">Content-Type</span></span>   | <span data-ttu-id="776d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="776d3-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="776d3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="776d3-126">Request body</span></span>
<span data-ttu-id="776d3-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="776d3-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="776d3-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="776d3-128">Parameter</span></span>    | <span data-ttu-id="776d3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="776d3-129">Type</span></span>   |<span data-ttu-id="776d3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="776d3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="776d3-131">entityType</span><span class="sxs-lookup"><span data-stu-id="776d3-131">entityType</span></span>|<span data-ttu-id="776d3-132">Строка</span><span class="sxs-lookup"><span data-stu-id="776d3-132">String</span></span>| <span data-ttu-id="776d3-133">`Group`— Это тип только поддерживаемые сущности.</span><span class="sxs-lookup"><span data-stu-id="776d3-133">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="776d3-134">displayName</span><span class="sxs-lookup"><span data-stu-id="776d3-134">displayName</span></span>|<span data-ttu-id="776d3-135">Строка</span><span class="sxs-lookup"><span data-stu-id="776d3-135">String</span></span>| <span data-ttu-id="776d3-136">Отображаемое имя группы, чтобы проверить.</span><span class="sxs-lookup"><span data-stu-id="776d3-136">The display name of the group to validate.</span></span> <span data-ttu-id="776d3-137">Свойство не требуется по отдельности.</span><span class="sxs-lookup"><span data-stu-id="776d3-137">The property is not individually required.</span></span> <span data-ttu-id="776d3-138">Тем не менее по крайней мере одно свойство (отображаемое имя или mailNickname) является обязательным.</span><span class="sxs-lookup"><span data-stu-id="776d3-138">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="776d3-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="776d3-139">mailNickname</span></span>|<span data-ttu-id="776d3-140">String</span><span class="sxs-lookup"><span data-stu-id="776d3-140">String</span></span>| <span data-ttu-id="776d3-141">Псевдоним почты группы для проверки.</span><span class="sxs-lookup"><span data-stu-id="776d3-141">The mail nickname of the group to validate.</span></span> <span data-ttu-id="776d3-142">Свойство не требуется по отдельности.</span><span class="sxs-lookup"><span data-stu-id="776d3-142">The property is not individually required.</span></span> <span data-ttu-id="776d3-143">Тем не менее по крайней мере одно свойство (отображаемое имя или mailNickname) является обязательным.</span><span class="sxs-lookup"><span data-stu-id="776d3-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="776d3-144">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="776d3-144">onBehalfOfUserId</span></span>|<span data-ttu-id="776d3-145">Guid</span><span class="sxs-lookup"><span data-stu-id="776d3-145">Guid</span></span>| <span data-ttu-id="776d3-146">Идентификатор объекта пользователя для олицетворения при вызове API.</span><span class="sxs-lookup"><span data-stu-id="776d3-146">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="776d3-147">Результаты проверки используются атрибуты onBehalfOfUserId и роли.</span><span class="sxs-lookup"><span data-stu-id="776d3-147">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="776d3-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="776d3-148">Response</span></span>

<span data-ttu-id="776d3-149">В случае успешного выполнения и нет ошибок проверки, метод возвращает `204 No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="776d3-149">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="776d3-150">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="776d3-150">It does not return anything in the response body.</span></span>

<span data-ttu-id="776d3-151">Если запрос является недопустимым, метод возвращает `400 Bad Request` код ответа.</span><span class="sxs-lookup"><span data-stu-id="776d3-151">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="776d3-152">Сообщение об ошибке с подробными сведениями о недопустимый запрос возвращается в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="776d3-152">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="776d3-153">Если ошибка проверки, метод возвращает `422 Unprocessable Entity` код ответа.</span><span class="sxs-lookup"><span data-stu-id="776d3-153">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="776d3-154">Сообщение об ошибке и коллекцию сведений об ошибках, возвращается в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="776d3-154">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="776d3-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="776d3-155">Examples</span></span>

<span data-ttu-id="776d3-156">Это пример успешной проверки запроса.</span><span class="sxs-lookup"><span data-stu-id="776d3-156">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="776d3-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="776d3-157">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="776d3-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="776d3-158">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="776d3-159">Это пример запроса с ошибок проверки.</span><span class="sxs-lookup"><span data-stu-id="776d3-159">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="776d3-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="776d3-160">Request</span></span>
```http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="776d3-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="776d3-161">Response</span></span>
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
  "tocPath": ""
}-->

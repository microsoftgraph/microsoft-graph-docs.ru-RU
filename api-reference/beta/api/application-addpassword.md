---
title: 'Приложение: Аддпассворд'
description: Добавление надежного пароля в приложение.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6547123c92947240ab0b82a143e95bc930abef21
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441580"
---
# <a name="application-addpassword"></a><span data-ttu-id="09305-103">Приложение: Аддпассворд</span><span class="sxs-lookup"><span data-stu-id="09305-103">application: addPassword</span></span>

<span data-ttu-id="09305-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="09305-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09305-105">Добавляет надежный пароль для [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="09305-105">Adds a strong password to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="09305-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09305-106">Permissions</span></span>

<span data-ttu-id="09305-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09305-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09305-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09305-109">Permission type</span></span>                        | <span data-ttu-id="09305-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09305-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="09305-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09305-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="09305-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09305-112">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="09305-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09305-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09305-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09305-114">Not supported.</span></span> |
| <span data-ttu-id="09305-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09305-115">Application</span></span>                            | <span data-ttu-id="09305-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09305-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09305-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09305-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="09305-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09305-118">Request headers</span></span>

| <span data-ttu-id="09305-119">Имя</span><span class="sxs-lookup"><span data-stu-id="09305-119">Name</span></span>           | <span data-ttu-id="09305-120">Описание</span><span class="sxs-lookup"><span data-stu-id="09305-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="09305-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09305-121">Authorization</span></span>  | <span data-ttu-id="09305-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09305-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="09305-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09305-124">Content-type</span></span>   | <span data-ttu-id="09305-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09305-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="09305-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="09305-127">Request body</span></span>

<span data-ttu-id="09305-128">В тексте запроса укажите необязательный `passwordCredential` объект со следующими свойствами.</span><span class="sxs-lookup"><span data-stu-id="09305-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="09305-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="09305-129">Property</span></span>     | <span data-ttu-id="09305-130">Тип</span><span class="sxs-lookup"><span data-stu-id="09305-130">Type</span></span>   |<span data-ttu-id="09305-131">Описание</span><span class="sxs-lookup"><span data-stu-id="09305-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="09305-132">displayName</span><span class="sxs-lookup"><span data-stu-id="09305-132">displayName</span></span> | <span data-ttu-id="09305-133">String</span><span class="sxs-lookup"><span data-stu-id="09305-133">String</span></span> | <span data-ttu-id="09305-134">Понятное имя для пароля.</span><span class="sxs-lookup"><span data-stu-id="09305-134">Friendly name for the password.</span></span> <span data-ttu-id="09305-135">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="09305-135">Optional.</span></span> |
| <span data-ttu-id="09305-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="09305-136">endDateTime</span></span> | <span data-ttu-id="09305-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09305-137">DateTimeOffset</span></span> | <span data-ttu-id="09305-138">Дата и время истечения срока действия пароля, представленного в формате ISO 8601, и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="09305-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="09305-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="09305-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="09305-140">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="09305-140">Optional.</span></span> |
| <span data-ttu-id="09305-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="09305-141">startDateTime</span></span> | <span data-ttu-id="09305-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09305-142">DateTimeOffset</span></span> | <span data-ttu-id="09305-143">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="09305-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="09305-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="09305-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="09305-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="09305-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="09305-146">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="09305-146">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="09305-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="09305-147">Response</span></span>

<span data-ttu-id="09305-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [пассвордкредентиал](../resources/passwordcredential.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09305-148">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="09305-149">Свойство **секреттекст** в объекте Response содержит надежные пароли, созданные Azure Active Directory длиной 16-64 символов.</span><span class="sxs-lookup"><span data-stu-id="09305-149">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="09305-150">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="09305-150">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="09305-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="09305-151">Examples</span></span>

<span data-ttu-id="09305-152">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="09305-152">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="09305-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="09305-153">Request</span></span>

<span data-ttu-id="09305-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09305-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="09305-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="09305-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addpassword"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
Content-type: application/json

{
  "passwordCredential": {
    "displayName": "Password friendly name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="09305-156">C#</span><span class="sxs-lookup"><span data-stu-id="09305-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addpassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09305-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09305-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09305-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09305-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="09305-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="09305-159">Response</span></span>

<span data-ttu-id="09305-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="09305-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordCredential"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "customKeyIdentifier": null,
    "endDateTime": "2021-09-09T19:50:29.3086381Z",
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "startDateTime": "2019-09-09T19:50:29.3086381Z",
    "secretText": "[6gyXA5S20@MN+WRXAJ]I-TO7g1:h2P8",
    "hint": "[6g",
    "displayName": "Password friendly name"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: addPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

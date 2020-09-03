---
title: 'Приложение: Аддпассворд'
description: Добавление надежного пароля в приложение.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d816e00298ca0a82df3f595f19950bb44570ab4
ms.sourcegitcommit: c6e8a2097267ace4c78124be48646f9129114b26
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/03/2020
ms.locfileid: "47340056"
---
# <a name="application-addpassword"></a><span data-ttu-id="c0d6c-103">Приложение: Аддпассворд</span><span class="sxs-lookup"><span data-stu-id="c0d6c-103">application: addPassword</span></span>

<span data-ttu-id="c0d6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0d6c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0d6c-105">Добавляет надежный пароль для [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="c0d6c-105">Adds a strong password to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0d6c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0d6c-106">Permissions</span></span>

<span data-ttu-id="c0d6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0d6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0d6c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0d6c-109">Permission type</span></span>                        | <span data-ttu-id="c0d6c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0d6c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c0d6c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0d6c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0d6c-112">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c0d6c-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="c0d6c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0d6c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0d6c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-114">Not supported.</span></span> |
| <span data-ttu-id="c0d6c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0d6c-115">Application</span></span>                            | <span data-ttu-id="c0d6c-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0d6c-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0d6c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0d6c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="c0d6c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0d6c-118">Request headers</span></span>

| <span data-ttu-id="c0d6c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c0d6c-119">Name</span></span>           | <span data-ttu-id="c0d6c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c0d6c-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="c0d6c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0d6c-121">Authorization</span></span>  | <span data-ttu-id="c0d6c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c0d6c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0d6c-124">Content-Type</span></span>   | <span data-ttu-id="c0d6c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0d6c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0d6c-127">Request body</span></span>

<span data-ttu-id="c0d6c-128">В тексте запроса укажите необязательный `passwordCredential` объект со следующими свойствами.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="c0d6c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0d6c-129">Property</span></span>     | <span data-ttu-id="c0d6c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c0d6c-130">Type</span></span>   |<span data-ttu-id="c0d6c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c0d6c-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c0d6c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c0d6c-132">displayName</span></span> | <span data-ttu-id="c0d6c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c0d6c-133">String</span></span> | <span data-ttu-id="c0d6c-134">Понятное имя для пароля.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-134">Friendly name for the password.</span></span> <span data-ttu-id="c0d6c-135">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-135">Optional.</span></span> |
| <span data-ttu-id="c0d6c-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c0d6c-136">endDateTime</span></span> | <span data-ttu-id="c0d6c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0d6c-137">DateTimeOffset</span></span> | <span data-ttu-id="c0d6c-138">Дата и время истечения срока действия пароля, представленного в формате ISO 8601, и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c0d6c-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c0d6c-140">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-140">Optional.</span></span> <span data-ttu-id="c0d6c-141">Значение по умолчанию — "startDateTime + 2 года".</span><span class="sxs-lookup"><span data-stu-id="c0d6c-141">The default value is "startDateTime + 2 years".</span></span> |
| <span data-ttu-id="c0d6c-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c0d6c-142">startDateTime</span></span> | <span data-ttu-id="c0d6c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0d6c-143">DateTimeOffset</span></span> | <span data-ttu-id="c0d6c-144">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="c0d6c-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c0d6c-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c0d6c-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c0d6c-147">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-147">Optional.</span></span>  <span data-ttu-id="c0d6c-148">Значение по умолчанию — "Now".</span><span class="sxs-lookup"><span data-stu-id="c0d6c-148">The default value is "now".</span></span> |

## <a name="response"></a><span data-ttu-id="c0d6c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0d6c-149">Response</span></span>

<span data-ttu-id="c0d6c-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [пассвордкредентиал](../resources/passwordcredential.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-150">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="c0d6c-151">Свойство **секреттекст** в объекте Response содержит надежные пароли, созданные Azure Active Directory длиной 16-64 символов.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-151">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="c0d6c-152">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-152">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="c0d6c-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="c0d6c-153">Examples</span></span>

<span data-ttu-id="c0d6c-154">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-154">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c0d6c-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0d6c-155">Request</span></span>

<span data-ttu-id="c0d6c-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-156">The following is an example of the request.</span></span> <span data-ttu-id="c0d6c-157">**Идентификатор** , указанный в запросе, это значение свойства **ID** приложения, а не значение свойства **AppID** .</span><span class="sxs-lookup"><span data-stu-id="c0d6c-157">The **id** that is specified in the request is the value of the **id** property of the application, not the value of the **appId** property.</span></span> 

# <a name="http"></a>[<span data-ttu-id="c0d6c-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0d6c-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addpassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addPassword
Content-type: application/json

{
  "passwordCredential": {
    "displayName": "Password friendly name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="c0d6c-159">C#</span><span class="sxs-lookup"><span data-stu-id="c0d6c-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addpassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0d6c-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0d6c-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0d6c-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0d6c-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0d6c-162">Java</span><span class="sxs-lookup"><span data-stu-id="c0d6c-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addpassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0d6c-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0d6c-163">Response</span></span>

<span data-ttu-id="c0d6c-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c0d6c-164">The following is an example of the response.</span></span>

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

---
title: 'приложение: addPassword'
description: Добавление надежного пароля в приложение.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 90fc14f3d56c9ca815d7abd721cdeef48dfdb23b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721980"
---
# <a name="application-addpassword"></a><span data-ttu-id="6b718-103">приложение: addPassword</span><span class="sxs-lookup"><span data-stu-id="6b718-103">application: addPassword</span></span>

<span data-ttu-id="6b718-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b718-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b718-105">Добавляет надежный пароль в [приложение.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="6b718-105">Adds a strong password to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b718-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b718-106">Permissions</span></span>

<span data-ttu-id="6b718-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b718-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b718-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b718-109">Permission type</span></span>                        | <span data-ttu-id="6b718-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b718-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6b718-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b718-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b718-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6b718-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="6b718-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b718-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b718-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b718-114">Application.ReadWrite.All</span></span> |
| <span data-ttu-id="6b718-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6b718-115">Application</span></span>                            | <span data-ttu-id="6b718-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b718-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b718-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b718-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="6b718-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b718-118">Request headers</span></span>

| <span data-ttu-id="6b718-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6b718-119">Name</span></span>           | <span data-ttu-id="6b718-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6b718-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="6b718-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b718-121">Authorization</span></span>  | <span data-ttu-id="6b718-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b718-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6b718-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b718-124">Content-Type</span></span>   | <span data-ttu-id="6b718-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b718-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b718-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b718-127">Request body</span></span>

<span data-ttu-id="6b718-128">В теле запроса укажи необязательный `passwordCredential` объект со следующими свойствами.</span><span class="sxs-lookup"><span data-stu-id="6b718-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="6b718-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b718-129">Property</span></span>     | <span data-ttu-id="6b718-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6b718-130">Type</span></span>   |<span data-ttu-id="6b718-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6b718-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6b718-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6b718-132">displayName</span></span> | <span data-ttu-id="6b718-133">String</span><span class="sxs-lookup"><span data-stu-id="6b718-133">String</span></span> | <span data-ttu-id="6b718-134">Удобное имя пароля.</span><span class="sxs-lookup"><span data-stu-id="6b718-134">Friendly name for the password.</span></span> <span data-ttu-id="6b718-135">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="6b718-135">Optional.</span></span> |
| <span data-ttu-id="6b718-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6b718-136">endDateTime</span></span> | <span data-ttu-id="6b718-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b718-137">DateTimeOffset</span></span> | <span data-ttu-id="6b718-138">Дата и время, в течение которых истекает срок действия пароля, представлены в формате ISO 8601 и всегда во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="6b718-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6b718-139">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="6b718-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="6b718-140">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="6b718-140">Optional.</span></span> <span data-ttu-id="6b718-141">Значение по умолчанию — startDateTime + 2 лет.</span><span class="sxs-lookup"><span data-stu-id="6b718-141">The default value is "startDateTime + 2 years".</span></span> |
| <span data-ttu-id="6b718-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6b718-142">startDateTime</span></span> | <span data-ttu-id="6b718-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b718-143">DateTimeOffset</span></span> | <span data-ttu-id="6b718-144">Дата и время, в течение которых пароль становится допустимым.</span><span class="sxs-lookup"><span data-stu-id="6b718-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="6b718-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6b718-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6b718-146">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="6b718-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="6b718-147">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="6b718-147">Optional.</span></span>  <span data-ttu-id="6b718-148">По умолчанию значение "сейчас".</span><span class="sxs-lookup"><span data-stu-id="6b718-148">The default value is "now".</span></span> |

## <a name="response"></a><span data-ttu-id="6b718-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b718-149">Response</span></span>

<span data-ttu-id="6b718-150">В случае успешной работы этот метод возвращает код отклика и новый `200 OK` [объект passwordCredential](../resources/passwordcredential.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6b718-150">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="6b718-151">Свойство **secretText в** объекте ответа содержит надежные пароли, созданные Azure Active Directory длиной 16-64 символов.</span><span class="sxs-lookup"><span data-stu-id="6b718-151">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="6b718-152">В будущем этот пароль не будет извлечен.</span><span class="sxs-lookup"><span data-stu-id="6b718-152">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="6b718-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="6b718-153">Examples</span></span>

<span data-ttu-id="6b718-154">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="6b718-154">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6b718-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b718-155">Request</span></span>

<span data-ttu-id="6b718-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b718-156">The following is an example of the request.</span></span> <span data-ttu-id="6b718-157">**ID,** указанный в запросе, — это значение свойства **id** приложения, а не свойства **appId.**</span><span class="sxs-lookup"><span data-stu-id="6b718-157">The **id** that is specified in the request is the value of the **id** property of the application, not the value of the **appId** property.</span></span> 

# <a name="http"></a>[<span data-ttu-id="6b718-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b718-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6b718-159">C#</span><span class="sxs-lookup"><span data-stu-id="6b718-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addpassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b718-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b718-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b718-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b718-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b718-162">Java</span><span class="sxs-lookup"><span data-stu-id="6b718-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addpassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6b718-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b718-163">Response</span></span>

<span data-ttu-id="6b718-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6b718-164">The following is an example of the response.</span></span>

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


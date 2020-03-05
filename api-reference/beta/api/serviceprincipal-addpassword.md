---
title: 'servicePrincipal: Аддпассворд'
description: Добавьте надежный пароль для servicePrincipal.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 11a8d6e6a54941e6ecee10878c01ed0e5f5e91da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453529"
---
# <a name="serviceprincipal-addpassword"></a><span data-ttu-id="92aef-103">servicePrincipal: Аддпассворд</span><span class="sxs-lookup"><span data-stu-id="92aef-103">servicePrincipal: addPassword</span></span>

<span data-ttu-id="92aef-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="92aef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92aef-105">Добавьте надежный пароль для объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="92aef-105">Add a strong password to a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="92aef-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92aef-106">Permissions</span></span>

<span data-ttu-id="92aef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92aef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92aef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92aef-109">Permission type</span></span>                        | <span data-ttu-id="92aef-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92aef-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="92aef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92aef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="92aef-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="92aef-112">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="92aef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92aef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92aef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92aef-114">Not supported.</span></span> |
| <span data-ttu-id="92aef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92aef-115">Application</span></span>                            | <span data-ttu-id="92aef-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92aef-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92aef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92aef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="92aef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92aef-118">Request headers</span></span>

| <span data-ttu-id="92aef-119">Имя</span><span class="sxs-lookup"><span data-stu-id="92aef-119">Name</span></span>           | <span data-ttu-id="92aef-120">Описание</span><span class="sxs-lookup"><span data-stu-id="92aef-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="92aef-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92aef-121">Authorization</span></span>  | <span data-ttu-id="92aef-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92aef-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="92aef-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92aef-124">Content-type</span></span>   | <span data-ttu-id="92aef-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92aef-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92aef-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="92aef-127">Request body</span></span>

<span data-ttu-id="92aef-128">В тексте запроса укажите необязательный `passwordCredential` объект со следующими свойствами.</span><span class="sxs-lookup"><span data-stu-id="92aef-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="92aef-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="92aef-129">Property</span></span>     | <span data-ttu-id="92aef-130">Тип</span><span class="sxs-lookup"><span data-stu-id="92aef-130">Type</span></span>   |<span data-ttu-id="92aef-131">Описание</span><span class="sxs-lookup"><span data-stu-id="92aef-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="92aef-132">displayName</span><span class="sxs-lookup"><span data-stu-id="92aef-132">displayName</span></span> | <span data-ttu-id="92aef-133">String</span><span class="sxs-lookup"><span data-stu-id="92aef-133">String</span></span> | <span data-ttu-id="92aef-134">Понятное имя для пароля.</span><span class="sxs-lookup"><span data-stu-id="92aef-134">Friendly name for the password.</span></span> <span data-ttu-id="92aef-135">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="92aef-135">Optional.</span></span> |
| <span data-ttu-id="92aef-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="92aef-136">endDateTime</span></span> | <span data-ttu-id="92aef-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92aef-137">DateTimeOffset</span></span> | <span data-ttu-id="92aef-138">Дата и время истечения срока действия пароля, представленного в формате ISO 8601, и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="92aef-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="92aef-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="92aef-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="92aef-140">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="92aef-140">Optional.</span></span> |
| <span data-ttu-id="92aef-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="92aef-141">startDateTime</span></span> | <span data-ttu-id="92aef-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92aef-142">DateTimeOffset</span></span> | <span data-ttu-id="92aef-143">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="92aef-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="92aef-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="92aef-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="92aef-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="92aef-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="92aef-146">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="92aef-146">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="92aef-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="92aef-147">Response</span></span>

<span data-ttu-id="92aef-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [пассвордкредентиал](../resources/passwordcredential.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92aef-148">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="92aef-149">Свойство **секреттекст** в объекте Response содержит надежные пароли, созданные Azure Active Directory длиной 16-64 символов.</span><span class="sxs-lookup"><span data-stu-id="92aef-149">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="92aef-150">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="92aef-150">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="92aef-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="92aef-151">Examples</span></span>

<span data-ttu-id="92aef-152">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="92aef-152">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="92aef-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="92aef-153">Request</span></span>

<span data-ttu-id="92aef-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92aef-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92aef-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="92aef-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_addpassword"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/addPassword
Content-type: application/json

{
  "passwordCredential": {
    "displayName": "Password friendly name"
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="92aef-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92aef-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="92aef-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="92aef-157">Response</span></span>

<span data-ttu-id="92aef-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="92aef-158">The following is an example of the response.</span></span>

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
  "description": "servicePrincipal: addPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

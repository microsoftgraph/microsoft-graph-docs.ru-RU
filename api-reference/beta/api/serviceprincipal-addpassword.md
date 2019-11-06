---
title: 'servicePrincipal: Аддпассворд'
description: Добавьте надежный пароль для servicePrincipal.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e2b279da894fcf47a778d194e833dfe5b1008f15
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997665"
---
# <a name="serviceprincipal-addpassword"></a><span data-ttu-id="fca68-103">servicePrincipal: Аддпассворд</span><span class="sxs-lookup"><span data-stu-id="fca68-103">servicePrincipal: addPassword</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fca68-104">Добавьте надежный пароль для объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="fca68-104">Add a strong password to a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fca68-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fca68-105">Permissions</span></span>

<span data-ttu-id="fca68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fca68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fca68-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fca68-108">Permission type</span></span>                        | <span data-ttu-id="fca68-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fca68-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fca68-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fca68-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fca68-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fca68-111">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="fca68-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fca68-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fca68-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fca68-113">Not supported.</span></span> |
| <span data-ttu-id="fca68-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fca68-114">Application</span></span>                            | <span data-ttu-id="fca68-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fca68-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fca68-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fca68-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="fca68-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fca68-117">Request headers</span></span>

| <span data-ttu-id="fca68-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fca68-118">Name</span></span>           | <span data-ttu-id="fca68-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fca68-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="fca68-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fca68-120">Authorization</span></span>  | <span data-ttu-id="fca68-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fca68-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fca68-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fca68-123">Content-type</span></span>   | <span data-ttu-id="fca68-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fca68-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fca68-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fca68-126">Request body</span></span>

<span data-ttu-id="fca68-127">В тексте запроса укажите необязательный `passwordCredential` объект со следующими свойствами.</span><span class="sxs-lookup"><span data-stu-id="fca68-127">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="fca68-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="fca68-128">Property</span></span>     | <span data-ttu-id="fca68-129">Тип</span><span class="sxs-lookup"><span data-stu-id="fca68-129">Type</span></span>   |<span data-ttu-id="fca68-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fca68-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fca68-131">displayName</span><span class="sxs-lookup"><span data-stu-id="fca68-131">displayName</span></span> | <span data-ttu-id="fca68-132">String</span><span class="sxs-lookup"><span data-stu-id="fca68-132">String</span></span> | <span data-ttu-id="fca68-133">Понятное имя для пароля.</span><span class="sxs-lookup"><span data-stu-id="fca68-133">Friendly name for the password.</span></span> <span data-ttu-id="fca68-134">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fca68-134">Optional.</span></span> |
| <span data-ttu-id="fca68-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fca68-135">endDateTime</span></span> | <span data-ttu-id="fca68-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fca68-136">DateTimeOffset</span></span> | <span data-ttu-id="fca68-137">Дата и время истечения срока действия пароля, представленного в формате ISO 8601, и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="fca68-137">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fca68-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fca68-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="fca68-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fca68-139">Optional.</span></span> |
| <span data-ttu-id="fca68-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fca68-140">startDateTime</span></span> | <span data-ttu-id="fca68-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fca68-141">DateTimeOffset</span></span> | <span data-ttu-id="fca68-142">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="fca68-142">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="fca68-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fca68-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fca68-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fca68-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="fca68-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fca68-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fca68-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="fca68-146">Response</span></span>

<span data-ttu-id="fca68-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [пассвордкредентиал](../resources/passwordcredential.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fca68-147">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="fca68-148">Свойство **секреттекст** в объекте Response содержит надежные пароли, созданные Azure Active Directory длиной 16-64 символов.</span><span class="sxs-lookup"><span data-stu-id="fca68-148">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="fca68-149">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="fca68-149">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="fca68-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="fca68-150">Examples</span></span>

<span data-ttu-id="fca68-151">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="fca68-151">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="fca68-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="fca68-152">Request</span></span>

<span data-ttu-id="fca68-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fca68-153">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fca68-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="fca68-154">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fca68-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fca68-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fca68-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="fca68-156">Response</span></span>

<span data-ttu-id="fca68-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fca68-157">The following is an example of the response.</span></span>

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

---
title: 'servicePrincipal: addPassword'
description: Добавление стойкого пароля объекту servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 167ad25cc11dc7fe730ad863af95f2303d7ab178
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131966"
---
# <a name="serviceprincipal-addpassword"></a><span data-ttu-id="6525d-103">servicePrincipal: addPassword</span><span class="sxs-lookup"><span data-stu-id="6525d-103">servicePrincipal: addPassword</span></span>

<span data-ttu-id="6525d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6525d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6525d-105">Добавьте надежный пароль в [объект servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="6525d-105">Add a strong password to a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6525d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6525d-106">Permissions</span></span>

<span data-ttu-id="6525d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6525d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6525d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6525d-109">Permission type</span></span>                        | <span data-ttu-id="6525d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6525d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6525d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6525d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6525d-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6525d-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="6525d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6525d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6525d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6525d-114">Not supported.</span></span> |
| <span data-ttu-id="6525d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6525d-115">Application</span></span>                            | <span data-ttu-id="6525d-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6525d-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6525d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6525d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="6525d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6525d-118">Request headers</span></span>

| <span data-ttu-id="6525d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6525d-119">Name</span></span>           | <span data-ttu-id="6525d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6525d-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="6525d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6525d-121">Authorization</span></span>  | <span data-ttu-id="6525d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6525d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6525d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6525d-124">Content-Type</span></span>   | <span data-ttu-id="6525d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6525d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6525d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6525d-127">Request body</span></span>

<span data-ttu-id="6525d-128">В теле запроса укажив необязательный `passwordCredential` объект со следующими свойствами.</span><span class="sxs-lookup"><span data-stu-id="6525d-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="6525d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6525d-129">Property</span></span>     | <span data-ttu-id="6525d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6525d-130">Type</span></span>   |<span data-ttu-id="6525d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6525d-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6525d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6525d-132">displayName</span></span> | <span data-ttu-id="6525d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6525d-133">String</span></span> | <span data-ttu-id="6525d-134">Удобное имя пароля.</span><span class="sxs-lookup"><span data-stu-id="6525d-134">Friendly name for the password.</span></span> <span data-ttu-id="6525d-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6525d-135">Optional.</span></span> |
| <span data-ttu-id="6525d-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6525d-136">endDateTime</span></span> | <span data-ttu-id="6525d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6525d-137">DateTimeOffset</span></span> | <span data-ttu-id="6525d-138">Дата и время истечения срока действия пароля представлены в формате ISO 8601 и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6525d-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6525d-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6525d-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="6525d-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6525d-140">Optional.</span></span> <span data-ttu-id="6525d-141">Значение по умолчанию : startDateTime + 2 years.</span><span class="sxs-lookup"><span data-stu-id="6525d-141">The default value is "startDateTime + 2 years".</span></span> |
| <span data-ttu-id="6525d-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6525d-142">startDateTime</span></span> | <span data-ttu-id="6525d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6525d-143">DateTimeOffset</span></span> | <span data-ttu-id="6525d-144">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="6525d-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="6525d-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6525d-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6525d-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6525d-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="6525d-147">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6525d-147">Optional.</span></span> <span data-ttu-id="6525d-148">Значение по умолчанию — "now".</span><span class="sxs-lookup"><span data-stu-id="6525d-148">The default value is "now".</span></span> |

## <a name="response"></a><span data-ttu-id="6525d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="6525d-149">Response</span></span>

<span data-ttu-id="6525d-150">В случае успеха этот метод возвращает код отклика и новый `200 OK` [объект passwordCredential](../resources/passwordcredential.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6525d-150">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="6525d-151">Свойство **secretText** в объекте ответа содержит надежные пароли, созданные Azure Active Directory длиной от 16 до 64 символов.</span><span class="sxs-lookup"><span data-stu-id="6525d-151">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="6525d-152">В будущем получить этот пароль не будет.</span><span class="sxs-lookup"><span data-stu-id="6525d-152">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="6525d-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="6525d-153">Examples</span></span>

<span data-ttu-id="6525d-154">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="6525d-154">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6525d-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="6525d-155">Request</span></span>

<span data-ttu-id="6525d-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6525d-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6525d-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="6525d-157">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="6525d-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6525d-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6525d-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="6525d-159">Response</span></span>

<span data-ttu-id="6525d-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6525d-160">The following is an example of the response.</span></span>

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




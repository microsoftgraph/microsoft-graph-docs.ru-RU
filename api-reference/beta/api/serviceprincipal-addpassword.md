---
title: 'servicePrincipal: Аддпассворд'
description: Добавьте надежный пароль для servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 781cb68eb8f73440972485e4151e23eb345425e2
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219111"
---
# <a name="serviceprincipal-addpassword"></a><span data-ttu-id="a5376-103">servicePrincipal: Аддпассворд</span><span class="sxs-lookup"><span data-stu-id="a5376-103">servicePrincipal: addPassword</span></span>

<span data-ttu-id="a5376-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5376-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5376-105">Добавьте надежный пароль для объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="a5376-105">Add a strong password to a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5376-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5376-106">Permissions</span></span>

<span data-ttu-id="a5376-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5376-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5376-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5376-109">Permission type</span></span>                        | <span data-ttu-id="a5376-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5376-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a5376-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5376-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5376-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5376-112">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="a5376-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5376-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5376-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5376-114">Not supported.</span></span> |
| <span data-ttu-id="a5376-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5376-115">Application</span></span>                            | <span data-ttu-id="a5376-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5376-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5376-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5376-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="a5376-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5376-118">Request headers</span></span>

| <span data-ttu-id="a5376-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a5376-119">Name</span></span>           | <span data-ttu-id="a5376-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a5376-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="a5376-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5376-121">Authorization</span></span>  | <span data-ttu-id="a5376-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5376-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a5376-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5376-124">Content-type</span></span>   | <span data-ttu-id="a5376-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5376-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5376-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5376-127">Request body</span></span>

<span data-ttu-id="a5376-128">В тексте запроса укажите необязательный `passwordCredential` объект со следующими свойствами.</span><span class="sxs-lookup"><span data-stu-id="a5376-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="a5376-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5376-129">Property</span></span>     | <span data-ttu-id="a5376-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a5376-130">Type</span></span>   |<span data-ttu-id="a5376-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a5376-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5376-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a5376-132">displayName</span></span> | <span data-ttu-id="a5376-133">String</span><span class="sxs-lookup"><span data-stu-id="a5376-133">String</span></span> | <span data-ttu-id="a5376-134">Понятное имя для пароля.</span><span class="sxs-lookup"><span data-stu-id="a5376-134">Friendly name for the password.</span></span> <span data-ttu-id="a5376-135">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="a5376-135">Optional.</span></span> |
| <span data-ttu-id="a5376-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a5376-136">endDateTime</span></span> | <span data-ttu-id="a5376-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5376-137">DateTimeOffset</span></span> | <span data-ttu-id="a5376-138">Дата и время истечения срока действия пароля, представленного в формате ISO 8601, и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="a5376-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a5376-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a5376-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a5376-140">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="a5376-140">Optional.</span></span> |
| <span data-ttu-id="a5376-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a5376-141">startDateTime</span></span> | <span data-ttu-id="a5376-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5376-142">DateTimeOffset</span></span> | <span data-ttu-id="a5376-143">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="a5376-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="a5376-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a5376-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a5376-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a5376-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a5376-146">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a5376-146">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a5376-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5376-147">Response</span></span>

<span data-ttu-id="a5376-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [пассвордкредентиал](../resources/passwordcredential.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a5376-148">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="a5376-149">Свойство **секреттекст** в объекте Response содержит надежные пароли, созданные Azure Active Directory длиной 16-64 символов.</span><span class="sxs-lookup"><span data-stu-id="a5376-149">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="a5376-150">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="a5376-150">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="a5376-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="a5376-151">Examples</span></span>

<span data-ttu-id="a5376-152">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="a5376-152">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a5376-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5376-153">Request</span></span>

<span data-ttu-id="a5376-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5376-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5376-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5376-155">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="a5376-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5376-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a5376-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5376-157">Response</span></span>

<span data-ttu-id="a5376-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5376-158">The following is an example of the response.</span></span>

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

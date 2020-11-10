---
title: Получение Пассвордаусентикатионмесод
description: Получение свойств и связей объекта пассвордаусентикатионмесод.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 44506848052e07d0cfb006b68d6a6052e4863436
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973068"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="2c3f3-103">Получение Пассвордаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="2c3f3-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="2c3f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c3f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c3f3-105">Получение свойств и связей объекта [метода проверки подлинности](../resources/passwordauthenticationmethod.md) с помощью пароля.</span><span class="sxs-lookup"><span data-stu-id="2c3f3-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2c3f3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c3f3-106">Permissions</span></span>

<span data-ttu-id="2c3f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c3f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c3f3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c3f3-109">Permission type</span></span>                        | <span data-ttu-id="2c3f3-110">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="2c3f3-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="2c3f3-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="2c3f3-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="2c3f3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c3f3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c3f3-113">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2c3f3-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="2c3f3-114">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2c3f3-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="2c3f3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c3f3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c3f3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c3f3-116">Not supported.</span></span> | <span data-ttu-id="2c3f3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c3f3-117">Not supported.</span></span> |
| <span data-ttu-id="2c3f3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c3f3-118">Application</span></span>                            | <span data-ttu-id="2c3f3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c3f3-119">Not supported.</span></span> | <span data-ttu-id="2c3f3-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c3f3-120">Not supported.</span></span> |

<span data-ttu-id="2c3f3-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="2c3f3-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="2c3f3-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2c3f3-122">Global admin</span></span>
* <span data-ttu-id="2c3f3-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="2c3f3-123">Global reader</span></span>
* <span data-ttu-id="2c3f3-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2c3f3-124">Privileged authentication admin</span></span>
* <span data-ttu-id="2c3f3-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2c3f3-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="2c3f3-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c3f3-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c3f3-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2c3f3-127">Optional query parameters</span></span>

<span data-ttu-id="2c3f3-128">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2c3f3-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c3f3-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c3f3-129">Request headers</span></span>

| <span data-ttu-id="2c3f3-130">Имя</span><span class="sxs-lookup"><span data-stu-id="2c3f3-130">Name</span></span>      |<span data-ttu-id="2c3f3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2c3f3-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2c3f3-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c3f3-132">Authorization</span></span> | <span data-ttu-id="2c3f3-133">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="2c3f3-133">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c3f3-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c3f3-134">Request body</span></span>

<span data-ttu-id="2c3f3-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c3f3-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c3f3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c3f3-136">Response</span></span>

<span data-ttu-id="2c3f3-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [пассвордаусентикатионмесод](../resources/passwordauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c3f3-137">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c3f3-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="2c3f3-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2c3f3-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c3f3-139">Request</span></span>

<span data-ttu-id="2c3f3-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c3f3-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c3f3-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c3f3-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="2c3f3-142">C#</span><span class="sxs-lookup"><span data-stu-id="2c3f3-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c3f3-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c3f3-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c3f3-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c3f3-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c3f3-145">Java</span><span class="sxs-lookup"><span data-stu-id="2c3f3-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2c3f3-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c3f3-146">Response</span></span>

<span data-ttu-id="2c3f3-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2c3f3-147">The following is an example of the response.</span></span>

> <span data-ttu-id="2c3f3-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c3f3-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "28c10230-6103-485e-b985-444c60001490",
  "password": null,
  "creationDateTime": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get passwordAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

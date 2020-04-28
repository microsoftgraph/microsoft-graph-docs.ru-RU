---
title: Получение Пассвордаусентикатионмесод
description: Получение свойств и связей объекта пассвордаусентикатионмесод.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7c11a59c4c63aa27df759e462fbc0f7fdea7c2c8
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806523"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="4cbf2-103">Получение Пассвордаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="4cbf2-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="4cbf2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cbf2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cbf2-105">Получение свойств и связей объекта [метода проверки подлинности](../resources/passwordauthenticationmethod.md) с помощью пароля.</span><span class="sxs-lookup"><span data-stu-id="4cbf2-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4cbf2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4cbf2-106">Permissions</span></span>

<span data-ttu-id="4cbf2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cbf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4cbf2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cbf2-109">Permission type</span></span>                        | <span data-ttu-id="4cbf2-110">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="4cbf2-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="4cbf2-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="4cbf2-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="4cbf2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cbf2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4cbf2-113">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4cbf2-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="4cbf2-114">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4cbf2-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="4cbf2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cbf2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cbf2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cbf2-116">Not supported.</span></span> | <span data-ttu-id="4cbf2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cbf2-117">Not supported.</span></span> |
| <span data-ttu-id="4cbf2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cbf2-118">Application</span></span>                            | <span data-ttu-id="4cbf2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cbf2-119">Not supported.</span></span> | <span data-ttu-id="4cbf2-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cbf2-120">Not supported.</span></span> |

<span data-ttu-id="4cbf2-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="4cbf2-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="4cbf2-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="4cbf2-122">Global admin</span></span>
* <span data-ttu-id="4cbf2-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="4cbf2-123">Global reader</span></span>
* <span data-ttu-id="4cbf2-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="4cbf2-124">Privileged authentication admin</span></span>
* <span data-ttu-id="4cbf2-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="4cbf2-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="4cbf2-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cbf2-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4cbf2-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4cbf2-127">Optional query parameters</span></span>

<span data-ttu-id="4cbf2-128">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4cbf2-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4cbf2-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cbf2-129">Request headers</span></span>

| <span data-ttu-id="4cbf2-130">Имя</span><span class="sxs-lookup"><span data-stu-id="4cbf2-130">Name</span></span>      |<span data-ttu-id="4cbf2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4cbf2-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4cbf2-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cbf2-132">Authorization</span></span> | <span data-ttu-id="4cbf2-133">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="4cbf2-133">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4cbf2-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4cbf2-134">Request body</span></span>

<span data-ttu-id="4cbf2-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4cbf2-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cbf2-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cbf2-136">Response</span></span>

<span data-ttu-id="4cbf2-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [пассвордаусентикатионмесод](../resources/passwordauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4cbf2-137">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4cbf2-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="4cbf2-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4cbf2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cbf2-139">Request</span></span>

<span data-ttu-id="4cbf2-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cbf2-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4cbf2-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="4cbf2-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="4cbf2-142">C#</span><span class="sxs-lookup"><span data-stu-id="4cbf2-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4cbf2-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4cbf2-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4cbf2-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4cbf2-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4cbf2-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cbf2-145">Response</span></span>

<span data-ttu-id="4cbf2-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4cbf2-146">The following is an example of the response.</span></span>

> <span data-ttu-id="4cbf2-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cbf2-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

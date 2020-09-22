---
title: Получение Фонеаусентикатионмесод
description: Получение одного объекта Фонеаусентикатионмесод.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f7592eb2ec463d1cf540ad7f42fbe676c4b0ee0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010619"
---
# <a name="get-phoneauthenticationmethod"></a><span data-ttu-id="a5807-103">Получение Фонеаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="a5807-103">Get phoneAuthenticationMethod</span></span>

<span data-ttu-id="a5807-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5807-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5807-105">Получение одного объекта [фонеаусентикатионмесод](../resources/phoneauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="a5807-105">Retrieve a single [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5807-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5807-106">Permissions</span></span>

<span data-ttu-id="a5807-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5807-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5807-109">Permission type</span></span>                        | <span data-ttu-id="a5807-110">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="a5807-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="a5807-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="a5807-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="a5807-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5807-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5807-113">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a5807-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="a5807-114">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a5807-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="a5807-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5807-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5807-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5807-116">Not supported.</span></span> | <span data-ttu-id="a5807-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5807-117">Not supported.</span></span> |
| <span data-ttu-id="a5807-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5807-118">Application</span></span>                            | <span data-ttu-id="a5807-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5807-119">Not supported.</span></span> | <span data-ttu-id="a5807-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5807-120">Not supported.</span></span> |

<span data-ttu-id="a5807-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="a5807-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="a5807-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a5807-122">Global admin</span></span>
* <span data-ttu-id="a5807-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="a5807-123">Global reader</span></span>
* <span data-ttu-id="a5807-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="a5807-124">Privileged authentication admin</span></span>
* <span data-ttu-id="a5807-125">Администратор проверки подлинности (видит только скрытые номера телефонов)</span><span class="sxs-lookup"><span data-stu-id="a5807-125">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="a5807-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5807-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods/{id}
GET /users/{id}/authentication/phoneMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5807-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a5807-127">Optional query parameters</span></span>

<span data-ttu-id="a5807-128">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a5807-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5807-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5807-129">Request headers</span></span>

| <span data-ttu-id="a5807-130">Имя</span><span class="sxs-lookup"><span data-stu-id="a5807-130">Name</span></span>      |<span data-ttu-id="a5807-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a5807-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5807-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5807-132">Authorization</span></span> | <span data-ttu-id="a5807-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5807-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5807-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5807-135">Request body</span></span>

<span data-ttu-id="a5807-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5807-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5807-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5807-137">Response</span></span>

<span data-ttu-id="a5807-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [фонеаусентикатионмесод](../resources/phoneauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a5807-138">If successful, this method returns a `200 OK` response code and the requested [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5807-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="a5807-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5807-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5807-140">Request</span></span>

<span data-ttu-id="a5807-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5807-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5807-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5807-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phoneauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="a5807-143">C#</span><span class="sxs-lookup"><span data-stu-id="a5807-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5807-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5807-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5807-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5807-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a5807-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5807-146">Response</span></span>

<span data-ttu-id="a5807-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a5807-147">The following is an example of the response.</span></span>

> <span data-ttu-id="a5807-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5807-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



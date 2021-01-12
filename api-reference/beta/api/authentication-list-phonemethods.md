---
title: Список phoneMethods
description: Получить список объектов метода проверки подлинности телефона.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5331de660e5b81a2908693e9377872ce64e3f678
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796480"
---
# <a name="list-phonemethods"></a><span data-ttu-id="d9dc0-103">Список phoneMethods</span><span class="sxs-lookup"><span data-stu-id="d9dc0-103">List phoneMethods</span></span>

<span data-ttu-id="d9dc0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9dc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9dc0-105">Получить список объектов метода [проверки подлинности](../resources/phoneauthenticationmethod.md) телефона.</span><span class="sxs-lookup"><span data-stu-id="d9dc0-105">Retrieve a list of [phone authentication method](../resources/phoneauthenticationmethod.md) objects.</span></span> <span data-ttu-id="d9dc0-106">Это возвратит до трех объектов, так как у пользователя может быть до трех телефонов, которые можно использовать для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d9dc0-106">This will return up to three objects, as a user can have up to three phones usable for authentication.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9dc0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9dc0-107">Permissions</span></span>

<span data-ttu-id="d9dc0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9dc0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9dc0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9dc0-110">Permission type</span></span>                        | <span data-ttu-id="d9dc0-111">Разрешения, действующие на себя (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="d9dc0-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="d9dc0-112">Разрешения, действующие над другими (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="d9dc0-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="d9dc0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9dc0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9dc0-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9dc0-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="d9dc0-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9dc0-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="d9dc0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9dc0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9dc0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9dc0-117">Not supported.</span></span> | <span data-ttu-id="d9dc0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9dc0-118">Not supported.</span></span> |
| <span data-ttu-id="d9dc0-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="d9dc0-119">Application</span></span>                            | <span data-ttu-id="d9dc0-120">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="d9dc0-120">Not applicable.</span></span> | <span data-ttu-id="d9dc0-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9dc0-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="d9dc0-122">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="d9dc0-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="d9dc0-123">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d9dc0-123">Global admin</span></span>
* <span data-ttu-id="d9dc0-124">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="d9dc0-124">Global reader</span></span>
* <span data-ttu-id="d9dc0-125">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="d9dc0-125">Privileged authentication admin</span></span>
* <span data-ttu-id="d9dc0-126">Администратор проверки подлинности (видит только маскирование номеров телефонов)</span><span class="sxs-lookup"><span data-stu-id="d9dc0-126">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="d9dc0-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9dc0-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods
GET /users/{id | userPrincipalName}/authentication/phoneMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9dc0-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d9dc0-128">Optional query parameters</span></span>

<span data-ttu-id="d9dc0-129">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d9dc0-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9dc0-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9dc0-130">Request headers</span></span>

| <span data-ttu-id="d9dc0-131">Имя</span><span class="sxs-lookup"><span data-stu-id="d9dc0-131">Name</span></span>      |<span data-ttu-id="d9dc0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d9dc0-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d9dc0-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9dc0-133">Authorization</span></span> | <span data-ttu-id="d9dc0-134">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="d9dc0-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9dc0-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9dc0-135">Request body</span></span>

<span data-ttu-id="d9dc0-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d9dc0-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9dc0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9dc0-137">Response</span></span>

<span data-ttu-id="d9dc0-138">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d9dc0-138">If successful, this method returns a `200 OK` response code and a collection of [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9dc0-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="d9dc0-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9dc0-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9dc0-140">Request</span></span>

<span data-ttu-id="d9dc0-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9dc0-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9dc0-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9dc0-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phonemethods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods
```
# <a name="c"></a>[<span data-ttu-id="d9dc0-143">C#</span><span class="sxs-lookup"><span data-stu-id="d9dc0-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phonemethods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9dc0-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9dc0-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phonemethods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9dc0-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9dc0-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phonemethods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9dc0-146">Java</span><span class="sxs-lookup"><span data-stu-id="d9dc0-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phonemethods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d9dc0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9dc0-147">Response</span></span>

<span data-ttu-id="d9dc0-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d9dc0-148">The following is an example of the response.</span></span>

> <span data-ttu-id="d9dc0-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9dc0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "phoneNumber": "+1 2065555555",
      "phoneType": "mobile",
      "smsSignInState": "ready",
      "id": "3179e48a-750b-4051-897c-87b9720928f7"
    },
    {
      "phoneNumber": "+1 2065555556",
      "phoneType": "alternateMobile",
      "smsSignInState": "notSupported",
      "id": "b6332ec1-7057-4abe-9331-3d72feddfe41"
    },
    {
      "phoneNumber": "+1 2065555557",
      "phoneType": "office",
      "smsSignInState": "notSupported",
      "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List phoneMethods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

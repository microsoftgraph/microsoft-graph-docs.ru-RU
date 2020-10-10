---
title: 'Фонеаусентикатионмесод: Енаблесмссигнин'
description: Включите вход в SMS для мобильного телефона.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75236ca18c192b1168a83a896269e4fd3b1c6675
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48417830"
---
# <a name="phoneauthenticationmethod-enablesmssignin"></a><span data-ttu-id="4439e-103">Фонеаусентикатионмесод: Енаблесмссигнин</span><span class="sxs-lookup"><span data-stu-id="4439e-103">phoneAuthenticationMethod: enableSmsSignIn</span></span>

<span data-ttu-id="4439e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4439e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4439e-105">Включите вход в SMS для существующего `mobile` номера телефона.</span><span class="sxs-lookup"><span data-stu-id="4439e-105">Enable SMS sign-in for an existing `mobile` phone number.</span></span> <span data-ttu-id="4439e-106">Успешное включение:</span><span class="sxs-lookup"><span data-stu-id="4439e-106">To be successfully enabled:</span></span>

* <span data-ttu-id="4439e-107">Телефон должен иметь значение `"phoneType": "mobile"` .</span><span class="sxs-lookup"><span data-stu-id="4439e-107">The phone must have `"phoneType": "mobile"`.</span></span>
* <span data-ttu-id="4439e-108">Телефон должен быть уникальным в системе входа SMS (никто другой не может использовать этот номер).</span><span class="sxs-lookup"><span data-stu-id="4439e-108">The phone must be unique in the SMS sign-in system (no one else can also be using that number).</span></span>
* <span data-ttu-id="4439e-109">Пользователю необходимо включить вход в систему SMS в политике [методы проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) .</span><span class="sxs-lookup"><span data-stu-id="4439e-109">The user must be enabled for SMS sign-in in the [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="4439e-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4439e-110">Permissions</span></span>

<span data-ttu-id="4439e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4439e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4439e-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4439e-113">Permission type</span></span>                        | <span data-ttu-id="4439e-114">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="4439e-114">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="4439e-115">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="4439e-115">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="4439e-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4439e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="4439e-117">Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4439e-117">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="4439e-118">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4439e-118">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="4439e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4439e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4439e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4439e-120">Not supported.</span></span> | <span data-ttu-id="4439e-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4439e-121">Not supported.</span></span> |
| <span data-ttu-id="4439e-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4439e-122">Application</span></span>                            | <span data-ttu-id="4439e-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4439e-123">Not supported.</span></span> | <span data-ttu-id="4439e-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4439e-124">Not supported.</span></span> |

<span data-ttu-id="4439e-125">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="4439e-125">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="4439e-126">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="4439e-126">Global admin</span></span>
* <span data-ttu-id="4439e-127">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="4439e-127">Privileged authentication admin</span></span>
* <span data-ttu-id="4439e-128">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="4439e-128">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="4439e-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4439e-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/enableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/enableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="4439e-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4439e-130">Request headers</span></span>

| <span data-ttu-id="4439e-131">Имя</span><span class="sxs-lookup"><span data-stu-id="4439e-131">Name</span></span>          | <span data-ttu-id="4439e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4439e-132">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4439e-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4439e-133">Authorization</span></span> | <span data-ttu-id="4439e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4439e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4439e-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4439e-136">Request body</span></span>

<span data-ttu-id="4439e-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4439e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4439e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4439e-138">Response</span></span>

<span data-ttu-id="4439e-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4439e-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4439e-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="4439e-141">Examples</span></span>

<span data-ttu-id="4439e-142">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4439e-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4439e-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4439e-143">Request</span></span>

<span data-ttu-id="4439e-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4439e-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4439e-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4439e-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_enablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="4439e-146">C#</span><span class="sxs-lookup"><span data-stu-id="4439e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-enablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4439e-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4439e-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-enablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4439e-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4439e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-enablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4439e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4439e-149">Response</span></span>

<span data-ttu-id="4439e-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4439e-150">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod: enableSmsSignIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
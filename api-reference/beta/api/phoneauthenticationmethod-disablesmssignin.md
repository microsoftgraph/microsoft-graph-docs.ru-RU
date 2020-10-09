---
title: 'Фонеаусентикатионмесод: Дисаблесмссигнин'
description: Отключение входа в SMS для мобильного телефона
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 953c417b53dd21d294dd00607e9adaf0ed22babd
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402669"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="5bc99-103">Фонеаусентикатионмесод: Дисаблесмссигнин</span><span class="sxs-lookup"><span data-stu-id="5bc99-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="5bc99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bc99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bc99-105">Отключить вход в SMS для существующего `mobile` номера телефона.</span><span class="sxs-lookup"><span data-stu-id="5bc99-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="5bc99-106">**Примечание:** Этот номер больше не будет доступен для входа в SMS, что может препятствовать входу пользователя в систему.</span><span class="sxs-lookup"><span data-stu-id="5bc99-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bc99-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5bc99-107">Permissions</span></span>

<span data-ttu-id="5bc99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bc99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5bc99-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bc99-110">Permission type</span></span>                        | <span data-ttu-id="5bc99-111">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="5bc99-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="5bc99-112">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="5bc99-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="5bc99-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bc99-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5bc99-114">Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5bc99-114">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="5bc99-115">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5bc99-115">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="5bc99-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bc99-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bc99-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bc99-117">Not supported.</span></span> | <span data-ttu-id="5bc99-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bc99-118">Not supported.</span></span> |
| <span data-ttu-id="5bc99-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bc99-119">Application</span></span>                            | <span data-ttu-id="5bc99-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bc99-120">Not supported.</span></span> | <span data-ttu-id="5bc99-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bc99-121">Not supported.</span></span> |

<span data-ttu-id="5bc99-122">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="5bc99-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="5bc99-123">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="5bc99-123">Global admin</span></span>
* <span data-ttu-id="5bc99-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="5bc99-124">Privileged authentication admin</span></span>
* <span data-ttu-id="5bc99-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="5bc99-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="5bc99-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bc99-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="5bc99-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bc99-127">Request headers</span></span>

| <span data-ttu-id="5bc99-128">Имя</span><span class="sxs-lookup"><span data-stu-id="5bc99-128">Name</span></span>          | <span data-ttu-id="5bc99-129">Описание</span><span class="sxs-lookup"><span data-stu-id="5bc99-129">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5bc99-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5bc99-130">Authorization</span></span> | <span data-ttu-id="5bc99-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bc99-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bc99-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5bc99-133">Request body</span></span>

<span data-ttu-id="5bc99-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bc99-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bc99-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bc99-135">Response</span></span>

<span data-ttu-id="5bc99-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5bc99-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5bc99-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="5bc99-138">Examples</span></span>

<span data-ttu-id="5bc99-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="5bc99-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5bc99-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bc99-140">Request</span></span>

<span data-ttu-id="5bc99-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bc99-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5bc99-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bc99-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="5bc99-143">C#</span><span class="sxs-lookup"><span data-stu-id="5bc99-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-disablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bc99-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bc99-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-disablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bc99-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bc99-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-disablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5bc99-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bc99-146">Response</span></span>

<span data-ttu-id="5bc99-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5bc99-147">The following is an example of the response.</span></span>
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
  "description": "phoneAuthenticationMethod: disableSmsSignIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
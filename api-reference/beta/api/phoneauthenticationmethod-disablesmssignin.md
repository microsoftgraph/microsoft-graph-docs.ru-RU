---
title: 'Фонеаусентикатионмесод: Дисаблесмссигнин'
description: Отключение входа в SMS для мобильного телефона
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dfb16775b2c4a452b3218e7fc4e19620e4174f16
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557782"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="8970f-103">Фонеаусентикатионмесод: Дисаблесмссигнин</span><span class="sxs-lookup"><span data-stu-id="8970f-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="8970f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8970f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8970f-105">Отключить вход в SMS для существующего `mobile` номера телефона.</span><span class="sxs-lookup"><span data-stu-id="8970f-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="8970f-106">**Примечание:** Этот номер больше не будет доступен для входа в SMS, что может препятствовать входу пользователя в систему.</span><span class="sxs-lookup"><span data-stu-id="8970f-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="8970f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8970f-107">Permissions</span></span>

<span data-ttu-id="8970f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8970f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8970f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8970f-110">Permission type</span></span>                        | <span data-ttu-id="8970f-111">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="8970f-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="8970f-112">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="8970f-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="8970f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8970f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8970f-114">Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8970f-114">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="8970f-115">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8970f-115">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="8970f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8970f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8970f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8970f-117">Not supported.</span></span> | <span data-ttu-id="8970f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8970f-118">Not supported.</span></span> |
| <span data-ttu-id="8970f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8970f-119">Application</span></span>                            | <span data-ttu-id="8970f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8970f-120">Not supported.</span></span> | <span data-ttu-id="8970f-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8970f-121">Not supported.</span></span> |

<span data-ttu-id="8970f-122">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="8970f-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="8970f-123">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8970f-123">Global admin</span></span>
* <span data-ttu-id="8970f-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="8970f-124">Privileged authentication admin</span></span>
* <span data-ttu-id="8970f-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="8970f-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="8970f-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8970f-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="8970f-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8970f-127">Request headers</span></span>

| <span data-ttu-id="8970f-128">Имя</span><span class="sxs-lookup"><span data-stu-id="8970f-128">Name</span></span>          | <span data-ttu-id="8970f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8970f-129">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8970f-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8970f-130">Authorization</span></span> | <span data-ttu-id="8970f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8970f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8970f-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8970f-133">Request body</span></span>

<span data-ttu-id="8970f-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8970f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8970f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8970f-135">Response</span></span>

<span data-ttu-id="8970f-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8970f-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8970f-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="8970f-138">Examples</span></span>

<span data-ttu-id="8970f-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8970f-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8970f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="8970f-140">Request</span></span>

<span data-ttu-id="8970f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8970f-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```

### <a name="response"></a><span data-ttu-id="8970f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8970f-142">Response</span></span>

<span data-ttu-id="8970f-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8970f-143">The following is an example of the response.</span></span>
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

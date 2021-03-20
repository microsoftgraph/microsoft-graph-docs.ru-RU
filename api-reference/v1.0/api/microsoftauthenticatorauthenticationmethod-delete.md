---
title: Удаление MicrosoftAuthenticatorAuthenticationMethod
description: Удаляет объект MicrosoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 848aa51dfa82d192b48c768a659f2da17fa71e94
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949046"
---
# <a name="delete-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="f48cf-103">Удаление MicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f48cf-103">Delete microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="f48cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f48cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f48cf-105">Удаляет объект [MicrosoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="f48cf-105">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f48cf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f48cf-106">Permissions</span></span>

<span data-ttu-id="f48cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f48cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="f48cf-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="f48cf-109">Permissions acting on self</span></span>

|<span data-ttu-id="f48cf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f48cf-110">Permission type</span></span>      | <span data-ttu-id="f48cf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f48cf-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="f48cf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f48cf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f48cf-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f48cf-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="f48cf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f48cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f48cf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f48cf-115">Not supported.</span></span> |
| <span data-ttu-id="f48cf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f48cf-116">Application</span></span>                            | <span data-ttu-id="f48cf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f48cf-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="f48cf-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="f48cf-118">Permissions acting on other users</span></span>

|<span data-ttu-id="f48cf-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f48cf-119">Permission type</span></span>      | <span data-ttu-id="f48cf-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f48cf-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="f48cf-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f48cf-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="f48cf-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f48cf-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="f48cf-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f48cf-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f48cf-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f48cf-124">Not supported.</span></span> |
| <span data-ttu-id="f48cf-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f48cf-125">Application</span></span>                            | <span data-ttu-id="f48cf-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f48cf-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="f48cf-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="f48cf-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="f48cf-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f48cf-128">Global admin</span></span>
* <span data-ttu-id="f48cf-129">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="f48cf-129">Privileged authentication admin</span></span>
* <span data-ttu-id="f48cf-130">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="f48cf-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="f48cf-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f48cf-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="f48cf-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f48cf-132">Request headers</span></span>
|<span data-ttu-id="f48cf-133">Имя</span><span class="sxs-lookup"><span data-stu-id="f48cf-133">Name</span></span>|<span data-ttu-id="f48cf-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f48cf-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f48cf-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f48cf-135">Authorization</span></span>|<span data-ttu-id="f48cf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f48cf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f48cf-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f48cf-138">Request body</span></span>
<span data-ttu-id="f48cf-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f48cf-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f48cf-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f48cf-140">Response</span></span>

<span data-ttu-id="f48cf-141">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f48cf-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f48cf-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="f48cf-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f48cf-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="f48cf-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="f48cf-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f48cf-144">Response</span></span>
<span data-ttu-id="f48cf-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f48cf-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


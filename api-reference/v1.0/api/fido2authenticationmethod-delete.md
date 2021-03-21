---
title: Удаление fido2AuthenticationMethod
description: Удаляет объект fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 26dc814b92a987d8868cf89d7802a601ef165dd9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964875"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="4f5c6-103">Удаление fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4f5c6-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="4f5c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f5c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f5c6-105">Удаляет объект метода проверки подлинности [ключа безопасности FIDO2 пользователя.](../resources/fido2authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="4f5c6-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f5c6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f5c6-106">Permissions</span></span>

<span data-ttu-id="4f5c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f5c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="4f5c6-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="4f5c6-109">Permissions acting on self</span></span>

|<span data-ttu-id="4f5c6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f5c6-110">Permission type</span></span>      | <span data-ttu-id="4f5c6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f5c6-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="4f5c6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f5c6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f5c6-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f5c6-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="4f5c6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f5c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f5c6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f5c6-115">Not supported.</span></span> |
| <span data-ttu-id="4f5c6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f5c6-116">Application</span></span>                            | <span data-ttu-id="4f5c6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f5c6-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="4f5c6-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="4f5c6-118">Permissions acting on other users</span></span>

|<span data-ttu-id="4f5c6-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f5c6-119">Permission type</span></span>      | <span data-ttu-id="4f5c6-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f5c6-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="4f5c6-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f5c6-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f5c6-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f5c6-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="4f5c6-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f5c6-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f5c6-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f5c6-124">Not supported.</span></span> |
| <span data-ttu-id="4f5c6-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f5c6-125">Application</span></span>                            | <span data-ttu-id="4f5c6-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f5c6-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="4f5c6-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="4f5c6-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="4f5c6-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="4f5c6-128">Global admin</span></span>
* <span data-ttu-id="4f5c6-129">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="4f5c6-129">Privileged authentication admin</span></span>
* <span data-ttu-id="4f5c6-130">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="4f5c6-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="4f5c6-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f5c6-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4f5c6-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f5c6-132">Request headers</span></span>
|<span data-ttu-id="4f5c6-133">Имя</span><span class="sxs-lookup"><span data-stu-id="4f5c6-133">Name</span></span>|<span data-ttu-id="4f5c6-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4f5c6-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4f5c6-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f5c6-135">Authorization</span></span>|<span data-ttu-id="4f5c6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f5c6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f5c6-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f5c6-138">Request body</span></span>
<span data-ttu-id="4f5c6-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f5c6-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f5c6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f5c6-140">Response</span></span>

<span data-ttu-id="4f5c6-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4f5c6-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f5c6-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="4f5c6-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f5c6-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f5c6-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4f5c6-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f5c6-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```

### <a name="response"></a><span data-ttu-id="4f5c6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f5c6-146">Response</span></span>
<span data-ttu-id="4f5c6-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4f5c6-147">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


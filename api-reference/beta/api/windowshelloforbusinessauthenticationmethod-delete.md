---
title: Удаление windowsHelloForBusinessAuthenticationMethod
description: Удаляет объект windowsHelloForBusinessAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d0412cc7bdc1ed20ddba80d70b992d3859ca507c
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873320"
---
# <a name="delete-windowshelloforbusinessauthenticationmethod"></a><span data-ttu-id="e13ac-103">Удаление windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e13ac-103">Delete windowsHelloForBusinessAuthenticationMethod</span></span>
<span data-ttu-id="e13ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e13ac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e13ac-105">Удаляет объект [windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="e13ac-105">Deletes a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e13ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e13ac-106">Permissions</span></span>

<span data-ttu-id="e13ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e13ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="e13ac-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="e13ac-109">Permissions acting on self</span></span>

|<span data-ttu-id="e13ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e13ac-110">Permission type</span></span>      | <span data-ttu-id="e13ac-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e13ac-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="e13ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e13ac-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e13ac-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e13ac-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="e13ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e13ac-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e13ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e13ac-115">Not supported.</span></span> |
| <span data-ttu-id="e13ac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e13ac-116">Application</span></span>                            | <span data-ttu-id="e13ac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e13ac-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="e13ac-118">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="e13ac-118">Permissions acting on other users</span></span>

|<span data-ttu-id="e13ac-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e13ac-119">Permission type</span></span>      | <span data-ttu-id="e13ac-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e13ac-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="e13ac-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e13ac-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="e13ac-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e13ac-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="e13ac-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e13ac-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e13ac-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e13ac-124">Not supported.</span></span> |
| <span data-ttu-id="e13ac-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="e13ac-125">Application</span></span>                            | <span data-ttu-id="e13ac-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e13ac-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="e13ac-127">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="e13ac-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="e13ac-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e13ac-128">Global admin</span></span>
* <span data-ttu-id="e13ac-129">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="e13ac-129">Privileged authentication admin</span></span>
* <span data-ttu-id="e13ac-130">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="e13ac-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="e13ac-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e13ac-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="e13ac-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e13ac-132">Request headers</span></span>
|<span data-ttu-id="e13ac-133">Имя</span><span class="sxs-lookup"><span data-stu-id="e13ac-133">Name</span></span>|<span data-ttu-id="e13ac-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e13ac-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e13ac-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e13ac-135">Authorization</span></span>|<span data-ttu-id="e13ac-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e13ac-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e13ac-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e13ac-138">Request body</span></span>
<span data-ttu-id="e13ac-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e13ac-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e13ac-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e13ac-140">Response</span></span>

<span data-ttu-id="e13ac-141">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e13ac-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e13ac-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="e13ac-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e13ac-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="e13ac-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="e13ac-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e13ac-144">Response</span></span>
<span data-ttu-id="e13ac-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e13ac-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


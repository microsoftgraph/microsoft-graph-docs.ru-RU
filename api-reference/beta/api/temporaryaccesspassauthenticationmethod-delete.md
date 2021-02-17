---
title: Удаление temporaryAccessPassAuthenticationMethod
description: Удаляет временный объектAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0aefe7a59e9fa0a13420182995bb60b0b7fe4121
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272665"
---
# <a name="delete-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="b4d1e-103">Удаление temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b4d1e-103">Delete temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="b4d1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4d1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4d1e-105">Удаление объекта [temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b4d1e-105">Delete a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="b4d1e-106">Несмотря на то что текущий временный проход доступа для пользователя действителен, его необходимо удалить, прежде чем можно будет создать новый временный проход доступа для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4d1e-106">While the current Temporary Access Pass on the user is valid, it needs to be deleted before a new Temporary Access Pass can be created on the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4d1e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4d1e-107">Permissions</span></span>
<span data-ttu-id="b4d1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4d1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="b4d1e-110">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="b4d1e-110">Permissions acting on self</span></span>

|<span data-ttu-id="b4d1e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4d1e-111">Permission type</span></span>      | <span data-ttu-id="b4d1e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4d1e-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b4d1e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4d1e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4d1e-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4d1e-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="b4d1e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4d1e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4d1e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4d1e-116">Not supported.</span></span> |
| <span data-ttu-id="b4d1e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4d1e-117">Application</span></span>                            | <span data-ttu-id="b4d1e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4d1e-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="b4d1e-119">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="b4d1e-119">Permissions acting on other users</span></span>

|<span data-ttu-id="b4d1e-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4d1e-120">Permission type</span></span>      | <span data-ttu-id="b4d1e-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4d1e-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="b4d1e-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4d1e-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4d1e-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4d1e-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b4d1e-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4d1e-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4d1e-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4d1e-125">Not supported.</span></span> |
| <span data-ttu-id="b4d1e-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4d1e-126">Application</span></span>                            | <span data-ttu-id="b4d1e-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4d1e-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b4d1e-128">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="b4d1e-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="b4d1e-129">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b4d1e-129">Global admin</span></span>
* <span data-ttu-id="b4d1e-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b4d1e-130">Privileged authentication admin</span></span>
* <span data-ttu-id="b4d1e-131">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b4d1e-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b4d1e-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4d1e-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{id}
DELETE /me/authentication/temporaryAccessPassMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b4d1e-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4d1e-133">Request headers</span></span>
|<span data-ttu-id="b4d1e-134">Имя</span><span class="sxs-lookup"><span data-stu-id="b4d1e-134">Name</span></span>|<span data-ttu-id="b4d1e-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b4d1e-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b4d1e-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4d1e-136">Authorization</span></span>|<span data-ttu-id="b4d1e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4d1e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4d1e-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4d1e-139">Request body</span></span>
<span data-ttu-id="b4d1e-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4d1e-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4d1e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4d1e-141">Response</span></span>

<span data-ttu-id="b4d1e-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b4d1e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4d1e-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="b4d1e-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4d1e-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4d1e-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_temporaryaccesspassauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/{id}
```


### <a name="response"></a><span data-ttu-id="b4d1e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4d1e-146">Response</span></span>
<span data-ttu-id="b4d1e-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b4d1e-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
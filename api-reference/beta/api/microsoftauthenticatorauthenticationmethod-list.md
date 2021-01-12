---
title: Список microsoftAuthenticatorAuthenticationMethods
description: Получите список объектов microsoftAuthenticatorAuthenticationMethod и их свойств.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a880cb5ac1b0594b46f4de3649fc5a07060eb8be
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796795"
---
# <a name="list-microsoftauthenticatorauthenticationmethods"></a><span data-ttu-id="4911c-103">Список microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="4911c-103">List microsoftAuthenticatorAuthenticationMethods</span></span>
<span data-ttu-id="4911c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4911c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4911c-105">Получите список объектов [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="4911c-105">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="4911c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4911c-106">Permissions</span></span>

<span data-ttu-id="4911c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4911c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="4911c-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="4911c-109">Permissions acting on self</span></span>

|<span data-ttu-id="4911c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4911c-110">Permission type</span></span>      | <span data-ttu-id="4911c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4911c-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="4911c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4911c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4911c-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4911c-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="4911c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4911c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4911c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4911c-115">Not supported.</span></span> |
| <span data-ttu-id="4911c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4911c-116">Application</span></span>                            | <span data-ttu-id="4911c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4911c-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="4911c-118">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="4911c-118">Permissions acting on other users</span></span>

|<span data-ttu-id="4911c-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4911c-119">Permission type</span></span>      | <span data-ttu-id="4911c-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4911c-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="4911c-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4911c-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="4911c-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4911c-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="4911c-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4911c-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4911c-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4911c-124">Not supported.</span></span> |
| <span data-ttu-id="4911c-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="4911c-125">Application</span></span>                            | <span data-ttu-id="4911c-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4911c-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="4911c-127">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="4911c-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="4911c-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="4911c-128">Global admin</span></span>
* <span data-ttu-id="4911c-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="4911c-129">Global reader</span></span>
* <span data-ttu-id="4911c-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="4911c-130">Privileged authentication admin</span></span>
* <span data-ttu-id="4911c-131">Администратор проверки подлинности (видит только маскирование номеров телефонов)</span><span class="sxs-lookup"><span data-stu-id="4911c-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="4911c-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4911c-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods
GET /user/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4911c-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4911c-133">Optional query parameters</span></span>

<span data-ttu-id="4911c-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4911c-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4911c-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4911c-135">Request headers</span></span>

|<span data-ttu-id="4911c-136">Имя</span><span class="sxs-lookup"><span data-stu-id="4911c-136">Name</span></span>|<span data-ttu-id="4911c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4911c-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4911c-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4911c-138">Authorization</span></span>|<span data-ttu-id="4911c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4911c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4911c-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4911c-141">Request body</span></span>

<span data-ttu-id="4911c-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4911c-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4911c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4911c-143">Response</span></span>

<span data-ttu-id="4911c-144">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4911c-144">If successful, this method returns a `200 OK` response code and a collection of [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4911c-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="4911c-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4911c-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="4911c-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/user/anirban@contoso.com/authentication/microsoftAuthenticatorMethods
```


### <a name="response"></a><span data-ttu-id="4911c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4911c-147">Response</span></span>
<span data-ttu-id="4911c-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4911c-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.microsoftAuthenticatorAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
      "id": "6803c096-c096-6803-96c0-036896c00368",
      "displayName": "Sandeep's iPhone",
      "deviceTag": "",
      "phoneAppVersion": "6.5.4",
      "createdDateTime": "2020-12-03T23:16:12Z"
    }
  ]
}
```


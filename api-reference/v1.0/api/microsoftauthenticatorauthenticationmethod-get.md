---
title: Get microsoftAuthenticatorAuthenticationMethod
description: Ознакомьтесь с свойствами и отношениями объекта MicrosoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 59a4fadb4658ee21f094bdc38e3b1eff6bd5cb7d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949043"
---
# <a name="get-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="843ea-103">Get microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="843ea-103">Get microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="843ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="843ea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="843ea-105">Ознакомьтесь с свойствами и отношениями объекта [MicrosoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="843ea-105">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="843ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="843ea-106">Permissions</span></span>

<span data-ttu-id="843ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="843ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="843ea-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="843ea-109">Permissions acting on self</span></span>

|<span data-ttu-id="843ea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="843ea-110">Permission type</span></span>      | <span data-ttu-id="843ea-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="843ea-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="843ea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="843ea-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="843ea-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="843ea-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="843ea-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="843ea-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="843ea-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="843ea-115">Not supported.</span></span> |
| <span data-ttu-id="843ea-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="843ea-116">Application</span></span>                            | <span data-ttu-id="843ea-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="843ea-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="843ea-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="843ea-118">Permissions acting on other users</span></span>

|<span data-ttu-id="843ea-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="843ea-119">Permission type</span></span>      | <span data-ttu-id="843ea-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="843ea-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="843ea-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="843ea-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="843ea-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="843ea-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="843ea-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="843ea-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="843ea-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="843ea-124">Not supported.</span></span> |
| <span data-ttu-id="843ea-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="843ea-125">Application</span></span>                            | <span data-ttu-id="843ea-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="843ea-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="843ea-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="843ea-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="843ea-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="843ea-128">Global admin</span></span>
* <span data-ttu-id="843ea-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="843ea-129">Global reader</span></span>
* <span data-ttu-id="843ea-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="843ea-130">Privileged authentication admin</span></span>
* <span data-ttu-id="843ea-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="843ea-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="843ea-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="843ea-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="843ea-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="843ea-133">Optional query parameters</span></span>
<span data-ttu-id="843ea-134">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="843ea-134">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="843ea-135">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="843ea-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="843ea-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="843ea-136">Request headers</span></span>
|<span data-ttu-id="843ea-137">Имя</span><span class="sxs-lookup"><span data-stu-id="843ea-137">Name</span></span>|<span data-ttu-id="843ea-138">Описание</span><span class="sxs-lookup"><span data-stu-id="843ea-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="843ea-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="843ea-139">Authorization</span></span>|<span data-ttu-id="843ea-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="843ea-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="843ea-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="843ea-142">Request body</span></span>
<span data-ttu-id="843ea-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="843ea-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="843ea-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="843ea-144">Response</span></span>

<span data-ttu-id="843ea-145">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект MicrosoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="843ea-145">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="843ea-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="843ea-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="843ea-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="843ea-147">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="843ea-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="843ea-148">Response</span></span>
<span data-ttu-id="843ea-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="843ea-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
    "id": "6803c096-c096-6803-96c0-036896c00368",
    "displayName": "Sandeep's iPhone",
    "deviceTag": "",
    "phoneAppVersion": "6.5.4",
    "createdDateTime": "2020-12-03T23:16:12Z"
  }
}
```

---
title: Get microsoftAuthenticatorAuthenticationMethod
description: Чтение свойств и связей объекта microsoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d676cab828c3e05122d699d060c2b41ea39bfd8
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796798"
---
# <a name="get-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="9ad2d-103">Get microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9ad2d-103">Get microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="9ad2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ad2d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ad2d-105">Чтение свойств и связей объекта [microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="9ad2d-105">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ad2d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ad2d-106">Permissions</span></span>

<span data-ttu-id="9ad2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ad2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="9ad2d-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="9ad2d-109">Permissions acting on self</span></span>

|<span data-ttu-id="9ad2d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ad2d-110">Permission type</span></span>      | <span data-ttu-id="9ad2d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ad2d-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9ad2d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ad2d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ad2d-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ad2d-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="9ad2d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ad2d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ad2d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ad2d-115">Not supported.</span></span> |
| <span data-ttu-id="9ad2d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ad2d-116">Application</span></span>                            | <span data-ttu-id="9ad2d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ad2d-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="9ad2d-118">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="9ad2d-118">Permissions acting on other users</span></span>

|<span data-ttu-id="9ad2d-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ad2d-119">Permission type</span></span>      | <span data-ttu-id="9ad2d-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ad2d-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="9ad2d-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ad2d-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ad2d-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ad2d-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="9ad2d-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ad2d-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ad2d-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ad2d-124">Not supported.</span></span> |
| <span data-ttu-id="9ad2d-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="9ad2d-125">Application</span></span>                            | <span data-ttu-id="9ad2d-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ad2d-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="9ad2d-127">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="9ad2d-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="9ad2d-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="9ad2d-128">Global admin</span></span>
* <span data-ttu-id="9ad2d-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="9ad2d-129">Global reader</span></span>
* <span data-ttu-id="9ad2d-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="9ad2d-130">Privileged authentication admin</span></span>
* <span data-ttu-id="9ad2d-131">Администратор проверки подлинности (видит только маскирование номеров телефонов)</span><span class="sxs-lookup"><span data-stu-id="9ad2d-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="9ad2d-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ad2d-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
GET /user/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ad2d-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9ad2d-133">Optional query parameters</span></span>
<span data-ttu-id="9ad2d-134">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9ad2d-134">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9ad2d-135">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9ad2d-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ad2d-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ad2d-136">Request headers</span></span>
|<span data-ttu-id="9ad2d-137">Имя</span><span class="sxs-lookup"><span data-stu-id="9ad2d-137">Name</span></span>|<span data-ttu-id="9ad2d-138">Описание</span><span class="sxs-lookup"><span data-stu-id="9ad2d-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9ad2d-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ad2d-139">Authorization</span></span>|<span data-ttu-id="9ad2d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ad2d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ad2d-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ad2d-142">Request body</span></span>
<span data-ttu-id="9ad2d-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ad2d-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ad2d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ad2d-144">Response</span></span>

<span data-ttu-id="9ad2d-145">В случае успеха этот метод возвращает код отклика и объект `200 OK` [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ad2d-145">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ad2d-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="9ad2d-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ad2d-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ad2d-147">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/user/anirban@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="9ad2d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ad2d-148">Response</span></span>
<span data-ttu-id="9ad2d-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9ad2d-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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

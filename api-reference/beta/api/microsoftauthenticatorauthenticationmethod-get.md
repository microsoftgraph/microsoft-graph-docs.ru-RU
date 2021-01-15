---
title: Get microsoftAuthenticatorAuthenticationMethod
description: Чтение свойств и связей объекта microsoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 76a192e9fd896f65deaba715b32cc8a0a4cad09a
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873446"
---
# <a name="get-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="04eae-103">Get microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="04eae-103">Get microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="04eae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04eae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="04eae-105">Чтение свойств и связей объекта [microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="04eae-105">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="04eae-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04eae-106">Permissions</span></span>

<span data-ttu-id="04eae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04eae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="04eae-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="04eae-109">Permissions acting on self</span></span>

|<span data-ttu-id="04eae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04eae-110">Permission type</span></span>      | <span data-ttu-id="04eae-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04eae-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="04eae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04eae-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="04eae-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04eae-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="04eae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04eae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04eae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04eae-115">Not supported.</span></span> |
| <span data-ttu-id="04eae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04eae-116">Application</span></span>                            | <span data-ttu-id="04eae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04eae-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="04eae-118">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="04eae-118">Permissions acting on other users</span></span>

|<span data-ttu-id="04eae-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04eae-119">Permission type</span></span>      | <span data-ttu-id="04eae-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04eae-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="04eae-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04eae-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="04eae-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04eae-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="04eae-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04eae-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04eae-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04eae-124">Not supported.</span></span> |
| <span data-ttu-id="04eae-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="04eae-125">Application</span></span>                            | <span data-ttu-id="04eae-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04eae-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="04eae-127">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="04eae-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="04eae-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="04eae-128">Global admin</span></span>
* <span data-ttu-id="04eae-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="04eae-129">Global reader</span></span>
* <span data-ttu-id="04eae-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="04eae-130">Privileged authentication admin</span></span>
* <span data-ttu-id="04eae-131">Администратор проверки подлинности (видит только маскирование номеров телефонов)</span><span class="sxs-lookup"><span data-stu-id="04eae-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="04eae-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04eae-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04eae-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="04eae-133">Optional query parameters</span></span>
<span data-ttu-id="04eae-134">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="04eae-134">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="04eae-135">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="04eae-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="04eae-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04eae-136">Request headers</span></span>
|<span data-ttu-id="04eae-137">Имя</span><span class="sxs-lookup"><span data-stu-id="04eae-137">Name</span></span>|<span data-ttu-id="04eae-138">Описание</span><span class="sxs-lookup"><span data-stu-id="04eae-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="04eae-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04eae-139">Authorization</span></span>|<span data-ttu-id="04eae-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04eae-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04eae-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04eae-142">Request body</span></span>
<span data-ttu-id="04eae-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04eae-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04eae-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="04eae-144">Response</span></span>

<span data-ttu-id="04eae-145">В случае успеха этот метод возвращает код отклика и объект `200 OK` [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04eae-145">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04eae-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="04eae-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04eae-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="04eae-147">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="04eae-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="04eae-148">Response</span></span>
<span data-ttu-id="04eae-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="04eae-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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

---
title: Обновление microsoftAuthenticatorAuthenticationMethodConfiguration
description: Обновление свойств объекта microsoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6d715e32d2e42a81cf042884ab38d4f06097a3f
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874508"
---
# <a name="update-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="78425-103">Обновление microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="78425-103">Update microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="78425-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78425-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78425-105">Обновление свойств объекта [microsoftAuthenticatorAuthenticationMethodConfiguration,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности Microsoft Authenticator для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="78425-105">Update the properties of a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>


## <a name="permissions"></a><span data-ttu-id="78425-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78425-106">Permissions</span></span>
<span data-ttu-id="78425-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78425-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78425-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78425-109">Permission type</span></span>|<span data-ttu-id="78425-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78425-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78425-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78425-111">Delegated (work or school account)</span></span>|<span data-ttu-id="78425-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="78425-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="78425-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78425-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78425-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78425-114">Not supported.</span></span>|
|<span data-ttu-id="78425-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78425-115">Application</span></span>|<span data-ttu-id="78425-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="78425-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="78425-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="78425-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="78425-118">Дополнительные сведения см. в [сведениях о роли.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="78425-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="78425-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78425-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="78425-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78425-120">Request headers</span></span>
|<span data-ttu-id="78425-121">Имя</span><span class="sxs-lookup"><span data-stu-id="78425-121">Name</span></span>|<span data-ttu-id="78425-122">Описание</span><span class="sxs-lookup"><span data-stu-id="78425-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="78425-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78425-123">Authorization</span></span>|<span data-ttu-id="78425-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78425-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="78425-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78425-126">Content-Type</span></span>|<span data-ttu-id="78425-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78425-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="78425-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="78425-129">Request body</span></span>
<span data-ttu-id="78425-130">В теле запроса предоставляем представление объекта [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) в JSON со значениями полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="78425-130">In the request body, supply a JSON representation of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="78425-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="78425-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="78425-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="78425-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="78425-133">Список свойств см. в [microsoftAuthenticatorAuthenticationMethodConfiguration.](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="78425-133">For the list of properties, see [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="78425-134">**Примечание.** Свойство `@odata.type` со значением должно `#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration` быть включено в тело.</span><span class="sxs-lookup"><span data-stu-id="78425-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="78425-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="78425-135">Response</span></span>

<span data-ttu-id="78425-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="78425-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78425-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="78425-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="78425-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="78425-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
Content-Type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "state": "String"
}
```


### <a name="response"></a><span data-ttu-id="78425-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="78425-140">Response</span></span>
<span data-ttu-id="78425-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="78425-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "129ae788-e788-129a-88e7-9a1288e79a12",
  "state": "String"
}
```


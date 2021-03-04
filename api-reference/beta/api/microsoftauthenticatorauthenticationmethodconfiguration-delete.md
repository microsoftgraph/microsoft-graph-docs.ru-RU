---
title: Удаление MicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Удаляет объект MicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 132ad08227887d13bdf9b11b413dfb711acb9a2e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447850"
---
# <a name="delete-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="b080d-103">Удаление MicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="b080d-103">Delete microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="b080d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b080d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b080d-105">Удалите изменения, внесенные в политику проверки подлинности [Microsoft Authenticator,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) возвращая политику к ее конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b080d-105">Remove changes made to the [Microsoft Authenticator authentication method policy](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="b080d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b080d-106">Permissions</span></span>
<span data-ttu-id="b080d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b080d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b080d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b080d-109">Permission type</span></span>|<span data-ttu-id="b080d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b080d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b080d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b080d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b080d-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b080d-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="b080d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b080d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b080d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b080d-114">Not supported.</span></span>|
|<span data-ttu-id="b080d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b080d-115">Application</span></span>|<span data-ttu-id="b080d-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b080d-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="b080d-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="b080d-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="b080d-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="b080d-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="b080d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b080d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="b080d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b080d-120">Request headers</span></span>
|<span data-ttu-id="b080d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b080d-121">Name</span></span>|<span data-ttu-id="b080d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b080d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b080d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b080d-123">Authorization</span></span>|<span data-ttu-id="b080d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b080d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b080d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b080d-126">Request body</span></span>
<span data-ttu-id="b080d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b080d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b080d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b080d-128">Response</span></span>

<span data-ttu-id="b080d-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b080d-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b080d-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="b080d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b080d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b080d-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="b080d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b080d-132">Response</span></span>
<span data-ttu-id="b080d-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b080d-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


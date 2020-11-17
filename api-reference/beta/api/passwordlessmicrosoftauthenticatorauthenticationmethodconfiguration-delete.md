---
title: Удаление Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион
description: Удаление объекта Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eafbb6940a3d70e7191c18369e2764c137f0d674
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086653"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="4ac69-103">Удаление Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4ac69-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="4ac69-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ac69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ac69-105">Удаление изменений, внесенных в [политику метода проверки подлинности для входа на телефон средства проверки подлинности Майкрософт](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) , путем возврата политики к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ac69-105">Remove changes made to the [Microsoft Authenticator Phone Sign-in authentication method policy](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

> [!NOTE]
> <span data-ttu-id="4ac69-106">Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии.</span><span class="sxs-lookup"><span data-stu-id="4ac69-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="4ac69-107">Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.</span><span class="sxs-lookup"><span data-stu-id="4ac69-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ac69-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ac69-108">Permissions</span></span>
<span data-ttu-id="4ac69-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ac69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ac69-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ac69-111">Permission type</span></span>|<span data-ttu-id="4ac69-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ac69-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ac69-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ac69-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ac69-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4ac69-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="4ac69-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ac69-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ac69-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ac69-116">Not supported.</span></span>|
|<span data-ttu-id="4ac69-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ac69-117">Application</span></span>|<span data-ttu-id="4ac69-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ac69-118">Not supported.</span></span>|

<span data-ttu-id="4ac69-119">Для делегированных сценариев администратору требуется следующая [роль](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="4ac69-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="4ac69-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="4ac69-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="4ac69-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ac69-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="4ac69-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ac69-122">Request headers</span></span>
|<span data-ttu-id="4ac69-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4ac69-123">Name</span></span>|<span data-ttu-id="4ac69-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4ac69-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4ac69-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ac69-125">Authorization</span></span>|<span data-ttu-id="4ac69-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ac69-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ac69-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ac69-128">Request body</span></span>
<span data-ttu-id="4ac69-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ac69-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ac69-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ac69-130">Response</span></span>

<span data-ttu-id="4ac69-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4ac69-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4ac69-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="4ac69-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ac69-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ac69-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="4ac69-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ac69-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


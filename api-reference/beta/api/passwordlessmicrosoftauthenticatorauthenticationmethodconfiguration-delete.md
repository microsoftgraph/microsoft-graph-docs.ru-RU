---
title: Удаление Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион
description: Удаление объекта Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3200e95acdee4042c3933d5926662d6e49d52052
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418518"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="17290-103">Удаление Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="17290-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="17290-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17290-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17290-105">Удаление изменений, внесенных в [политику метода проверки подлинности для входа на телефон средства проверки подлинности Майкрософт](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) , путем возврата политики к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="17290-105">Remove changes made to the [Microsoft Authenticator Phone Sign-in authentication method policy](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

> [!NOTE]
> <span data-ttu-id="17290-106">Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии.</span><span class="sxs-lookup"><span data-stu-id="17290-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="17290-107">Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.</span><span class="sxs-lookup"><span data-stu-id="17290-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="17290-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17290-108">Permissions</span></span>
<span data-ttu-id="17290-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17290-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17290-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17290-111">Permission type</span></span>|<span data-ttu-id="17290-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17290-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17290-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17290-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17290-114">Policy. ReadWrite. AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="17290-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="17290-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17290-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17290-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17290-116">Not supported.</span></span>|
|<span data-ttu-id="17290-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17290-117">Application</span></span>|<span data-ttu-id="17290-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17290-118">Not supported.</span></span>|

<span data-ttu-id="17290-119">Для делегированных сценариев администратору требуется одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="17290-119">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="17290-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="17290-120">Global admin</span></span>
* <span data-ttu-id="17290-121">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="17290-121">Global reader</span></span>
* <span data-ttu-id="17290-122">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="17290-122">Privileged authentication admin</span></span>
* <span data-ttu-id="17290-123">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="17290-123">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="17290-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17290-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="17290-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17290-125">Request headers</span></span>
|<span data-ttu-id="17290-126">Имя</span><span class="sxs-lookup"><span data-stu-id="17290-126">Name</span></span>|<span data-ttu-id="17290-127">Описание</span><span class="sxs-lookup"><span data-stu-id="17290-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="17290-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17290-128">Authorization</span></span>|<span data-ttu-id="17290-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17290-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="17290-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="17290-131">Request body</span></span>
<span data-ttu-id="17290-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17290-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17290-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="17290-133">Response</span></span>

<span data-ttu-id="17290-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="17290-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="17290-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="17290-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="17290-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="17290-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="17290-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="17290-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


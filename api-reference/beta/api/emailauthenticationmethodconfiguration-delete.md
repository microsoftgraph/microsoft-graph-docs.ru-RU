---
title: Удаление emailAuthenticationMethodConfiguration
description: Удаляет объект emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 18ac6ff95148c0f31b9cd7c507038e7a4dd94f23
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436318"
---
# <a name="delete-emailauthenticationmethodconfiguration"></a><span data-ttu-id="aeb99-103">Удаление emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="aeb99-103">Delete emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="aeb99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aeb99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aeb99-105">Удалите изменения, внесенные в политику метода проверки [подлинности](../resources/emailauthenticationmethodconfiguration.md) электронной почты, возвращая политику к ее конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="aeb99-105">Remove changes made to the [email authentication method policy](../resources/emailauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="aeb99-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aeb99-106">Permissions</span></span>
<span data-ttu-id="aeb99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aeb99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aeb99-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aeb99-109">Permission type</span></span>|<span data-ttu-id="aeb99-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aeb99-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aeb99-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aeb99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aeb99-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="aeb99-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="aeb99-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aeb99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aeb99-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aeb99-114">Not supported.</span></span>|
|<span data-ttu-id="aeb99-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aeb99-115">Application</span></span>|<span data-ttu-id="aeb99-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aeb99-116">Not supported.</span></span>|

<span data-ttu-id="aeb99-117">Для делегирования сценариев администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="aeb99-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="aeb99-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="aeb99-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="aeb99-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aeb99-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="aeb99-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aeb99-120">Request headers</span></span>

|<span data-ttu-id="aeb99-121">Имя</span><span class="sxs-lookup"><span data-stu-id="aeb99-121">Name</span></span>|<span data-ttu-id="aeb99-122">Описание</span><span class="sxs-lookup"><span data-stu-id="aeb99-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="aeb99-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aeb99-123">Authorization</span></span>|<span data-ttu-id="aeb99-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aeb99-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aeb99-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aeb99-126">Request body</span></span>

<span data-ttu-id="aeb99-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aeb99-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aeb99-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="aeb99-128">Response</span></span>

<span data-ttu-id="aeb99-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aeb99-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="aeb99-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="aeb99-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aeb99-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="aeb99-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethodconfiguration"
}
-->

```http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

### <a name="response"></a><span data-ttu-id="aeb99-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="aeb99-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```


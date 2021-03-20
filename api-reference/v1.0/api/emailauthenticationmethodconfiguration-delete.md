---
title: Удаление emailAuthenticationMethodConfiguration
description: Удаляет объект emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8b25e0545eba722ab251a450600eb587d2ebad35
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964831"
---
# <a name="delete-emailauthenticationmethodconfiguration"></a><span data-ttu-id="af736-103">Удаление emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="af736-103">Delete emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="af736-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af736-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af736-105">Удалите изменения, внесенные в политику метода проверки [подлинности](../resources/emailauthenticationmethodconfiguration.md) электронной почты, возвращая политику к ее конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af736-105">Remove changes made to the [email authentication method policy](../resources/emailauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="af736-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af736-106">Permissions</span></span>
<span data-ttu-id="af736-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af736-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af736-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af736-109">Permission type</span></span>|<span data-ttu-id="af736-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af736-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af736-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af736-111">Delegated (work or school account)</span></span>|<span data-ttu-id="af736-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="af736-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="af736-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af736-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af736-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af736-114">Not supported.</span></span>|
|<span data-ttu-id="af736-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af736-115">Application</span></span>|<span data-ttu-id="af736-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="af736-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="af736-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="af736-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="af736-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="af736-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="af736-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af736-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="af736-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af736-120">Request headers</span></span>

|<span data-ttu-id="af736-121">Имя</span><span class="sxs-lookup"><span data-stu-id="af736-121">Name</span></span>|<span data-ttu-id="af736-122">Описание</span><span class="sxs-lookup"><span data-stu-id="af736-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="af736-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af736-123">Authorization</span></span>|<span data-ttu-id="af736-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af736-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af736-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af736-126">Request body</span></span>

<span data-ttu-id="af736-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af736-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af736-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="af736-128">Response</span></span>

<span data-ttu-id="af736-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="af736-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="af736-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="af736-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="af736-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="af736-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethodconfiguration"
}
-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

### <a name="response"></a><span data-ttu-id="af736-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="af736-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```


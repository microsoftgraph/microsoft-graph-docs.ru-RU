---
title: Удаление temporaryAccessPassAuthenticationMethodConfiguration
description: Удалите изменения, внесенные в временный объектAccessPassAuthenticationMethodConfiguration.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 37ea21542aa9ceace151428fcf951c0a87ecbf82
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272682"
---
# <a name="delete-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="711b4-103">Удаление temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="711b4-103">Delete temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="711b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="711b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="711b4-105">Удалите изменения объекта [temporaryAccessPassAuthenticationMethodConfiguration,](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) вернув политику к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="711b4-105">Remove changes made to the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="711b4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="711b4-106">Permissions</span></span>
<span data-ttu-id="711b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="711b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="711b4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="711b4-109">Permission type</span></span>|<span data-ttu-id="711b4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="711b4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="711b4-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="711b4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="711b4-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="711b4-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="711b4-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="711b4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="711b4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="711b4-114">Not supported.</span></span>|
|<span data-ttu-id="711b4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="711b4-115">Application</span></span>|<span data-ttu-id="711b4-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="711b4-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="711b4-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="711b4-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="711b4-118">Дополнительные сведения см. в [ролях.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="711b4-118">For more information, see [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="711b4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="711b4-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```


## <a name="request-headers"></a><span data-ttu-id="711b4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="711b4-120">Request headers</span></span>
|<span data-ttu-id="711b4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="711b4-121">Name</span></span>|<span data-ttu-id="711b4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="711b4-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="711b4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="711b4-123">Authorization</span></span>|<span data-ttu-id="711b4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="711b4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="711b4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="711b4-126">Request body</span></span>
<span data-ttu-id="711b4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="711b4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="711b4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="711b4-128">Response</span></span>

<span data-ttu-id="711b4-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="711b4-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="711b4-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="711b4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="711b4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="711b4-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```


### <a name="response"></a><span data-ttu-id="711b4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="711b4-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

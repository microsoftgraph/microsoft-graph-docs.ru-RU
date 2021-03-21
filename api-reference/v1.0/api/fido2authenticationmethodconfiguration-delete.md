---
title: Удаление fido2AuthenticationMethodConfiguration
description: Удаление объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1dbf6514a7dc21cb078f369d5e1e1db66f374661
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965001"
---
# <a name="delete-fido2authenticationmethodconfiguration"></a><span data-ttu-id="69109-103">Удаление fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="69109-103">Delete fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="69109-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69109-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69109-105">Удалите изменения, внесенные в политику метода проверки подлинности [FIDO2,](../resources/fido2authenticationmethodconfiguration.md) возвращая политику к ее конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="69109-105">Remove changes made to the [FIDO2 authentication method policy](../resources/fido2authenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="69109-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69109-106">Permissions</span></span>
<span data-ttu-id="69109-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69109-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="69109-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69109-109">Permission type</span></span>|<span data-ttu-id="69109-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69109-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69109-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69109-111">Delegated (work or school account)</span></span>|<span data-ttu-id="69109-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="69109-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="69109-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69109-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69109-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69109-114">Not supported.</span></span>|
|<span data-ttu-id="69109-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69109-115">Application</span></span>|<span data-ttu-id="69109-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="69109-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="69109-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="69109-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="69109-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="69109-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="69109-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69109-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="69109-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69109-120">Request headers</span></span>
|<span data-ttu-id="69109-121">Имя</span><span class="sxs-lookup"><span data-stu-id="69109-121">Name</span></span>|<span data-ttu-id="69109-122">Описание</span><span class="sxs-lookup"><span data-stu-id="69109-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="69109-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69109-123">Authorization</span></span>|<span data-ttu-id="69109-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69109-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69109-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69109-126">Request body</span></span>
<span data-ttu-id="69109-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69109-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69109-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="69109-128">Response</span></span>

<span data-ttu-id="69109-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="69109-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="69109-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="69109-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69109-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="69109-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="69109-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="69109-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


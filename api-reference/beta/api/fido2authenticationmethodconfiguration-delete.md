---
title: Удаление fido2AuthenticationMethodConfiguration
description: Удаление объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef92348219476f5a6ee344d5a25a5d1e7943e645
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086664"
---
# <a name="delete-fido2authenticationmethodconfiguration"></a><span data-ttu-id="62c25-103">Удаление fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="62c25-103">Delete fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="62c25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62c25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62c25-105">Удаление изменений, внесенных в [политику метода проверки подлинности FIDO2](../resources/fido2authenticationmethodconfiguration.md) , путем возврата политики к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="62c25-105">Remove changes made to the [FIDO2 authentication method policy](../resources/fido2authenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="62c25-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62c25-106">Permissions</span></span>
<span data-ttu-id="62c25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62c25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="62c25-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62c25-109">Permission type</span></span>|<span data-ttu-id="62c25-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62c25-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62c25-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62c25-111">Delegated (work or school account)</span></span>|<span data-ttu-id="62c25-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="62c25-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="62c25-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62c25-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62c25-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62c25-114">Not supported.</span></span>|
|<span data-ttu-id="62c25-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62c25-115">Application</span></span>|<span data-ttu-id="62c25-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62c25-116">Not supported.</span></span>|

<span data-ttu-id="62c25-117">Для делегированных сценариев администратору требуется следующая [роль](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="62c25-117">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="62c25-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="62c25-118">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="62c25-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62c25-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="62c25-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62c25-120">Request headers</span></span>
|<span data-ttu-id="62c25-121">Имя</span><span class="sxs-lookup"><span data-stu-id="62c25-121">Name</span></span>|<span data-ttu-id="62c25-122">Описание</span><span class="sxs-lookup"><span data-stu-id="62c25-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="62c25-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62c25-123">Authorization</span></span>|<span data-ttu-id="62c25-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62c25-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62c25-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62c25-126">Request body</span></span>
<span data-ttu-id="62c25-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62c25-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62c25-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="62c25-128">Response</span></span>

<span data-ttu-id="62c25-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="62c25-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="62c25-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="62c25-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62c25-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="62c25-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="62c25-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="62c25-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


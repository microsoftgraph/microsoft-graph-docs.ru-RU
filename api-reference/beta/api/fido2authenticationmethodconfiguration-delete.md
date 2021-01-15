---
title: Удаление fido2AuthenticationMethodConfiguration
description: Удаление объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 473c0605cc302b29730ddb359f51904050296ff2
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873005"
---
# <a name="delete-fido2authenticationmethodconfiguration"></a><span data-ttu-id="a39df-103">Удаление fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="a39df-103">Delete fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="a39df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a39df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a39df-105">Удалите изменения, внесенные в политику метода проверки подлинности [FIDO2,](../resources/fido2authenticationmethodconfiguration.md) вернув политику к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a39df-105">Remove changes made to the [FIDO2 authentication method policy](../resources/fido2authenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="a39df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a39df-106">Permissions</span></span>
<span data-ttu-id="a39df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a39df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a39df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a39df-109">Permission type</span></span>|<span data-ttu-id="a39df-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a39df-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a39df-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a39df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a39df-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a39df-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="a39df-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a39df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a39df-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a39df-114">Not supported.</span></span>|
|<span data-ttu-id="a39df-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a39df-115">Application</span></span>|<span data-ttu-id="a39df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a39df-116">Not supported.</span></span>|

<span data-ttu-id="a39df-117">Для делегирования сценариев администратору требуется следующая [роль:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="a39df-117">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="a39df-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a39df-118">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="a39df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a39df-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="a39df-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a39df-120">Request headers</span></span>
|<span data-ttu-id="a39df-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a39df-121">Name</span></span>|<span data-ttu-id="a39df-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a39df-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a39df-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a39df-123">Authorization</span></span>|<span data-ttu-id="a39df-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a39df-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a39df-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a39df-126">Request body</span></span>
<span data-ttu-id="a39df-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a39df-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a39df-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a39df-128">Response</span></span>

<span data-ttu-id="a39df-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a39df-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a39df-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a39df-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a39df-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a39df-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="a39df-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a39df-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


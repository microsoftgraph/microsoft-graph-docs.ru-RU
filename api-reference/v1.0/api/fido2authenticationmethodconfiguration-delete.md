---
title: Удаление fido2AuthenticationMethodConfiguration
description: Удаление объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8d13d64975c31458a1487d0efd060b8d1b0d57d2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202685"
---
# <a name="delete-fido2authenticationmethodconfiguration"></a><span data-ttu-id="e74fd-103">Удаление fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="e74fd-103">Delete fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="e74fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e74fd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e74fd-105">Удалите изменения, внесенные в политику метода проверки подлинности [FIDO2,](../resources/fido2authenticationmethodconfiguration.md) возвращая политику к ее конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e74fd-105">Remove changes made to the [FIDO2 authentication method policy](../resources/fido2authenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="e74fd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e74fd-106">Permissions</span></span>
<span data-ttu-id="e74fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e74fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e74fd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e74fd-109">Permission type</span></span>|<span data-ttu-id="e74fd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e74fd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e74fd-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e74fd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e74fd-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e74fd-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="e74fd-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e74fd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e74fd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e74fd-114">Not supported.</span></span>|
|<span data-ttu-id="e74fd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e74fd-115">Application</span></span>|<span data-ttu-id="e74fd-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e74fd-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="e74fd-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="e74fd-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="e74fd-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="e74fd-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="e74fd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e74fd-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="e74fd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e74fd-120">Request headers</span></span>
|<span data-ttu-id="e74fd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e74fd-121">Name</span></span>|<span data-ttu-id="e74fd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e74fd-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e74fd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e74fd-123">Authorization</span></span>|<span data-ttu-id="e74fd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e74fd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e74fd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e74fd-126">Request body</span></span>
<span data-ttu-id="e74fd-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e74fd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e74fd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e74fd-128">Response</span></span>

<span data-ttu-id="e74fd-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e74fd-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e74fd-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="e74fd-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e74fd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e74fd-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e74fd-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e74fd-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```
# <a name="c"></a>[<span data-ttu-id="e74fd-133">C#</span><span class="sxs-lookup"><span data-stu-id="e74fd-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e74fd-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e74fd-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e74fd-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e74fd-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e74fd-136">Java</span><span class="sxs-lookup"><span data-stu-id="e74fd-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e74fd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e74fd-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


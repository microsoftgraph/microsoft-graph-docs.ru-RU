---
title: Удаление fido2AuthenticationMethodConfiguration
description: Удаление объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2c68e931c3b7bfbb125f165bfbda01b3100027da
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471168"
---
# <a name="delete-fido2authenticationmethodconfiguration"></a><span data-ttu-id="81c7f-103">Удаление fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="81c7f-103">Delete fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="81c7f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81c7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81c7f-105">Удалите изменения, внесенные в политику метода проверки подлинности [FIDO2,](../resources/fido2authenticationmethodconfiguration.md) возвращая политику к ее конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="81c7f-105">Remove changes made to the [FIDO2 authentication method policy](../resources/fido2authenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="81c7f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81c7f-106">Permissions</span></span>
<span data-ttu-id="81c7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81c7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="81c7f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81c7f-109">Permission type</span></span>|<span data-ttu-id="81c7f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81c7f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81c7f-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81c7f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81c7f-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="81c7f-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="81c7f-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81c7f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81c7f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81c7f-114">Not supported.</span></span>|
|<span data-ttu-id="81c7f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81c7f-115">Application</span></span>|<span data-ttu-id="81c7f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81c7f-116">Not supported.</span></span>|

<span data-ttu-id="81c7f-117">Для делегирования сценариев администратору требуется следующая [роль:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="81c7f-117">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="81c7f-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="81c7f-118">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="81c7f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81c7f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="81c7f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81c7f-120">Request headers</span></span>
|<span data-ttu-id="81c7f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="81c7f-121">Name</span></span>|<span data-ttu-id="81c7f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="81c7f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="81c7f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81c7f-123">Authorization</span></span>|<span data-ttu-id="81c7f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81c7f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81c7f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81c7f-126">Request body</span></span>
<span data-ttu-id="81c7f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81c7f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81c7f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="81c7f-128">Response</span></span>

<span data-ttu-id="81c7f-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="81c7f-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="81c7f-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="81c7f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81c7f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="81c7f-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="81c7f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="81c7f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```
# <a name="c"></a>[<span data-ttu-id="81c7f-133">C#</span><span class="sxs-lookup"><span data-stu-id="81c7f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81c7f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81c7f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81c7f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81c7f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81c7f-136">Java</span><span class="sxs-lookup"><span data-stu-id="81c7f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="81c7f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="81c7f-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


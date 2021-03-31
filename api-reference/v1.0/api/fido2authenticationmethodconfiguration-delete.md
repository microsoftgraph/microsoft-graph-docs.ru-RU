---
title: Удаление fido2AuthenticationMethodConfiguration
description: Удаление объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9718be65a374e4bd6dc55121a63f1c4040744f8b
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469362"
---
# <a name="delete-fido2authenticationmethodconfiguration"></a><span data-ttu-id="0cbb5-103">Удаление fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="0cbb5-103">Delete fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="0cbb5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cbb5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0cbb5-105">Удалите изменения, внесенные в политику метода проверки подлинности [FIDO2,](../resources/fido2authenticationmethodconfiguration.md) возвращая политику к ее конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0cbb5-105">Remove changes made to the [FIDO2 authentication method policy](../resources/fido2authenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cbb5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0cbb5-106">Permissions</span></span>
<span data-ttu-id="0cbb5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cbb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0cbb5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cbb5-109">Permission type</span></span>|<span data-ttu-id="0cbb5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cbb5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cbb5-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cbb5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0cbb5-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0cbb5-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="0cbb5-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cbb5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cbb5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cbb5-114">Not supported.</span></span>|
|<span data-ttu-id="0cbb5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0cbb5-115">Application</span></span>|<span data-ttu-id="0cbb5-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0cbb5-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="0cbb5-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="0cbb5-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="0cbb5-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="0cbb5-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="0cbb5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cbb5-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="0cbb5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cbb5-120">Request headers</span></span>
|<span data-ttu-id="0cbb5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0cbb5-121">Name</span></span>|<span data-ttu-id="0cbb5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0cbb5-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0cbb5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0cbb5-123">Authorization</span></span>|<span data-ttu-id="0cbb5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cbb5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cbb5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cbb5-126">Request body</span></span>
<span data-ttu-id="0cbb5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0cbb5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cbb5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cbb5-128">Response</span></span>

<span data-ttu-id="0cbb5-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0cbb5-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0cbb5-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="0cbb5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0cbb5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cbb5-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0cbb5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cbb5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```
# <a name="c"></a>[<span data-ttu-id="0cbb5-133">C#</span><span class="sxs-lookup"><span data-stu-id="0cbb5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cbb5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cbb5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cbb5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cbb5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cbb5-136">Java</span><span class="sxs-lookup"><span data-stu-id="0cbb5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0cbb5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cbb5-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


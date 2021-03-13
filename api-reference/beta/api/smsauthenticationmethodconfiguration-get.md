---
title: Get smsAuthenticationMethodConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта smsAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cc09a85fefb46142c46d5383a0d7225636041b8b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761852"
---
# <a name="get-smsauthenticationmethodconfiguration"></a><span data-ttu-id="131ff-103">Get smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="131ff-103">Get smsAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="131ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="131ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="131ff-105">Ознакомьтесь с свойствами и отношениями объекта [smsAuthenticationMethodConfiguration,](../resources/smsauthenticationmethodconfiguration.md) представляюного политику метода проверки подлинности текстовых сообщений для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="131ff-105">Read the properties and relationships of a [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object, which represents the Text Message authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="131ff-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="131ff-106">Permissions</span></span>
<span data-ttu-id="131ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="131ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="131ff-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="131ff-109">Permission type</span></span>|<span data-ttu-id="131ff-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="131ff-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="131ff-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="131ff-111">Delegated (work or school account)</span></span>|<span data-ttu-id="131ff-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="131ff-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="131ff-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="131ff-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="131ff-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="131ff-114">Not supported.</span></span>|
|<span data-ttu-id="131ff-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="131ff-115">Application</span></span>|<span data-ttu-id="131ff-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="131ff-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="131ff-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="131ff-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="131ff-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="131ff-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="131ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="131ff-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```

## <a name="request-headers"></a><span data-ttu-id="131ff-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="131ff-120">Request headers</span></span>
|<span data-ttu-id="131ff-121">Имя</span><span class="sxs-lookup"><span data-stu-id="131ff-121">Name</span></span>|<span data-ttu-id="131ff-122">Описание</span><span class="sxs-lookup"><span data-stu-id="131ff-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="131ff-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="131ff-123">Authorization</span></span>|<span data-ttu-id="131ff-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="131ff-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="131ff-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="131ff-126">Request body</span></span>
<span data-ttu-id="131ff-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="131ff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="131ff-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="131ff-128">Response</span></span>

<span data-ttu-id="131ff-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="131ff-129">If successful, this method returns a `200 OK` response code and a [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="131ff-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="131ff-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="131ff-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="131ff-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="131ff-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="131ff-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_smsauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```
# <a name="c"></a>[<span data-ttu-id="131ff-133">C#</span><span class="sxs-lookup"><span data-stu-id="131ff-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-smsauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="131ff-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="131ff-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-smsauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="131ff-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="131ff-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-smsauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="131ff-136">Java</span><span class="sxs-lookup"><span data-stu-id="131ff-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-smsauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="131ff-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="131ff-137">Response</span></span>
<span data-ttu-id="131ff-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="131ff-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.smsAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
    "id": "713980c7-80c7-7139-c780-3971c7803971",
    "state": "String"
  }
}
```


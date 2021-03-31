---
title: Get fido2AuthenticationMethodConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7d67b65577546b187f616462e3faeefa7aedb7b4
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469019"
---
# <a name="get-fido2authenticationmethodconfiguration"></a><span data-ttu-id="a5d37-103">Get fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="a5d37-103">Get fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="a5d37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5d37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5d37-105">Извлечение свойств и связей объекта [fido2AuthenticationMethodConfiguration,](../resources/fido2authenticationmethodconfiguration.md) который представляет [](../resources/authenticationmethodspolicies-overview.md) политику метода проверки подлинности ключей безопасности FIDO2 для клиента Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a5d37-105">Retrieve the properties and relationships of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5d37-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5d37-106">Permissions</span></span>
<span data-ttu-id="a5d37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5d37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5d37-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5d37-109">Permission type</span></span>|<span data-ttu-id="a5d37-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5d37-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5d37-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5d37-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a5d37-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a5d37-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="a5d37-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5d37-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5d37-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5d37-114">Not supported.</span></span>|
|<span data-ttu-id="a5d37-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5d37-115">Application</span></span>|<span data-ttu-id="a5d37-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a5d37-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="a5d37-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="a5d37-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="a5d37-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="a5d37-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="a5d37-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5d37-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="a5d37-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5d37-120">Request headers</span></span>
|<span data-ttu-id="a5d37-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a5d37-121">Name</span></span>|<span data-ttu-id="a5d37-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a5d37-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a5d37-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5d37-123">Authorization</span></span>|<span data-ttu-id="a5d37-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5d37-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5d37-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5d37-126">Request body</span></span>
<span data-ttu-id="a5d37-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5d37-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5d37-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5d37-128">Response</span></span>

<span data-ttu-id="a5d37-129">В случае успеха этот метод возвращает код отклика и `200 OK` [объект fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a5d37-129">If successful, this method returns a `200 OK` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5d37-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a5d37-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5d37-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5d37-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a5d37-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5d37-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```
# <a name="c"></a>[<span data-ttu-id="a5d37-133">C#</span><span class="sxs-lookup"><span data-stu-id="a5d37-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5d37-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5d37-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5d37-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5d37-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5d37-136">Java</span><span class="sxs-lookup"><span data-stu-id="a5d37-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fido2authenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a5d37-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5d37-137">Response</span></span>
<span data-ttu-id="a5d37-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5d37-138">The following is an example of the response.</span></span>

<span data-ttu-id="a5d37-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a5d37-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "value":{
      "@odata.type":"#microsoft.graph.fido2AuthenticationMethodConfiguration",
      "id":"Fido2",
      "state":"enabled",
      "isSelfServiceRegistrationAllowed":true,
      "isAttestationEnforced":true,
      "keyRestrictions":{
         "isEnforced":false,
         "enforcementType":"block",
         "aaGuids":[
            
         ]
      },
      "includeTargets":[
         {
            "targetType":"group",
            "id":"all_users",
            "isRegistrationRequired":false,
            "useForSignIn":true
         }
      ]
   }
}
```


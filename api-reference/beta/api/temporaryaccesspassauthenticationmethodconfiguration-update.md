---
title: Обновление temporaryAccessPassAuthenticationMethodConfiguration
description: Обновление свойств объекта temporaryAccessPassAuthenticationMethodConfiguration.
author: inbarckms
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6cd30c6016739fcb40c3d6541b1fd1b03f72bee6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049641"
---
# <a name="update-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="1ef6f-103">Обновление temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ef6f-103">Update temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="1ef6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ef6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ef6f-105">Обновим свойства объекта [temporaryAccessPassAuthenticationMethodConfiguration,](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности временных пропусков доступа для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1ef6f-105">Update the properties of a [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object,  which represents the Temporary Access Pass authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ef6f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ef6f-106">Permissions</span></span>
<span data-ttu-id="1ef6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ef6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ef6f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ef6f-109">Permission type</span></span>|<span data-ttu-id="1ef6f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ef6f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ef6f-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ef6f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1ef6f-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1ef6f-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="1ef6f-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ef6f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ef6f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ef6f-114">Not supported.</span></span>|
|<span data-ttu-id="1ef6f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ef6f-115">Application</span></span>|<span data-ttu-id="1ef6f-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1ef6f-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="1ef6f-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="1ef6f-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="1ef6f-118">Дополнительные сведения см. в[дополнительных сведениях.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="1ef6f-118">For more information, see[roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="1ef6f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ef6f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```

## <a name="request-headers"></a><span data-ttu-id="1ef6f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ef6f-120">Request headers</span></span>
|<span data-ttu-id="1ef6f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1ef6f-121">Name</span></span>|<span data-ttu-id="1ef6f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1ef6f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1ef6f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ef6f-123">Authorization</span></span>|<span data-ttu-id="1ef6f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ef6f-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1ef6f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ef6f-126">Content-Type</span></span>|<span data-ttu-id="1ef6f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ef6f-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ef6f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ef6f-129">Request body</span></span>
<span data-ttu-id="1ef6f-130">В теле запроса поставляем представление JSON объекта [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) со значениями полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="1ef6f-130">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="1ef6f-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="1ef6f-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1ef6f-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1ef6f-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="1ef6f-133">Все свойства объекта могут быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="1ef6f-133">All properties of the object can be updated.</span></span> <span data-ttu-id="1ef6f-134">Список свойств см. в [пункте temporaryAccessPassAuthenticationMethodConfiguration.](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ef6f-134">For a list of properties, see [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="1ef6f-135">**Примечание:** Свойство `@odata.type` со значением `#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration` должно быть включено в тело.</span><span class="sxs-lookup"><span data-stu-id="1ef6f-135">**Note:** The `@odata.type` property with a value of `#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="1ef6f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ef6f-136">Response</span></span>

<span data-ttu-id="1ef6f-p107">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1ef6f-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ef6f-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="1ef6f-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1ef6f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ef6f-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1ef6f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ef6f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_temporaryaccesspassauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
Content-Type: application/json

{
  "@odata.type":"#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  "state":"enabled",
  "defaultLifetimeInMinutes":60,
  "defaultLength":8,
  "minimumLifetimeInMinutes":60,
  "maximumLifetimeInMinutes":1440,"
  isUsableOnce":false,
  "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false,
            "useForSignIn": true
        }
    ]
}


```
# <a name="javascript"></a>[<span data-ttu-id="1ef6f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ef6f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-temporaryaccesspassauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ef6f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ef6f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-temporaryaccesspassauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ef6f-144">Java</span><span class="sxs-lookup"><span data-stu-id="1ef6f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-temporaryaccesspassauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1ef6f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ef6f-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

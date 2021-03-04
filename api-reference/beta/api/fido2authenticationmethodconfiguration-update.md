---
title: Обновление fido2AuthenticationMethodConfiguration
description: Обновление свойств объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 93ea4ad235ba58df44c33be8c64beaa294557628
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436000"
---
# <a name="update-fido2authenticationmethodconfiguration"></a><span data-ttu-id="05f7b-103">Обновление fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="05f7b-103">Update fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="05f7b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05f7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05f7b-105">Обновим свойства объекта [fido2AuthenticationMethodConfiguration,](../resources/fido2authenticationmethodconfiguration.md) который представляет политику метода проверки подлинности ключей безопасности FIDO2 для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="05f7b-105">Update the properties of a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="05f7b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05f7b-106">Permissions</span></span>
<span data-ttu-id="05f7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05f7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05f7b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05f7b-109">Permission type</span></span>|<span data-ttu-id="05f7b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05f7b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05f7b-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05f7b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05f7b-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="05f7b-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="05f7b-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05f7b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05f7b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05f7b-114">Not supported.</span></span>|
|<span data-ttu-id="05f7b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05f7b-115">Application</span></span>|<span data-ttu-id="05f7b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05f7b-116">Not supported.</span></span>|

<span data-ttu-id="05f7b-117">Для делегирования сценариев администратору требуется следующая [роль:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="05f7b-117">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="05f7b-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="05f7b-118">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="05f7b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05f7b-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="05f7b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05f7b-120">Request headers</span></span>
|<span data-ttu-id="05f7b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="05f7b-121">Name</span></span>|<span data-ttu-id="05f7b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="05f7b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="05f7b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05f7b-123">Authorization</span></span>|<span data-ttu-id="05f7b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05f7b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="05f7b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05f7b-126">Content-Type</span></span>|<span data-ttu-id="05f7b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05f7b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="05f7b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05f7b-129">Request body</span></span>
<span data-ttu-id="05f7b-130">В корпусе запроса необходимо предоставить представление JSON объекта [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) со значениями полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="05f7b-130">In the request body, supply a JSON representation of a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="05f7b-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="05f7b-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="05f7b-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="05f7b-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="05f7b-133">Список свойств, которые можно обновить, см. [в списке fido2AuthenticationMethodConfiguration.](../resources/fido2authenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05f7b-133">For the list of properties that can be updated, see [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="05f7b-134">**Примечание:** Свойство `@odata.type` со значением `#microsoft.graph.fido2AuthenticationMethodConfiguration` должно быть включено в тело.</span><span class="sxs-lookup"><span data-stu-id="05f7b-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.fido2AuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="05f7b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="05f7b-135">Response</span></span>

<span data-ttu-id="05f7b-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05f7b-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05f7b-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="05f7b-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05f7b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="05f7b-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_fido2authenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
    "state": "enabled",
    "isAttestationEnforced": "true"
}
```


### <a name="response"></a><span data-ttu-id="05f7b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="05f7b-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


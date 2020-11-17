---
title: Обновление fido2AuthenticationMethodConfiguration
description: Обновление свойств объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc943876c99700cf77702bb76998308b6837c5c0
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086657"
---
# <a name="update-fido2authenticationmethodconfiguration"></a><span data-ttu-id="c3c3e-103">Обновление fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3c3e-103">Update fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="c3c3e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3c3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3c3e-105">Обновление свойств объекта [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) , который представляет политику метода проверки подлинности FIDO2 с ключами безопасности для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c3c3e-105">Update the properties of a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3c3e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3c3e-106">Permissions</span></span>
<span data-ttu-id="c3c3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3c3e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3c3e-109">Permission type</span></span>|<span data-ttu-id="c3c3e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3c3e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3c3e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3c3e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3c3e-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c3c3e-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="c3c3e-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3c3e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3c3e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3c3e-114">Not supported.</span></span>|
|<span data-ttu-id="c3c3e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3c3e-115">Application</span></span>|<span data-ttu-id="c3c3e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3c3e-116">Not supported.</span></span>|

<span data-ttu-id="c3c3e-117">Для делегированных сценариев администратору требуется следующая [роль](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="c3c3e-117">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="c3c3e-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="c3c3e-118">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="c3c3e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3c3e-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="c3c3e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3c3e-120">Request headers</span></span>
|<span data-ttu-id="c3c3e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c3c3e-121">Name</span></span>|<span data-ttu-id="c3c3e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c3c3e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c3c3e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3c3e-123">Authorization</span></span>|<span data-ttu-id="c3c3e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3c3e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c3c3e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3c3e-126">Content-Type</span></span>|<span data-ttu-id="c3c3e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3c3e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3c3e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3c3e-129">Request body</span></span>
<span data-ttu-id="c3c3e-130">В тексте запроса добавьте представление объекта [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) в формате JSON со значениями полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c3c3e-130">In the request body, supply a JSON representation of a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="c3c3e-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="c3c3e-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c3c3e-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c3c3e-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="c3c3e-133">Список свойств, которые можно обновлять, приведен в разделе [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3c3e-133">For the list of properties that can be updated, see [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="c3c3e-134">**Примечание:** `@odata.type` Свойство со значением `#microsoft.graph.fido2AuthenticationMethodConfiguration` должно быть включено в текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="c3c3e-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.fido2AuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="c3c3e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3c3e-135">Response</span></span>

<span data-ttu-id="c3c3e-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c3c3e-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3c3e-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="c3c3e-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3c3e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3c3e-139">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="c3c3e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3c3e-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


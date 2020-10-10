---
title: Обновление fido2AuthenticationMethodConfiguration
description: Обновление свойств объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4337d6d7207cdfd60c1dc16e39d7e0c5c2739cc8
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418434"
---
# <a name="update-fido2authenticationmethodconfiguration"></a><span data-ttu-id="4c467-103">Обновление fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c467-103">Update fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="4c467-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c467-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c467-105">Обновление свойств объекта [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) , который представляет политику метода проверки подлинности FIDO2 с ключами безопасности для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4c467-105">Update the properties of a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c467-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c467-106">Permissions</span></span>
<span data-ttu-id="4c467-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c467-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c467-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c467-109">Permission type</span></span>|<span data-ttu-id="4c467-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c467-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c467-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c467-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c467-112">Policy. ReadWrite. AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4c467-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="4c467-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c467-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c467-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c467-114">Not supported.</span></span>|
|<span data-ttu-id="4c467-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c467-115">Application</span></span>|<span data-ttu-id="4c467-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c467-116">Not supported.</span></span>|

<span data-ttu-id="4c467-117">Для делегированных сценариев администратору требуется одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="4c467-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="4c467-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="4c467-118">Global admin</span></span>
* <span data-ttu-id="4c467-119">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="4c467-119">Global reader</span></span>
* <span data-ttu-id="4c467-120">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="4c467-120">Privileged authentication admin</span></span>
* <span data-ttu-id="4c467-121">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="4c467-121">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="4c467-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c467-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="4c467-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c467-123">Request headers</span></span>
|<span data-ttu-id="4c467-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4c467-124">Name</span></span>|<span data-ttu-id="4c467-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4c467-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4c467-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c467-126">Authorization</span></span>|<span data-ttu-id="4c467-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c467-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4c467-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c467-129">Content-Type</span></span>|<span data-ttu-id="4c467-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c467-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c467-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c467-132">Request body</span></span>
<span data-ttu-id="4c467-133">В тексте запроса добавьте представление объекта [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) в формате JSON со значениями полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4c467-133">In the request body, supply a JSON representation of a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="4c467-134">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="4c467-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4c467-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4c467-135">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="4c467-136">Список свойств, которые можно обновлять, приведен в разделе [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c467-136">For the list of properties that can be updated, see [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="4c467-137">**Примечание:** `@odata.type` Свойство со значением `#microsoft.graph.fido2AuthenticationMethodConfiguration` должно быть включено в текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="4c467-137">**Note:** The `@odata.type` property with a value of `#microsoft.graph.fido2AuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="4c467-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c467-138">Response</span></span>

<span data-ttu-id="4c467-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4c467-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c467-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c467-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c467-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c467-142">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="4c467-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c467-143">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


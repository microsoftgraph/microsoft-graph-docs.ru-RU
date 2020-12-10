---
title: Обновление Емаилаусентикатионмесодконфигуратион
description: Обновление свойств объекта Емаилаусентикатионмесодконфигуратион.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b7fdd3566904c3ee8ad56210be03a8274cc858b
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617140"
---
# <a name="update-emailauthenticationmethodconfiguration"></a><span data-ttu-id="2d9ce-103">Обновление Емаилаусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2d9ce-103">Update emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="2d9ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d9ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d9ce-105">Обновление свойств объекта [емаилаусентикатионмесодконфигуратион](../resources/emailauthenticationmethodconfiguration.md) , представляющего [политику метода проверки подлинности](../resources/authenticationmethodspolicies-overview.md) OTP для клиента Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2d9ce-105">Update the properties of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d9ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d9ce-106">Permissions</span></span>
<span data-ttu-id="2d9ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d9ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d9ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d9ce-109">Permission type</span></span>|<span data-ttu-id="2d9ce-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d9ce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d9ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d9ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2d9ce-112">Policy. ReadWrite. AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2d9ce-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="2d9ce-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d9ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d9ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d9ce-114">Not supported.</span></span>|
|<span data-ttu-id="2d9ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d9ce-115">Application</span></span>|<span data-ttu-id="2d9ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d9ce-116">Not supported.</span></span>|

<span data-ttu-id="2d9ce-117">Для делегированных сценариев администратору требуется одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="2d9ce-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="2d9ce-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2d9ce-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="2d9ce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d9ce-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /policies/authenticationMethodsPolicy/email
```

## <a name="request-headers"></a><span data-ttu-id="2d9ce-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d9ce-120">Request headers</span></span>

|<span data-ttu-id="2d9ce-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2d9ce-121">Name</span></span>|<span data-ttu-id="2d9ce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2d9ce-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2d9ce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d9ce-123">Authorization</span></span>|<span data-ttu-id="2d9ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d9ce-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2d9ce-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d9ce-126">Content-Type</span></span>|<span data-ttu-id="2d9ce-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d9ce-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d9ce-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d9ce-129">Request body</span></span>

<span data-ttu-id="2d9ce-130">В тексте запроса добавьте представление объекта [емаилаусентикатионмесодконфигуратион](../resources/emailauthenticationmethodconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d9ce-130">In the request body, supply a JSON representation of the [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object.</span></span> <span data-ttu-id="2d9ce-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="2d9ce-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2d9ce-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2d9ce-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="2d9ce-133">Список свойств, которые можно обновлять, приведен в разделе [емаилаусентикатионмесодконфигуратион](../resources/emailauthenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d9ce-133">For the list of properties that can be updated, see [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="2d9ce-134">**Примечание:** `@odata.type` Свойство со значением `#microsoft.graph.emailAuthenticationMethodConfiguration` должно быть включено в текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="2d9ce-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.emailAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="2d9ce-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d9ce-135">Response</span></span>

<span data-ttu-id="2d9ce-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2d9ce-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d9ce-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="2d9ce-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d9ce-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d9ce-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethodconfiguration"
}
-->

```http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfiguration/email
Content-Type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "allowExternalIdToUseEmailOtp": "false",
}
```

### <a name="response"></a><span data-ttu-id="2d9ce-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d9ce-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 NO CONTENT
```


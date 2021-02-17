---
title: Обновление temporaryAccessPassAuthenticationMethodConfiguration
description: Обновление свойств объекта temporaryAccessPassAuthenticationMethodConfiguration.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 868234129fbcaa89d19ac2778c80e8aac6a93aed
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272674"
---
# <a name="update-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="791b5-103">Обновление temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="791b5-103">Update temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="791b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="791b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="791b5-105">Обновление свойств объекта [temporaryAccessPassAuthenticationMethodConfiguration,](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности для временного прохода доступа для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="791b5-105">Update the properties of a [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object,  which represents the Temporary Access Pass authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="791b5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="791b5-106">Permissions</span></span>
<span data-ttu-id="791b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="791b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="791b5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="791b5-109">Permission type</span></span>|<span data-ttu-id="791b5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="791b5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="791b5-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="791b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="791b5-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="791b5-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="791b5-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="791b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="791b5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="791b5-114">Not supported.</span></span>|
|<span data-ttu-id="791b5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="791b5-115">Application</span></span>|<span data-ttu-id="791b5-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="791b5-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="791b5-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="791b5-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="791b5-118">Дополнительные сведения см. в[ролях.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="791b5-118">For more information, see[roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="791b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="791b5-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```

## <a name="request-headers"></a><span data-ttu-id="791b5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="791b5-120">Request headers</span></span>
|<span data-ttu-id="791b5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="791b5-121">Name</span></span>|<span data-ttu-id="791b5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="791b5-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="791b5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="791b5-123">Authorization</span></span>|<span data-ttu-id="791b5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="791b5-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="791b5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="791b5-126">Content-Type</span></span>|<span data-ttu-id="791b5-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="791b5-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="791b5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="791b5-129">Request body</span></span>
<span data-ttu-id="791b5-130">В теле запроса предоставляем представление объекта [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) в JSON со значениями полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="791b5-130">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="791b5-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="791b5-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="791b5-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="791b5-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="791b5-133">Все свойства объекта можно обновить.</span><span class="sxs-lookup"><span data-stu-id="791b5-133">All properties of the object can be updated.</span></span> <span data-ttu-id="791b5-134">Список свойств см. в подстроке [temporaryAccessPassAuthenticationMethodConfiguration.](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="791b5-134">For a list of properties, see [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="791b5-135">**Примечание.** Свойство `@odata.type` со значением должно `#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration` быть включено в тело.</span><span class="sxs-lookup"><span data-stu-id="791b5-135">**Note:** The `@odata.type` property with a value of `#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="791b5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="791b5-136">Response</span></span>

<span data-ttu-id="791b5-p107">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="791b5-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="791b5-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="791b5-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="791b5-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="791b5-140">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="791b5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="791b5-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
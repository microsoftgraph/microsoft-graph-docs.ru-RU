---
title: Обновление smsAuthenticationMethodConfiguration
description: Обновление свойств объекта smsAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbdcddf77f2e85517b6c8d1685b4129b1e8d83f0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475631"
---
# <a name="update-smsauthenticationmethodconfiguration"></a><span data-ttu-id="8c79c-103">Обновление smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c79c-103">Update smsAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="8c79c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c79c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c79c-105">Обновим свойства объекта [smsAuthenticationMethodConfiguration,](../resources/smsauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности текстовых сообщений для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8c79c-105">Update the properties of a [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object, which represents the Text Message authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c79c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c79c-106">Permissions</span></span>
<span data-ttu-id="8c79c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c79c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c79c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c79c-109">Permission type</span></span>|<span data-ttu-id="8c79c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c79c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c79c-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c79c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c79c-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8c79c-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="8c79c-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c79c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c79c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c79c-114">Not supported.</span></span>|
|<span data-ttu-id="8c79c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c79c-115">Application</span></span>|<span data-ttu-id="8c79c-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8c79c-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="8c79c-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="8c79c-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="8c79c-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="8c79c-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="8c79c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c79c-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```

## <a name="request-headers"></a><span data-ttu-id="8c79c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c79c-120">Request headers</span></span>
|<span data-ttu-id="8c79c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8c79c-121">Name</span></span>|<span data-ttu-id="8c79c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8c79c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8c79c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c79c-123">Authorization</span></span>|<span data-ttu-id="8c79c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c79c-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8c79c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c79c-126">Content-Type</span></span>|<span data-ttu-id="8c79c-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c79c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c79c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c79c-129">Request body</span></span>
<span data-ttu-id="8c79c-130">В тексте запроса необходимо предоставить представление JSON объекта [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) со значениями полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8c79c-130">In the request body, supply a JSON representation of the [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="8c79c-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="8c79c-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8c79c-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8c79c-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="8c79c-133">В следующей таблице показаны свойства, необходимые при обновлении [объекта smsAuthenticationMethodConfiguration.](../resources/smsauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c79c-133">The following table shows the properties that are required when you update the [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object.</span></span>

|<span data-ttu-id="8c79c-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c79c-134">Property</span></span>|<span data-ttu-id="8c79c-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8c79c-135">Type</span></span>|<span data-ttu-id="8c79c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8c79c-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c79c-137">id</span><span class="sxs-lookup"><span data-stu-id="8c79c-137">id</span></span>|<span data-ttu-id="8c79c-138">String</span><span class="sxs-lookup"><span data-stu-id="8c79c-138">String</span></span>|<span data-ttu-id="8c79c-139">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8c79c-139">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="8c79c-140">state</span><span class="sxs-lookup"><span data-stu-id="8c79c-140">state</span></span>|<span data-ttu-id="8c79c-141">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="8c79c-141">authenticationMethodState</span></span>|<span data-ttu-id="8c79c-142">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8c79c-142">Possible values are: `enabled`, `disabled`.</span></span>|

><span data-ttu-id="8c79c-143">**Примечание:** Свойство `@odata.type` со значением `#microsoft.graph.smsAuthenticationMethodConfiguration` должно быть включено в тело.</span><span class="sxs-lookup"><span data-stu-id="8c79c-143">**Note:** The `@odata.type` property with a value of `#microsoft.graph.smsAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="8c79c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c79c-144">Response</span></span>

<span data-ttu-id="8c79c-145">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8c79c-145">If successful, this method returns a `200 OK` response code and an updated [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c79c-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c79c-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c79c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c79c-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8c79c-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c79c-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_smsauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
Content-Type: application/json
Content-length: 100

{
    "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
    "id": "Sms",
    "state": "enabled"
}
```
# <a name="c"></a>[<span data-ttu-id="8c79c-149">C#</span><span class="sxs-lookup"><span data-stu-id="8c79c-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-smsauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c79c-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c79c-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-smsauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c79c-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c79c-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-smsauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c79c-152">Java</span><span class="sxs-lookup"><span data-stu-id="8c79c-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-smsauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8c79c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c79c-153">Response</span></span>
<span data-ttu-id="8c79c-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c79c-154">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
  "id": "713980c7-80c7-7139-c780-3971c7803971",
  "state": "String"
}
```


---
title: 'authenticationMethodsRoot: usersRegisteredByFeature'
description: Получите количество пользователей, способных выполнять многофакторную проверку подлинности, самостоятельный сброс паролей и проверку подлинности без пароля.
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: c6f0976e364e2cf4b24883bef10e7f3c6e49480f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129672"
---
# <a name="authenticationmethodsroot-usersregisteredbyfeature"></a><span data-ttu-id="c7da0-103">authenticationMethodsRoot: usersRegisteredByFeature</span><span class="sxs-lookup"><span data-stu-id="c7da0-103">authenticationMethodsRoot: usersRegisteredByFeature</span></span>
<span data-ttu-id="c7da0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7da0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7da0-105">Получите количество пользователей, способных выполнять многофакторную проверку подлинности, самостоятельный сброс паролей и проверку подлинности без пароля.</span><span class="sxs-lookup"><span data-stu-id="c7da0-105">Get the number of users capable of multi-factor authentication, self-service password reset, and passwordless authentication.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7da0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7da0-106">Permissions</span></span>
<span data-ttu-id="c7da0-107">Для вызова этого API требуются разрешения ниже.</span><span class="sxs-lookup"><span data-stu-id="c7da0-107">The following permissions are required to call this API.</span></span> <span data-ttu-id="c7da0-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7da0-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7da0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7da0-109">Permission type</span></span>|<span data-ttu-id="c7da0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7da0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7da0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7da0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7da0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7da0-112">Reports.Read.All</span></span>|
|<span data-ttu-id="c7da0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7da0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7da0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7da0-114">Not supported.</span></span>|
|<span data-ttu-id="c7da0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7da0-115">Application</span></span>|<span data-ttu-id="c7da0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7da0-116">Not supported.</span></span>|

<span data-ttu-id="c7da0-117">Для доступа к API требуется одна [из](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="c7da0-117">In order to access the API, [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) is required:</span></span>

* <span data-ttu-id="c7da0-118">Читатель отчетов</span><span class="sxs-lookup"><span data-stu-id="c7da0-118">Reports reader</span></span>
* <span data-ttu-id="c7da0-119">Читатель сведений о безопасности</span><span class="sxs-lookup"><span data-stu-id="c7da0-119">Security reader</span></span>
* <span data-ttu-id="c7da0-120">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="c7da0-120">Security admin</span></span>
* <span data-ttu-id="c7da0-121">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="c7da0-121">Global reader</span></span>
* <span data-ttu-id="c7da0-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="c7da0-122">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="c7da0-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7da0-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/usersRegisteredByFeature
```

## <a name="function-parameters"></a><span data-ttu-id="c7da0-124">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c7da0-124">Function parameters</span></span>
<span data-ttu-id="c7da0-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="c7da0-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c7da0-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="c7da0-126">Parameter</span></span>|<span data-ttu-id="c7da0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c7da0-127">Type</span></span>|<span data-ttu-id="c7da0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c7da0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7da0-129">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="c7da0-129">includedUserTypes</span></span>|<span data-ttu-id="c7da0-130">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="c7da0-130">includedUserTypes</span></span>|<span data-ttu-id="c7da0-131">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7da0-131">User type.</span></span> <span data-ttu-id="c7da0-132">Возможные значения: `all`, `member`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="c7da0-132">Possible values are: `all`, `member`, `guest`.</span></span>|
|<span data-ttu-id="c7da0-133">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="c7da0-133">includedUserRoles</span></span>|<span data-ttu-id="c7da0-134">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="c7da0-134">includedUserRoles</span></span>|<span data-ttu-id="c7da0-135">Тип роли пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7da0-135">User role type.</span></span> <span data-ttu-id="c7da0-136">Возможные значения: `all`, `privilegedAdmin`, `admin`, `user`.</span><span class="sxs-lookup"><span data-stu-id="c7da0-136">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|

<span data-ttu-id="c7da0-137">Значение состоит `privilegedAdmin` из следующих привилегированных ролей администратора:</span><span class="sxs-lookup"><span data-stu-id="c7da0-137">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="c7da0-138">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="c7da0-138">Global admin</span></span>
* <span data-ttu-id="c7da0-139">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="c7da0-139">Security admin</span></span>
* <span data-ttu-id="c7da0-140">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="c7da0-140">Conditional Access admin</span></span>
* <span data-ttu-id="c7da0-141">Администратор Exchange</span><span class="sxs-lookup"><span data-stu-id="c7da0-141">Exchange admin</span></span>
* <span data-ttu-id="c7da0-142">Администратор SharePoint</span><span class="sxs-lookup"><span data-stu-id="c7da0-142">SharePoint admin</span></span>
* <span data-ttu-id="c7da0-143">Администратор службы поддержки</span><span class="sxs-lookup"><span data-stu-id="c7da0-143">Helpdesk admin</span></span>
* <span data-ttu-id="c7da0-144">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="c7da0-144">Billing admin</span></span>
* <span data-ttu-id="c7da0-145">Администратор пользователей</span><span class="sxs-lookup"><span data-stu-id="c7da0-145">User admin</span></span>
* <span data-ttu-id="c7da0-146">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="c7da0-146">Authentication admin</span></span>

<span data-ttu-id="c7da0-147">Это значение `admin` включает все роли администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c7da0-147">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="c7da0-148">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7da0-148">Request headers</span></span>
|<span data-ttu-id="c7da0-149">Имя</span><span class="sxs-lookup"><span data-stu-id="c7da0-149">Name</span></span>|<span data-ttu-id="c7da0-150">Описание</span><span class="sxs-lookup"><span data-stu-id="c7da0-150">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c7da0-151">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7da0-151">Authorization</span></span>|<span data-ttu-id="c7da0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7da0-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7da0-154">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7da0-154">Request body</span></span>
<span data-ttu-id="c7da0-155">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7da0-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7da0-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7da0-156">Response</span></span>

<span data-ttu-id="c7da0-157">В случае успеха эта функция возвращает код отклика и `200 OK` [userRegistrationFeatureSummary](../resources/userregistrationfeaturesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7da0-157">If successful, this function returns a `200 OK` response code and a [userRegistrationFeatureSummary](../resources/userregistrationfeaturesummary.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7da0-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="c7da0-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7da0-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7da0-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c7da0-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7da0-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "authenticationmethodsroot_usersregisteredbyfeature"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')
```
# <a name="c"></a>[<span data-ttu-id="c7da0-161">C#</span><span class="sxs-lookup"><span data-stu-id="c7da0-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/authenticationmethodsroot-usersregisteredbyfeature-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7da0-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7da0-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/authenticationmethodsroot-usersregisteredbyfeature-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7da0-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7da0-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/authenticationmethodsroot-usersregisteredbyfeature-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7da0-164">Java</span><span class="sxs-lookup"><span data-stu-id="c7da0-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/authenticationmethodsroot-usersregisteredbyfeature-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c7da0-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7da0-165">Response</span></span>
<span data-ttu-id="c7da0-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c7da0-166">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.userRegistrationFeatureSummary",
    "totalUserCount": 23123,
    "userTypes": "all",
    "userRoles": "all",
    "userRegistrationFeatureCounts": [{
            "feature": "ssprRegistered",
            "userCount": 23423
        },
        {
            "feature": "ssprEnabled",
            "userCount": 4234
        },
        {
            "feature": "ssprCapable",
            "userCount": 4234
        }, {
            "feature": "passwordlessRegistered",
            "userCount": 323
        },
        {
            "feature": "mfaCapable",
            "userCount": 3345
        }
    ]
}
```

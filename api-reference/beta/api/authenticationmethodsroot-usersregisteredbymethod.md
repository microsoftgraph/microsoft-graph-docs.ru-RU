---
title: 'authenticationMethodsRoot: usersRegisteredByMethod'
description: Получите количество пользователей, зарегистрированных для каждого метода проверки подлинности.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 36b4d9ae280d34ab74a6c974710e3726ae089a1b
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092385"
---
# <a name="authenticationmethodsroot-usersregisteredbymethod"></a><span data-ttu-id="36e5e-103">authenticationMethodsRoot: usersRegisteredByMethod</span><span class="sxs-lookup"><span data-stu-id="36e5e-103">authenticationMethodsRoot: usersRegisteredByMethod</span></span>
<span data-ttu-id="36e5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36e5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36e5e-105">Получите количество пользователей, зарегистрированных для каждого метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="36e5e-105">Get the number of users registered for each authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="36e5e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36e5e-106">Permissions</span></span>
<span data-ttu-id="36e5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36e5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36e5e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36e5e-109">Permission type</span></span>|<span data-ttu-id="36e5e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36e5e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36e5e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36e5e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36e5e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="36e5e-112">Reports.Read.All</span></span>|
|<span data-ttu-id="36e5e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36e5e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36e5e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36e5e-114">Not supported.</span></span>|
|<span data-ttu-id="36e5e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36e5e-115">Application</span></span>|<span data-ttu-id="36e5e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36e5e-116">Not supported.</span></span>|

<span data-ttu-id="36e5e-117">Для доступа к API требуется одна [из](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="36e5e-117">In order to access the API, [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) is required:</span></span>

* <span data-ttu-id="36e5e-118">Читатель отчетов</span><span class="sxs-lookup"><span data-stu-id="36e5e-118">Reports reader</span></span>
* <span data-ttu-id="36e5e-119">Читатель сведений о безопасности</span><span class="sxs-lookup"><span data-stu-id="36e5e-119">Security reader</span></span>
* <span data-ttu-id="36e5e-120">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="36e5e-120">Security admin</span></span>
* <span data-ttu-id="36e5e-121">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="36e5e-121">Global reader</span></span>
* <span data-ttu-id="36e5e-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="36e5e-122">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="36e5e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36e5e-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/usersRegisteredByMethod
```

## <a name="function-parameters"></a><span data-ttu-id="36e5e-124">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="36e5e-124">Function parameters</span></span>
<span data-ttu-id="36e5e-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="36e5e-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="36e5e-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="36e5e-126">Parameter</span></span>|<span data-ttu-id="36e5e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="36e5e-127">Type</span></span>|<span data-ttu-id="36e5e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="36e5e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36e5e-129">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="36e5e-129">includedUserTypes</span></span>|<span data-ttu-id="36e5e-130">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="36e5e-130">includedUserTypes</span></span>|<span data-ttu-id="36e5e-131">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="36e5e-131">User type.</span></span> <span data-ttu-id="36e5e-132">Возможные значения: `all`, `member`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="36e5e-132">Possible values are: `all`, `member`, `guest`.</span></span>|
|<span data-ttu-id="36e5e-133">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="36e5e-133">includedUserRoles</span></span>|<span data-ttu-id="36e5e-134">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="36e5e-134">includedUserRoles</span></span>|<span data-ttu-id="36e5e-135">Тип роли пользователя.</span><span class="sxs-lookup"><span data-stu-id="36e5e-135">User role type.</span></span> <span data-ttu-id="36e5e-136">Возможные значения: `all`, `privilegedAdmin`, `admin`, `user`.</span><span class="sxs-lookup"><span data-stu-id="36e5e-136">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|

<span data-ttu-id="36e5e-137">Значение состоит `privilegedAdmin` из следующих привилегированных ролей администратора:</span><span class="sxs-lookup"><span data-stu-id="36e5e-137">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="36e5e-138">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="36e5e-138">Global admin</span></span>
* <span data-ttu-id="36e5e-139">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="36e5e-139">Security admin</span></span>
* <span data-ttu-id="36e5e-140">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="36e5e-140">Conditional Access admin</span></span>
* <span data-ttu-id="36e5e-141">Администратор Exchange</span><span class="sxs-lookup"><span data-stu-id="36e5e-141">Exchange admin</span></span>
* <span data-ttu-id="36e5e-142">Администратор SharePoint</span><span class="sxs-lookup"><span data-stu-id="36e5e-142">SharePoint admin</span></span>
* <span data-ttu-id="36e5e-143">Администратор службы поддержки</span><span class="sxs-lookup"><span data-stu-id="36e5e-143">Helpdesk admin</span></span>
* <span data-ttu-id="36e5e-144">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="36e5e-144">Billing admin</span></span>
* <span data-ttu-id="36e5e-145">Администратор пользователей</span><span class="sxs-lookup"><span data-stu-id="36e5e-145">User admin</span></span>
* <span data-ttu-id="36e5e-146">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="36e5e-146">Authentication admin</span></span>

<span data-ttu-id="36e5e-147">Это значение `admin` включает все роли администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="36e5e-147">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="36e5e-148">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36e5e-148">Request headers</span></span>
|<span data-ttu-id="36e5e-149">Имя</span><span class="sxs-lookup"><span data-stu-id="36e5e-149">Name</span></span>|<span data-ttu-id="36e5e-150">Описание</span><span class="sxs-lookup"><span data-stu-id="36e5e-150">Description</span></span>|
|:---|:---|
|<span data-ttu-id="36e5e-151">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36e5e-151">Authorization</span></span>|<span data-ttu-id="36e5e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36e5e-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36e5e-154">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36e5e-154">Request body</span></span>
<span data-ttu-id="36e5e-155">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36e5e-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36e5e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="36e5e-156">Response</span></span>

<span data-ttu-id="36e5e-157">В случае успеха эта функция возвращает код отклика и `200 OK` [userRegistrationMethodSummary](../resources/userregistrationmethodsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36e5e-157">If successful, this function returns a `200 OK` response code and a [userRegistrationMethodSummary](../resources/userregistrationmethodsummary.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36e5e-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="36e5e-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36e5e-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="36e5e-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="36e5e-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="36e5e-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "authenticationmethodsroot_usersregisteredbymethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')
```
# <a name="c"></a>[<span data-ttu-id="36e5e-161">C#</span><span class="sxs-lookup"><span data-stu-id="36e5e-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/authenticationmethodsroot-usersregisteredbymethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36e5e-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36e5e-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/authenticationmethodsroot-usersregisteredbymethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36e5e-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36e5e-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/authenticationmethodsroot-usersregisteredbymethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36e5e-164">Java</span><span class="sxs-lookup"><span data-stu-id="36e5e-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/authenticationmethodsroot-usersregisteredbymethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="36e5e-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="36e5e-165">Response</span></span>
<span data-ttu-id="36e5e-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="36e5e-166">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.userRegistrationMethodSummary",
    "userTypes": "all",
    "userRoles": "all",
    "userRegistrationMethodCounts": [{
            "authenticationMethod": "password",
            "userCount": 12209
        },
        {
            "authenticationMethod": "windowsHelloForBusiness",
            "userCount": 223
        },
        {
            "authenticationMethod": "mobilePhone",
            "userCount": 4234
        }
    ]
}
```

---
title: 'authenticationMethodsRoot: usersRegisteredByMethod'
description: Получите количество пользователей, зарегистрированных для каждого метода проверки подлинности.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 684603da36a4d5dcf08fc575042b49055e581e7b
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052581"
---
# <a name="authenticationmethodsroot-usersregisteredbymethod"></a><span data-ttu-id="6d30b-103">authenticationMethodsRoot: usersRegisteredByMethod</span><span class="sxs-lookup"><span data-stu-id="6d30b-103">authenticationMethodsRoot: usersRegisteredByMethod</span></span>
<span data-ttu-id="6d30b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d30b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d30b-105">Получите количество пользователей, зарегистрированных для каждого метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6d30b-105">Get the number of users registered for each authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d30b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d30b-106">Permissions</span></span>
<span data-ttu-id="6d30b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d30b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d30b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d30b-109">Permission type</span></span>|<span data-ttu-id="6d30b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d30b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d30b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d30b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d30b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d30b-112">Reports.Read.All</span></span>|
|<span data-ttu-id="6d30b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d30b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d30b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d30b-114">Not supported.</span></span>|
|<span data-ttu-id="6d30b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d30b-115">Application</span></span>|<span data-ttu-id="6d30b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d30b-116">Not supported.</span></span>|

<span data-ttu-id="6d30b-117">Для доступа к API требуется одна [из](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="6d30b-117">In order to access the API, [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) is required:</span></span>

* <span data-ttu-id="6d30b-118">Читатель отчетов</span><span class="sxs-lookup"><span data-stu-id="6d30b-118">Reports reader</span></span>
* <span data-ttu-id="6d30b-119">Читатель сведений о безопасности</span><span class="sxs-lookup"><span data-stu-id="6d30b-119">Security reader</span></span>
* <span data-ttu-id="6d30b-120">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="6d30b-120">Security admin</span></span>
* <span data-ttu-id="6d30b-121">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="6d30b-121">Global reader</span></span>
* <span data-ttu-id="6d30b-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6d30b-122">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="6d30b-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d30b-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/usersRegisteredByMethod
```

## <a name="function-parameters"></a><span data-ttu-id="6d30b-124">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6d30b-124">Function parameters</span></span>
<span data-ttu-id="6d30b-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="6d30b-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6d30b-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="6d30b-126">Parameter</span></span>|<span data-ttu-id="6d30b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6d30b-127">Type</span></span>|<span data-ttu-id="6d30b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6d30b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d30b-129">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="6d30b-129">includedUserTypes</span></span>|<span data-ttu-id="6d30b-130">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="6d30b-130">includedUserTypes</span></span>|<span data-ttu-id="6d30b-131">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="6d30b-131">User type.</span></span> <span data-ttu-id="6d30b-132">Возможные значения: `all`, `member`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="6d30b-132">Possible values are: `all`, `member`, `guest`.</span></span>|
|<span data-ttu-id="6d30b-133">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="6d30b-133">includedUserRoles</span></span>|<span data-ttu-id="6d30b-134">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="6d30b-134">includedUserRoles</span></span>|<span data-ttu-id="6d30b-135">Тип роли пользователя.</span><span class="sxs-lookup"><span data-stu-id="6d30b-135">User role type.</span></span> <span data-ttu-id="6d30b-136">Возможные значения: `all`, `privilegedAdmin`, `admin`, `user`.</span><span class="sxs-lookup"><span data-stu-id="6d30b-136">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|

<span data-ttu-id="6d30b-137">Значение состоит `privilegedAdmin` из следующих привилегированных ролей администратора:</span><span class="sxs-lookup"><span data-stu-id="6d30b-137">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="6d30b-138">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6d30b-138">Global admin</span></span>
* <span data-ttu-id="6d30b-139">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="6d30b-139">Security admin</span></span>
* <span data-ttu-id="6d30b-140">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="6d30b-140">Conditional Access admin</span></span>
* <span data-ttu-id="6d30b-141">Администратор Exchange</span><span class="sxs-lookup"><span data-stu-id="6d30b-141">Exchange admin</span></span>
* <span data-ttu-id="6d30b-142">Администратор SharePoint</span><span class="sxs-lookup"><span data-stu-id="6d30b-142">SharePoint admin</span></span>
* <span data-ttu-id="6d30b-143">Администратор службы поддержки</span><span class="sxs-lookup"><span data-stu-id="6d30b-143">Helpdesk admin</span></span>
* <span data-ttu-id="6d30b-144">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="6d30b-144">Billing admin</span></span>
* <span data-ttu-id="6d30b-145">Администратор пользователей</span><span class="sxs-lookup"><span data-stu-id="6d30b-145">User admin</span></span>
* <span data-ttu-id="6d30b-146">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="6d30b-146">Authentication admin</span></span>

<span data-ttu-id="6d30b-147">Значение включает `admin` все роли администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6d30b-147">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="6d30b-148">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d30b-148">Request headers</span></span>
|<span data-ttu-id="6d30b-149">Имя</span><span class="sxs-lookup"><span data-stu-id="6d30b-149">Name</span></span>|<span data-ttu-id="6d30b-150">Описание</span><span class="sxs-lookup"><span data-stu-id="6d30b-150">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6d30b-151">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d30b-151">Authorization</span></span>|<span data-ttu-id="6d30b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d30b-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d30b-154">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d30b-154">Request body</span></span>
<span data-ttu-id="6d30b-155">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d30b-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d30b-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d30b-156">Response</span></span>

<span data-ttu-id="6d30b-157">В случае успеха эта функция возвращает код отклика и `200 OK` [userRegistrationMethodSummary](../resources/userregistrationmethodsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d30b-157">If successful, this function returns a `200 OK` response code and a [userRegistrationMethodSummary](../resources/userregistrationmethodsummary.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d30b-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="6d30b-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d30b-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d30b-159">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "authenticationmethodsroot_usersregisteredbymethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')
```


### <a name="response"></a><span data-ttu-id="6d30b-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d30b-160">Response</span></span>
<span data-ttu-id="6d30b-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6d30b-161">**Note:** The response object shown here might be shortened for readability.</span></span>
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

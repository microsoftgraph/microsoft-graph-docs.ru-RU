---
title: Get windowsHelloForBusinessAuthenticationMethod
description: Чтение свойств и связей объекта windowsHelloForBusinessAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e9fdb6b8b48a12f1f618479b2e939944e25288fe
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873313"
---
# <a name="get-windowshelloforbusinessauthenticationmethod"></a><span data-ttu-id="72ddd-103">Get windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="72ddd-103">Get windowsHelloForBusinessAuthenticationMethod</span></span>
<span data-ttu-id="72ddd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72ddd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72ddd-105">Чтение свойств и связей объекта [windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="72ddd-105">Read the properties and relationships of a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72ddd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72ddd-106">Permissions</span></span>

<span data-ttu-id="72ddd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72ddd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="72ddd-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="72ddd-109">Permissions acting on self</span></span>

|<span data-ttu-id="72ddd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72ddd-110">Permission type</span></span>      | <span data-ttu-id="72ddd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72ddd-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="72ddd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72ddd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="72ddd-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72ddd-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="72ddd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72ddd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72ddd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72ddd-115">Not supported.</span></span> |
| <span data-ttu-id="72ddd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72ddd-116">Application</span></span>                            | <span data-ttu-id="72ddd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72ddd-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="72ddd-118">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="72ddd-118">Permissions acting on other users</span></span>

|<span data-ttu-id="72ddd-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72ddd-119">Permission type</span></span>      | <span data-ttu-id="72ddd-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72ddd-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="72ddd-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72ddd-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="72ddd-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72ddd-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="72ddd-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72ddd-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72ddd-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72ddd-124">Not supported.</span></span> |
| <span data-ttu-id="72ddd-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="72ddd-125">Application</span></span>                            | <span data-ttu-id="72ddd-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72ddd-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="72ddd-127">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="72ddd-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="72ddd-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="72ddd-128">Global admin</span></span>
* <span data-ttu-id="72ddd-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="72ddd-129">Global reader</span></span>
* <span data-ttu-id="72ddd-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="72ddd-130">Privileged authentication admin</span></span>
* <span data-ttu-id="72ddd-131">Администратор проверки подлинности (видит только маскирование номеров телефонов)</span><span class="sxs-lookup"><span data-stu-id="72ddd-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="72ddd-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72ddd-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72ddd-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72ddd-133">Optional query parameters</span></span>

<span data-ttu-id="72ddd-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72ddd-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72ddd-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72ddd-135">Request headers</span></span>
|<span data-ttu-id="72ddd-136">Имя</span><span class="sxs-lookup"><span data-stu-id="72ddd-136">Name</span></span>|<span data-ttu-id="72ddd-137">Описание</span><span class="sxs-lookup"><span data-stu-id="72ddd-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="72ddd-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72ddd-138">Authorization</span></span>|<span data-ttu-id="72ddd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72ddd-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72ddd-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72ddd-141">Request body</span></span>
<span data-ttu-id="72ddd-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72ddd-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72ddd-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="72ddd-143">Response</span></span>

<span data-ttu-id="72ddd-144">В случае успеха этот метод возвращает код отклика и объект `200 OK` [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72ddd-144">If successful, this method returns a `200 OK` response code and a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72ddd-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="72ddd-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72ddd-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="72ddd-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2
```

### <a name="response"></a><span data-ttu-id="72ddd-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="72ddd-147">Response</span></span>
<span data-ttu-id="72ddd-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="72ddd-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsHelloForBusinessAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
    "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
    "displayName": "Jordan's Surface Book",
    "createdDateTime": "2020-11-27T23:12:49Z",
    "keyStrength": "normal"
  }
}
```


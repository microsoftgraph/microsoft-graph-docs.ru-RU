---
title: Список windowsHelloForBusinessAuthenticationMethods
description: Получите список объектов windowsHelloForBusinessAuthenticationMethod и их свойств.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: df1f8979ef506eaddd4cf68bb3f60f8da9656d86
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964835"
---
# <a name="list-windowshelloforbusinessauthenticationmethods"></a><span data-ttu-id="1d7d4-103">Список windowsHelloForBusinessAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="1d7d4-103">List windowsHelloForBusinessAuthenticationMethods</span></span>
<span data-ttu-id="1d7d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d7d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d7d4-105">Получите список объектов [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="1d7d4-105">Get a list of the [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d7d4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d7d4-106">Permissions</span></span>

<span data-ttu-id="1d7d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d7d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="1d7d4-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="1d7d4-109">Permissions acting on self</span></span>

|<span data-ttu-id="1d7d4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d7d4-110">Permission type</span></span>      | <span data-ttu-id="1d7d4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d7d4-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="1d7d4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d7d4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d7d4-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d7d4-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="1d7d4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d7d4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d7d4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d7d4-115">Not supported.</span></span> |
| <span data-ttu-id="1d7d4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d7d4-116">Application</span></span>                            | <span data-ttu-id="1d7d4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d7d4-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="1d7d4-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="1d7d4-118">Permissions acting on other users</span></span>

|<span data-ttu-id="1d7d4-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d7d4-119">Permission type</span></span>      | <span data-ttu-id="1d7d4-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d7d4-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="1d7d4-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d7d4-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d7d4-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7d4-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="1d7d4-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d7d4-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d7d4-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d7d4-124">Not supported.</span></span> |
| <span data-ttu-id="1d7d4-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d7d4-125">Application</span></span>                            | <span data-ttu-id="1d7d4-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7d4-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="1d7d4-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="1d7d4-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="1d7d4-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1d7d4-128">Global admin</span></span>
* <span data-ttu-id="1d7d4-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="1d7d4-129">Global reader</span></span>
* <span data-ttu-id="1d7d4-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="1d7d4-130">Privileged authentication admin</span></span>
* <span data-ttu-id="1d7d4-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="1d7d4-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="1d7d4-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d7d4-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/windowsHelloForBusinessMethods
GET /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d7d4-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1d7d4-133">Optional query parameters</span></span>

<span data-ttu-id="1d7d4-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d7d4-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d7d4-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d7d4-135">Request headers</span></span>
|<span data-ttu-id="1d7d4-136">Имя</span><span class="sxs-lookup"><span data-stu-id="1d7d4-136">Name</span></span>|<span data-ttu-id="1d7d4-137">Описание</span><span class="sxs-lookup"><span data-stu-id="1d7d4-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1d7d4-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d7d4-138">Authorization</span></span>|<span data-ttu-id="1d7d4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d7d4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d7d4-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d7d4-141">Request body</span></span>
<span data-ttu-id="1d7d4-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d7d4-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d7d4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d7d4-143">Response</span></span>

<span data-ttu-id="1d7d4-144">В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` [объектов windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1d7d4-144">If successful, this method returns a `200 OK` response code and a collection of [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d7d4-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="1d7d4-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d7d4-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d7d4-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods
```


### <a name="response"></a><span data-ttu-id="1d7d4-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d7d4-147">Response</span></span>
<span data-ttu-id="1d7d4-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1d7d4-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsHelloForBusinessAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
      "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
      "displayName": "Jordan's Surface Book",
      "createdDateTime": "2020-11-27T23:12:49Z",
      "keyStrength": "normal"
    },
    {
      "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
      "id": "e6dab818-e68d-433e-89d5-547357870cb2",
      "displayName": "New Surface Duo",
      "createdDateTime": "2020-12-25T02:20:13Z",
      "keyStrength": "normal"
    }
  ]
}
```


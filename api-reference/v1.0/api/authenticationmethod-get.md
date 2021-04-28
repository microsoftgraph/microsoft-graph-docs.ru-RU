---
title: Получить проверку подлинностиMethod
description: Извлечение свойств и связей объекта authenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 40f5a7ec777e17b1b19c7f33f354c607f53b5480
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054625"
---
# <a name="get-authenticationmethod"></a><span data-ttu-id="54d75-103">Получить проверку подлинностиMethod</span><span class="sxs-lookup"><span data-stu-id="54d75-103">Get authenticationMethod</span></span>

<span data-ttu-id="54d75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54d75-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54d75-105">Извлечение свойств и связей объекта [authenticationMethod.](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="54d75-105">Retrieve the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="54d75-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54d75-106">Permissions</span></span>

<span data-ttu-id="54d75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54d75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="54d75-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="54d75-109">Permissions acting on self</span></span>

|<span data-ttu-id="54d75-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54d75-110">Permission type</span></span>      | <span data-ttu-id="54d75-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54d75-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="54d75-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54d75-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="54d75-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54d75-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="54d75-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54d75-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54d75-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54d75-115">Not supported.</span></span> |
| <span data-ttu-id="54d75-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54d75-116">Application</span></span>                            | <span data-ttu-id="54d75-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54d75-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="54d75-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="54d75-118">Permissions acting on other users</span></span>

|<span data-ttu-id="54d75-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54d75-119">Permission type</span></span>      | <span data-ttu-id="54d75-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54d75-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="54d75-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54d75-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="54d75-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54d75-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="54d75-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54d75-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54d75-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54d75-124">Not supported.</span></span> |
| <span data-ttu-id="54d75-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54d75-125">Application</span></span>                            | <span data-ttu-id="54d75-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54d75-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="54d75-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="54d75-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="54d75-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="54d75-128">Global admin</span></span>
* <span data-ttu-id="54d75-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="54d75-129">Global reader</span></span>
* <span data-ttu-id="54d75-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="54d75-130">Privileged authentication admin</span></span>
* <span data-ttu-id="54d75-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="54d75-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="54d75-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54d75-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods/{id}
GET /users/{id | userPrincipalName}/authentication/methods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54d75-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="54d75-133">Optional query parameters</span></span>

<span data-ttu-id="54d75-134">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="54d75-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54d75-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54d75-135">Request headers</span></span>

| <span data-ttu-id="54d75-136">Имя</span><span class="sxs-lookup"><span data-stu-id="54d75-136">Name</span></span>      |<span data-ttu-id="54d75-137">Описание</span><span class="sxs-lookup"><span data-stu-id="54d75-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54d75-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54d75-138">Authorization</span></span> | <span data-ttu-id="54d75-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54d75-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54d75-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54d75-141">Request body</span></span>

<span data-ttu-id="54d75-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54d75-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54d75-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="54d75-143">Response</span></span>

<span data-ttu-id="54d75-144">В случае успешной работы этот метод возвращает код ответа и запрашиваемую проверку `200 OK` [подлинностиMethod](../resources/authenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="54d75-144">If successful, this method returns a `200 OK` response code and the requested [authenticationMethod](../resources/authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54d75-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="54d75-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54d75-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="54d75-146">Request</span></span>

<span data-ttu-id="54d75-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54d75-147">The following is an example of the request.</span></span>


```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/authentication/methods/{id}
```

### <a name="response"></a><span data-ttu-id="54d75-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="54d75-148">Response</span></span>

<span data-ttu-id="54d75-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="54d75-149">The following is an example of the response.</span></span>

> <span data-ttu-id="54d75-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="54d75-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
    "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
    "displayName": "Jordan's Surface Book",
    "createdDateTime": "2020-11-27T23:12:49Z",
    "keyStrength": "normal"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

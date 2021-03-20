---
title: Получить проверку подлинностиMethod
description: Извлечение свойств и связей объекта authenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ff118645edf0a303c5017d11e7cdbb1e770bab58
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949068"
---
# <a name="get-authenticationmethod"></a><span data-ttu-id="994d1-103">Получить проверку подлинностиMethod</span><span class="sxs-lookup"><span data-stu-id="994d1-103">Get authenticationMethod</span></span>

<span data-ttu-id="994d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="994d1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="994d1-105">Извлечение свойств и связей объекта [authenticationMethod.](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="994d1-105">Retrieve the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="994d1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="994d1-106">Permissions</span></span>

<span data-ttu-id="994d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="994d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="994d1-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="994d1-109">Permissions acting on self</span></span>

|<span data-ttu-id="994d1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="994d1-110">Permission type</span></span>      | <span data-ttu-id="994d1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="994d1-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="994d1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="994d1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="994d1-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="994d1-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="994d1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="994d1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="994d1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="994d1-115">Not supported.</span></span> |
| <span data-ttu-id="994d1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="994d1-116">Application</span></span>                            | <span data-ttu-id="994d1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="994d1-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="994d1-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="994d1-118">Permissions acting on other users</span></span>

|<span data-ttu-id="994d1-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="994d1-119">Permission type</span></span>      | <span data-ttu-id="994d1-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="994d1-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="994d1-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="994d1-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="994d1-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="994d1-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="994d1-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="994d1-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="994d1-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="994d1-124">Not supported.</span></span> |
| <span data-ttu-id="994d1-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="994d1-125">Application</span></span>                            | <span data-ttu-id="994d1-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="994d1-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="994d1-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="994d1-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="994d1-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="994d1-128">Global admin</span></span>
* <span data-ttu-id="994d1-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="994d1-129">Global reader</span></span>
* <span data-ttu-id="994d1-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="994d1-130">Privileged authentication admin</span></span>
* <span data-ttu-id="994d1-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="994d1-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="994d1-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="994d1-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods/{id}
GET /users/{id | userPrincipalName}/authentication/methods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="994d1-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="994d1-133">Optional query parameters</span></span>

<span data-ttu-id="994d1-134">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="994d1-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="994d1-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="994d1-135">Request headers</span></span>

| <span data-ttu-id="994d1-136">Имя</span><span class="sxs-lookup"><span data-stu-id="994d1-136">Name</span></span>      |<span data-ttu-id="994d1-137">Описание</span><span class="sxs-lookup"><span data-stu-id="994d1-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="994d1-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="994d1-138">Authorization</span></span> | <span data-ttu-id="994d1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="994d1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="994d1-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="994d1-141">Request body</span></span>

<span data-ttu-id="994d1-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="994d1-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="994d1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="994d1-143">Response</span></span>

<span data-ttu-id="994d1-144">В случае успешной работы этот метод возвращает код ответа и запрашиваемую проверку `200 OK` [подлинностиMethod](../resources/authenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="994d1-144">If successful, this method returns a `200 OK` response code and the requested [authenticationMethod](../resources/authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="994d1-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="994d1-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="994d1-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="994d1-146">Request</span></span>

<span data-ttu-id="994d1-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="994d1-147">The following is an example of the request.</span></span>


```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/authentication/methods/{id}
```

### <a name="response"></a><span data-ttu-id="994d1-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="994d1-148">Response</span></span>

<span data-ttu-id="994d1-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="994d1-149">The following is an example of the response.</span></span>

> <span data-ttu-id="994d1-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="994d1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

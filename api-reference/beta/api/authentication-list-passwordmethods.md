---
title: Список Пассвордмесодс
description: Получение списка объектов пассвордаусентикатионмесод.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f4425a47e7fede4f82a15fec1b04f0c7de655731
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557671"
---
# <a name="list-passwordmethods"></a><span data-ttu-id="57ca1-103">Список Пассвордмесодс</span><span class="sxs-lookup"><span data-stu-id="57ca1-103">List passwordMethods</span></span>

<span data-ttu-id="57ca1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57ca1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57ca1-105">Получение списка объектов [метода проверки подлинности паролей](../resources/passwordauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="57ca1-105">Retrieve a list of [password authentication method](../resources/passwordauthenticationmethod.md) objects.</span></span> <span data-ttu-id="57ca1-106">При этом будет возвращен ровно один объект, так как пользователь может иметь только один пароль.</span><span class="sxs-lookup"><span data-stu-id="57ca1-106">This will return exactly one object, as a user can have exactly one password.</span></span>

## <a name="permissions"></a><span data-ttu-id="57ca1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57ca1-107">Permissions</span></span>

<span data-ttu-id="57ca1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57ca1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57ca1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57ca1-110">Permission type</span></span>                        | <span data-ttu-id="57ca1-111">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="57ca1-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="57ca1-112">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="57ca1-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="57ca1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57ca1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="57ca1-114">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="57ca1-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="57ca1-115">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="57ca1-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="57ca1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57ca1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57ca1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57ca1-117">Not supported.</span></span> | <span data-ttu-id="57ca1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57ca1-118">Not supported.</span></span> |
| <span data-ttu-id="57ca1-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57ca1-119">Application</span></span>                            | <span data-ttu-id="57ca1-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57ca1-120">Not supported.</span></span> | <span data-ttu-id="57ca1-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57ca1-121">Not supported.</span></span> |

<span data-ttu-id="57ca1-122">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="57ca1-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="57ca1-123">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="57ca1-123">Global admin</span></span>
* <span data-ttu-id="57ca1-124">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="57ca1-124">Global reader</span></span>
* <span data-ttu-id="57ca1-125">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="57ca1-125">Privileged authentication admin</span></span>
* <span data-ttu-id="57ca1-126">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="57ca1-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="57ca1-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57ca1-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods
GET /users/{id}/authentication/passwordMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57ca1-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="57ca1-128">Optional query parameters</span></span>

<span data-ttu-id="57ca1-129">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="57ca1-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57ca1-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57ca1-130">Request headers</span></span>

| <span data-ttu-id="57ca1-131">Имя</span><span class="sxs-lookup"><span data-stu-id="57ca1-131">Name</span></span>      |<span data-ttu-id="57ca1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="57ca1-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="57ca1-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="57ca1-133">Authorization</span></span> | <span data-ttu-id="57ca1-134">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="57ca1-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="57ca1-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="57ca1-135">Request body</span></span>

<span data-ttu-id="57ca1-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57ca1-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57ca1-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="57ca1-137">Response</span></span>

<span data-ttu-id="57ca1-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [пассвордаусентикатионмесод](../resources/passwordauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57ca1-138">If successful, this method returns a `200 OK` response code and a collection of [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57ca1-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="57ca1-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57ca1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="57ca1-140">Request</span></span>

<span data-ttu-id="57ca1-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57ca1-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_passwordmethods"
}-->

```http
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods
```

### <a name="response"></a><span data-ttu-id="57ca1-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="57ca1-142">Response</span></span>

<span data-ttu-id="57ca1-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57ca1-143">The following is an example of the response.</span></span>

> <span data-ttu-id="57ca1-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57ca1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "28c10230-6103-485e-b985-444c60001490",
      "password": null,
      "creationDateTime": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List passwordMethods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
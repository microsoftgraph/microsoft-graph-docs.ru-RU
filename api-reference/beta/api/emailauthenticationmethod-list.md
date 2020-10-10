---
title: Список Емаилаусентикатионмесодс
description: Получение списка объектов Емаилаусентикатионмесод и их свойств.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 92fdd0b55eb10264710550dae63aba6afddeff0c
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418458"
---
# <a name="list-emailauthenticationmethods"></a><span data-ttu-id="dc574-103">Список Емаилаусентикатионмесодс</span><span class="sxs-lookup"><span data-stu-id="dc574-103">List emailAuthenticationMethods</span></span>
<span data-ttu-id="dc574-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc574-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc574-105">Получение списка объектов [метода проверки подлинности электронной почты](../resources/emailauthenticationmethod.md) пользователя и их свойств.</span><span class="sxs-lookup"><span data-stu-id="dc574-105">Retrieve a list of a user's [email Authentication Method](../resources/emailauthenticationmethod.md) objects and their properties.</span></span> <span data-ttu-id="dc574-106">Этот вызов будет возвращать только один объект, так как для пользователей можно задать только один метод электронной почты.</span><span class="sxs-lookup"><span data-stu-id="dc574-106">This call will only return a single object as only one email method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc574-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc574-107">Permissions</span></span>
<span data-ttu-id="dc574-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc574-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc574-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc574-110">Permission type</span></span>|<span data-ttu-id="dc574-111">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc574-111">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="dc574-112">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="dc574-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="dc574-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc574-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc574-114">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dc574-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="dc574-115">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dc574-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="dc574-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc574-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc574-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc574-117">Not supported.</span></span>|<span data-ttu-id="dc574-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc574-118">Not supported.</span></span>
|<span data-ttu-id="dc574-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc574-119">Application</span></span>|<span data-ttu-id="dc574-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc574-120">Not supported.</span></span>|<span data-ttu-id="dc574-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc574-121">Not supported.</span></span>

<span data-ttu-id="dc574-122">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="dc574-122">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="dc574-123">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="dc574-123">Global admin</span></span>
* <span data-ttu-id="dc574-124">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="dc574-124">Global reader</span></span>
* <span data-ttu-id="dc574-125">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="dc574-125">Privileged authentication admin</span></span>
* <span data-ttu-id="dc574-126">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="dc574-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="dc574-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc574-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods
GET /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc574-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dc574-128">Optional query parameters</span></span>
<span data-ttu-id="dc574-129">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="dc574-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc574-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc574-130">Request headers</span></span>
|<span data-ttu-id="dc574-131">Имя</span><span class="sxs-lookup"><span data-stu-id="dc574-131">Name</span></span>|<span data-ttu-id="dc574-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dc574-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dc574-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc574-133">Authorization</span></span>|<span data-ttu-id="dc574-134">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="dc574-134">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc574-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dc574-135">Request body</span></span>
<span data-ttu-id="dc574-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc574-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc574-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc574-137">Response</span></span>

<span data-ttu-id="dc574-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc574-138">If successful, this method returns a `200 OK` response code and a collection of [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc574-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="dc574-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc574-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc574-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods
```


### <a name="response"></a><span data-ttu-id="dc574-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc574-141">Response</span></span>
<span data-ttu-id="dc574-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc574-142">The following is an example of the response.</span></span>

<span data-ttu-id="dc574-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dc574-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.emailAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
      "emailAddress": "Kim@contoso.com"
    }
  ]
}
```


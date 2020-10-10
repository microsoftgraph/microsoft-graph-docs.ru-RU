---
title: Получение Емаилаусентикатионмесод
description: Чтение свойств и связей объекта Емаилаусентикатионмесод.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6041eb67d4bec818ccc25946559bd26a1a7b7bce
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418463"
---
# <a name="get-emailauthenticationmethod"></a><span data-ttu-id="00f77-103">Получение Емаилаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="00f77-103">Get emailAuthenticationMethod</span></span>
<span data-ttu-id="00f77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00f77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00f77-105">Получение объекта [метода проверки подлинности электронной почты](../resources/emailauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="00f77-105">Retrieve a user's single [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="00f77-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00f77-106">Permissions</span></span>
<span data-ttu-id="00f77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00f77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00f77-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00f77-109">Permission type</span></span>|<span data-ttu-id="00f77-110">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="00f77-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="00f77-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="00f77-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="00f77-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00f77-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00f77-113">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="00f77-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="00f77-114">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="00f77-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="00f77-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00f77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00f77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f77-116">Not supported.</span></span>|<span data-ttu-id="00f77-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f77-117">Not supported.</span></span>
|<span data-ttu-id="00f77-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00f77-118">Application</span></span>|<span data-ttu-id="00f77-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f77-119">Not supported.</span></span>|<span data-ttu-id="00f77-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f77-120">Not supported.</span></span>

<span data-ttu-id="00f77-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="00f77-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="00f77-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="00f77-122">Global admin</span></span>
* <span data-ttu-id="00f77-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="00f77-123">Global reader</span></span>
* <span data-ttu-id="00f77-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="00f77-124">Privileged authentication admin</span></span>
* <span data-ttu-id="00f77-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="00f77-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="00f77-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00f77-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods/{id}
GET /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="00f77-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00f77-127">Request headers</span></span>
|<span data-ttu-id="00f77-128">Имя</span><span class="sxs-lookup"><span data-stu-id="00f77-128">Name</span></span>|<span data-ttu-id="00f77-129">Описание</span><span class="sxs-lookup"><span data-stu-id="00f77-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="00f77-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00f77-130">Authorization</span></span>|<span data-ttu-id="00f77-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00f77-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00f77-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00f77-133">Request body</span></span>
<span data-ttu-id="00f77-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00f77-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00f77-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="00f77-135">Response</span></span>

<span data-ttu-id="00f77-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00f77-136">If successful, this method returns a `200 OK` response code and the requested [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00f77-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="00f77-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="00f77-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="00f77-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```


### <a name="response"></a><span data-ttu-id="00f77-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="00f77-139">Response</span></span>
<span data-ttu-id="00f77-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00f77-140">The following is an example of the response.</span></span>

<span data-ttu-id="00f77-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="00f77-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
      "emailAddress": "Kim@contoso.com"
  }
}
```


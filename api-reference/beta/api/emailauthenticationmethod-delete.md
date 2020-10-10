---
title: Удаление Емаилаусентикатионмесод
description: Удаляет объект Емаилаусентикатионмесод.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 281d20e1903e05c4d131f3b2a087d5c1d2043793
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418462"
---
# <a name="delete-emailauthenticationmethod"></a><span data-ttu-id="fde97-103">Удаление Емаилаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="fde97-103">Delete emailAuthenticationMethod</span></span>
<span data-ttu-id="fde97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fde97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fde97-105">Удаляет объект [метода проверки подлинности электронной почты](../resources/emailauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="fde97-105">Deletes a user's [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fde97-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fde97-106">Permissions</span></span>
<span data-ttu-id="fde97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fde97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fde97-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fde97-109">Permission type</span></span>|<span data-ttu-id="fde97-110">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="fde97-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="fde97-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="fde97-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="fde97-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fde97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fde97-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde97-113">Not supported.</span></span>|<span data-ttu-id="fde97-114">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fde97-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="fde97-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fde97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fde97-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde97-116">Not supported.</span></span>|<span data-ttu-id="fde97-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde97-117">Not supported.</span></span>
|<span data-ttu-id="fde97-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fde97-118">Application</span></span>|<span data-ttu-id="fde97-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde97-119">Not supported.</span></span>|<span data-ttu-id="fde97-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde97-120">Not supported.</span></span>

<span data-ttu-id="fde97-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="fde97-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="fde97-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="fde97-122">Global admin</span></span>
* <span data-ttu-id="fde97-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="fde97-123">Global reader</span></span>
* <span data-ttu-id="fde97-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="fde97-124">Privileged authentication admin</span></span>
* <span data-ttu-id="fde97-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="fde97-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="fde97-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fde97-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fde97-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fde97-127">Request headers</span></span>
|<span data-ttu-id="fde97-128">Имя</span><span class="sxs-lookup"><span data-stu-id="fde97-128">Name</span></span>|<span data-ttu-id="fde97-129">Описание</span><span class="sxs-lookup"><span data-stu-id="fde97-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fde97-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fde97-130">Authorization</span></span>|<span data-ttu-id="fde97-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fde97-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fde97-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fde97-133">Request body</span></span>
<span data-ttu-id="fde97-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fde97-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fde97-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fde97-135">Response</span></span>

<span data-ttu-id="fde97-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fde97-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fde97-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="fde97-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fde97-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="fde97-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```


### <a name="response"></a><span data-ttu-id="fde97-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fde97-140">Response</span></span>
<span data-ttu-id="fde97-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fde97-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


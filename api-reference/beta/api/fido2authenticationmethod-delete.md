---
title: Удаление fido2AuthenticationMethod
description: Удаляет объект fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: af396880c260a8e74dc67636015e68e49ce291de
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418423"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="53316-103">Удаление fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="53316-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="53316-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53316-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53316-105">Удаляет объект [метода проверки подлинности для ключа безопасности FIDO2](../resources/fido2authenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="53316-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53316-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53316-106">Permissions</span></span>
<span data-ttu-id="53316-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53316-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53316-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53316-109">Permission type</span></span>|<span data-ttu-id="53316-110">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="53316-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="53316-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="53316-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="53316-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53316-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53316-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53316-113">Not supported.</span></span>|<span data-ttu-id="53316-114">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="53316-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="53316-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53316-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53316-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53316-116">Not supported.</span></span>|<span data-ttu-id="53316-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53316-117">Not supported.</span></span>
|<span data-ttu-id="53316-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53316-118">Application</span></span>|<span data-ttu-id="53316-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53316-119">Not supported.</span></span>|<span data-ttu-id="53316-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53316-120">Not supported.</span></span>

<span data-ttu-id="53316-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="53316-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="53316-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="53316-122">Global admin</span></span>
* <span data-ttu-id="53316-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="53316-123">Global reader</span></span>
* <span data-ttu-id="53316-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="53316-124">Privileged authentication admin</span></span>
* <span data-ttu-id="53316-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="53316-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="53316-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53316-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="53316-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53316-127">Request headers</span></span>
|<span data-ttu-id="53316-128">Имя</span><span class="sxs-lookup"><span data-stu-id="53316-128">Name</span></span>|<span data-ttu-id="53316-129">Описание</span><span class="sxs-lookup"><span data-stu-id="53316-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="53316-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53316-130">Authorization</span></span>|<span data-ttu-id="53316-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53316-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53316-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="53316-133">Request body</span></span>
<span data-ttu-id="53316-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53316-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53316-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="53316-135">Response</span></span>

<span data-ttu-id="53316-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="53316-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53316-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="53316-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53316-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="53316-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="53316-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="53316-140">Response</span></span>
<span data-ttu-id="53316-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="53316-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


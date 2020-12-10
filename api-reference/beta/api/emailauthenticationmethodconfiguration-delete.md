---
title: Удаление Емаилаусентикатионмесодконфигуратион
description: Удаляет объект Емаилаусентикатионмесодконфигуратион.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d5b9ac408a9de38ceb75f8ee04ee3c442705936d
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617137"
---
# <a name="delete-emailauthenticationmethodconfiguration"></a><span data-ttu-id="73ebd-103">Удаление Емаилаусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="73ebd-103">Delete emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="73ebd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73ebd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73ebd-105">Удаление изменений, внесенных в [политику метода проверки подлинности электронной почты](../resources/emailauthenticationmethodconfiguration.md) , путем возврата политики к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="73ebd-105">Remove changes made to the [email authentication method policy](../resources/emailauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="73ebd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73ebd-106">Permissions</span></span>
<span data-ttu-id="73ebd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73ebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73ebd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73ebd-109">Permission type</span></span>|<span data-ttu-id="73ebd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73ebd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73ebd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73ebd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="73ebd-112">Policy. ReadWrite. AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73ebd-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="73ebd-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73ebd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73ebd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73ebd-114">Not supported.</span></span>|
|<span data-ttu-id="73ebd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73ebd-115">Application</span></span>|<span data-ttu-id="73ebd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73ebd-116">Not supported.</span></span>|

<span data-ttu-id="73ebd-117">Для делегированных сценариев администратору требуется одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="73ebd-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="73ebd-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="73ebd-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="73ebd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73ebd-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="73ebd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73ebd-120">Request headers</span></span>

|<span data-ttu-id="73ebd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="73ebd-121">Name</span></span>|<span data-ttu-id="73ebd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="73ebd-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="73ebd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73ebd-123">Authorization</span></span>|<span data-ttu-id="73ebd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73ebd-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73ebd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73ebd-126">Request body</span></span>

<span data-ttu-id="73ebd-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73ebd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73ebd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="73ebd-128">Response</span></span>

<span data-ttu-id="73ebd-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="73ebd-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="73ebd-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="73ebd-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73ebd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="73ebd-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethodconfiguration"
}
-->

```http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

### <a name="response"></a><span data-ttu-id="73ebd-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="73ebd-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```


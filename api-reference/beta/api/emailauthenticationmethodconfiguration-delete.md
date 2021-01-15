---
title: Удаление emailAuthenticationMethodConfiguration
description: Удаляет объект emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 479162c2ff7215b8926ed954d58efaedec84fe88
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49871906"
---
# <a name="delete-emailauthenticationmethodconfiguration"></a><span data-ttu-id="c6741-103">Удаление emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="c6741-103">Delete emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="c6741-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6741-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6741-105">Удалите изменения, [внесенные](../resources/emailauthenticationmethodconfiguration.md) в политику метода проверки подлинности электронной почты, вернув политику к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c6741-105">Remove changes made to the [email authentication method policy](../resources/emailauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6741-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6741-106">Permissions</span></span>
<span data-ttu-id="c6741-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6741-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6741-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6741-109">Permission type</span></span>|<span data-ttu-id="c6741-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6741-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6741-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6741-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c6741-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c6741-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="c6741-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6741-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6741-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6741-114">Not supported.</span></span>|
|<span data-ttu-id="c6741-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6741-115">Application</span></span>|<span data-ttu-id="c6741-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6741-116">Not supported.</span></span>|

<span data-ttu-id="c6741-117">Для делегирования сценариев администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="c6741-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="c6741-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="c6741-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="c6741-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6741-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="c6741-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6741-120">Request headers</span></span>

|<span data-ttu-id="c6741-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c6741-121">Name</span></span>|<span data-ttu-id="c6741-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c6741-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c6741-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6741-123">Authorization</span></span>|<span data-ttu-id="c6741-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6741-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6741-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6741-126">Request body</span></span>

<span data-ttu-id="c6741-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6741-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6741-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6741-128">Response</span></span>

<span data-ttu-id="c6741-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c6741-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c6741-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="c6741-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c6741-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6741-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethodconfiguration"
}
-->

```http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

### <a name="response"></a><span data-ttu-id="c6741-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6741-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```


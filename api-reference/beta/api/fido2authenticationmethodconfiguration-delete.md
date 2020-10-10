---
title: Удаление fido2AuthenticationMethodConfiguration
description: Удаление объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8dbb2b7d2c8948763ffc48ac299cc3f2f330498a
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418419"
---
# <a name="delete-fido2authenticationmethodconfiguration"></a><span data-ttu-id="6afa2-103">Удаление fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="6afa2-103">Delete fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="6afa2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6afa2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6afa2-105">Удаление изменений, внесенных в [политику метода проверки подлинности FIDO2](../resources/fido2authenticationmethodconfiguration.md) , путем возврата политики к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6afa2-105">Remove changes made to the [FIDO2 authentication method policy](../resources/fido2authenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="6afa2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6afa2-106">Permissions</span></span>
<span data-ttu-id="6afa2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6afa2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6afa2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6afa2-109">Permission type</span></span>|<span data-ttu-id="6afa2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6afa2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6afa2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6afa2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6afa2-112">Policy. ReadWrite. AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6afa2-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="6afa2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6afa2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6afa2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6afa2-114">Not supported.</span></span>|
|<span data-ttu-id="6afa2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6afa2-115">Application</span></span>|<span data-ttu-id="6afa2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6afa2-116">Not supported.</span></span>|

<span data-ttu-id="6afa2-117">Для делегированных сценариев администратору требуется одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="6afa2-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="6afa2-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6afa2-118">Global admin</span></span>
* <span data-ttu-id="6afa2-119">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="6afa2-119">Global reader</span></span>
* <span data-ttu-id="6afa2-120">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="6afa2-120">Privileged authentication admin</span></span>
* <span data-ttu-id="6afa2-121">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="6afa2-121">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="6afa2-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6afa2-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="6afa2-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6afa2-123">Request headers</span></span>
|<span data-ttu-id="6afa2-124">Имя</span><span class="sxs-lookup"><span data-stu-id="6afa2-124">Name</span></span>|<span data-ttu-id="6afa2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="6afa2-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6afa2-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6afa2-126">Authorization</span></span>|<span data-ttu-id="6afa2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6afa2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6afa2-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6afa2-129">Request body</span></span>
<span data-ttu-id="6afa2-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6afa2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6afa2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6afa2-131">Response</span></span>

<span data-ttu-id="6afa2-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6afa2-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6afa2-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="6afa2-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6afa2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6afa2-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="6afa2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6afa2-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


---
title: 'riskyUser: confirmCompromised'
description: Подтверждение скомпрометации пользователя
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 193baf4a8e450f0fc05812da8cb48440ebfccab1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440096"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="04dc8-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="04dc8-103">riskyUser: confirmCompromised</span></span>
<span data-ttu-id="04dc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04dc8-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="04dc8-105">**Примечание:** API riskyUsers требует лицензии Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="04dc8-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="04dc8-106">Подтвердим, что один или несколько [объектов riskyUser](../resources/riskyuser.md) могут быть скомпрометированы.</span><span class="sxs-lookup"><span data-stu-id="04dc8-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="04dc8-107">Это действие задает высокий уровень риска целевого пользователя.</span><span class="sxs-lookup"><span data-stu-id="04dc8-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="04dc8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04dc8-108">Permissions</span></span>
<span data-ttu-id="04dc8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="04dc8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="04dc8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04dc8-111">Permission type</span></span>      | <span data-ttu-id="04dc8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04dc8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04dc8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04dc8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="04dc8-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04dc8-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="04dc8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04dc8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04dc8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04dc8-116">Not supported.</span></span>    |
|<span data-ttu-id="04dc8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04dc8-117">Application</span></span> | <span data-ttu-id="04dc8-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04dc8-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04dc8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04dc8-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/confirmCompromised
```

## <a name="request-headers"></a><span data-ttu-id="04dc8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04dc8-120">Request headers</span></span>
|<span data-ttu-id="04dc8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="04dc8-121">Name</span></span>|<span data-ttu-id="04dc8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="04dc8-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="04dc8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04dc8-123">Authorization</span></span>|<span data-ttu-id="04dc8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04dc8-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="04dc8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04dc8-126">Content-Type</span></span>|<span data-ttu-id="04dc8-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04dc8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04dc8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04dc8-129">Request body</span></span>
<span data-ttu-id="04dc8-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04dc8-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="04dc8-131">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="04dc8-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="04dc8-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="04dc8-132">Parameter</span></span>|<span data-ttu-id="04dc8-133">Тип</span><span class="sxs-lookup"><span data-stu-id="04dc8-133">Type</span></span>|<span data-ttu-id="04dc8-134">Описание</span><span class="sxs-lookup"><span data-stu-id="04dc8-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04dc8-135">userIds</span><span class="sxs-lookup"><span data-stu-id="04dc8-135">userIds</span></span>|<span data-ttu-id="04dc8-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="04dc8-136">String collection</span></span>|<span data-ttu-id="04dc8-137">Укажите рискованные пользовательские ИД, которые необходимо отклонять в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="04dc8-137">Specify the risky user IDs to dismiss in the request body.</span></span>|



## <a name="response"></a><span data-ttu-id="04dc8-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="04dc8-138">Response</span></span>

<span data-ttu-id="04dc8-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04dc8-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="04dc8-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="04dc8-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04dc8-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="04dc8-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "riskyuser_confirmcompromised"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised
Content-Type: application/json
Content-length: 39

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```


### <a name="response"></a><span data-ttu-id="04dc8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="04dc8-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



---
title: 'Рискюсер: Конфирмкомпромисед'
description: Подтверждение того, что пользователь скомпрометирован
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3ff671b2dd15057f3bfc93634f00e2caebe9d3bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023102"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="29e1b-103">Рискюсер: Конфирмкомпромисед</span><span class="sxs-lookup"><span data-stu-id="29e1b-103">riskyUser: confirmCompromised</span></span>
<span data-ttu-id="29e1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29e1b-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="29e1b-105">**Примечание:** Для API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="29e1b-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="29e1b-106">Подтвердите, что один или несколько объектов [рискюсер](../resources/riskyuser.md) считаются скомпрометированными.</span><span class="sxs-lookup"><span data-stu-id="29e1b-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="29e1b-107">Это действие устанавливает высокий уровень риска для целевого пользователя.</span><span class="sxs-lookup"><span data-stu-id="29e1b-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="29e1b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29e1b-108">Permissions</span></span>
<span data-ttu-id="29e1b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="29e1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="29e1b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29e1b-111">Permission type</span></span>      | <span data-ttu-id="29e1b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29e1b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29e1b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29e1b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="29e1b-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29e1b-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="29e1b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29e1b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29e1b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29e1b-116">Not supported.</span></span>    |
|<span data-ttu-id="29e1b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29e1b-117">Application</span></span> | <span data-ttu-id="29e1b-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29e1b-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29e1b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29e1b-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/confirmCompromised
```

## <a name="request-headers"></a><span data-ttu-id="29e1b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29e1b-120">Request headers</span></span>
|<span data-ttu-id="29e1b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="29e1b-121">Name</span></span>|<span data-ttu-id="29e1b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="29e1b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="29e1b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29e1b-123">Authorization</span></span>|<span data-ttu-id="29e1b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29e1b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="29e1b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29e1b-126">Content-Type</span></span>|<span data-ttu-id="29e1b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29e1b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29e1b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29e1b-129">Request body</span></span>
<span data-ttu-id="29e1b-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29e1b-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="29e1b-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="29e1b-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="29e1b-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="29e1b-132">Parameter</span></span>|<span data-ttu-id="29e1b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="29e1b-133">Type</span></span>|<span data-ttu-id="29e1b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="29e1b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29e1b-135">userIds</span><span class="sxs-lookup"><span data-stu-id="29e1b-135">userIds</span></span>|<span data-ttu-id="29e1b-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="29e1b-136">String collection</span></span>|<span data-ttu-id="29e1b-137">Укажите рискованные идентификаторы пользователей, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="29e1b-137">Specify the risky user IDs to dismiss in the request body.</span></span>|



## <a name="response"></a><span data-ttu-id="29e1b-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="29e1b-138">Response</span></span>

<span data-ttu-id="29e1b-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="29e1b-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="29e1b-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="29e1b-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="29e1b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="29e1b-141">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="29e1b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="29e1b-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



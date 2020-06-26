---
title: 'Рискюсер: Конфирмкомпромисед'
description: Подтверждение того, что пользователь скомпрометирован
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f82194dff2e805fe73d11ad4301a0e2c74347335
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897591"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="ef932-103">Рискюсер: Конфирмкомпромисед</span><span class="sxs-lookup"><span data-stu-id="ef932-103">riskyUser: confirmCompromised</span></span>
<span data-ttu-id="ef932-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef932-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="ef932-105">**Примечание:** Для API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="ef932-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="ef932-106">Подтвердите, что один или несколько объектов [рискюсер](../resources/riskyuser.md) считаются скомпрометированными.</span><span class="sxs-lookup"><span data-stu-id="ef932-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="ef932-107">Это действие устанавливает высокий уровень риска для целевого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef932-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef932-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef932-108">Permissions</span></span>
<span data-ttu-id="ef932-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ef932-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ef932-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="ef932-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="ef932-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef932-111">Permission type</span></span>      | <span data-ttu-id="ef932-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef932-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef932-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef932-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ef932-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef932-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef932-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef932-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef932-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef932-116">Not supported.</span></span>    |
|<span data-ttu-id="ef932-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ef932-117">Application</span></span> | <span data-ttu-id="ef932-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef932-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef932-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef932-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/confirmCompromised
```

## <a name="request-headers"></a><span data-ttu-id="ef932-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef932-120">Request headers</span></span>
|<span data-ttu-id="ef932-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ef932-121">Name</span></span>|<span data-ttu-id="ef932-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ef932-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ef932-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef932-123">Authorization</span></span>|<span data-ttu-id="ef932-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="ef932-124">Bearer {token}.</span></span> <span data-ttu-id="ef932-125">Required.</span><span class="sxs-lookup"><span data-stu-id="ef932-125">Required.</span></span>|
|<span data-ttu-id="ef932-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef932-126">Content-Type</span></span>|<span data-ttu-id="ef932-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="ef932-127">application/json.</span></span> <span data-ttu-id="ef932-128">Required.</span><span class="sxs-lookup"><span data-stu-id="ef932-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef932-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef932-129">Request body</span></span>
<span data-ttu-id="ef932-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef932-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ef932-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ef932-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ef932-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="ef932-132">Parameter</span></span>|<span data-ttu-id="ef932-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ef932-133">Type</span></span>|<span data-ttu-id="ef932-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ef932-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef932-135">userIds</span><span class="sxs-lookup"><span data-stu-id="ef932-135">userIds</span></span>|<span data-ttu-id="ef932-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ef932-136">String collection</span></span>|<span data-ttu-id="ef932-137">Укажите рискованные идентификаторы пользователей, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="ef932-137">Specify the risky user IDs to dismiss in the request body.</span></span>|



## <a name="response"></a><span data-ttu-id="ef932-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef932-138">Response</span></span>

<span data-ttu-id="ef932-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ef932-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ef932-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="ef932-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ef932-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef932-141">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="ef932-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef932-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


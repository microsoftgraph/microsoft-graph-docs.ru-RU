---
title: 'riskyUser: увольнение'
description: Увольнение рискованного пользователя
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d03d2199d11b2b9f285d8a425e01c70a6a49da35
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440089"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="60d02-103">riskyUser: увольнение</span><span class="sxs-lookup"><span data-stu-id="60d02-103">riskyUser: dismiss</span></span>
<span data-ttu-id="60d02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60d02-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="60d02-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="60d02-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="60d02-106">Отклонять риск одного или более [объектов riskyUser.](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="60d02-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="60d02-107">Это действие задает целевому пользователю уровень риска ни к одному.</span><span class="sxs-lookup"><span data-stu-id="60d02-107">This action sets the targeted user's risk level to none.</span></span>

## <a name="permissions"></a><span data-ttu-id="60d02-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60d02-108">Permissions</span></span>
<span data-ttu-id="60d02-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="60d02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="60d02-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60d02-111">Permission type</span></span>      | <span data-ttu-id="60d02-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60d02-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60d02-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60d02-113">Delegated (work or school account)</span></span> | <span data-ttu-id="60d02-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60d02-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="60d02-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60d02-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60d02-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60d02-116">Not supported.</span></span>    |
|<span data-ttu-id="60d02-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60d02-117">Application</span></span> | <span data-ttu-id="60d02-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60d02-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60d02-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60d02-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/dismiss
```

## <a name="request-headers"></a><span data-ttu-id="60d02-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60d02-120">Request headers</span></span>
|<span data-ttu-id="60d02-121">Имя</span><span class="sxs-lookup"><span data-stu-id="60d02-121">Name</span></span>|<span data-ttu-id="60d02-122">Описание</span><span class="sxs-lookup"><span data-stu-id="60d02-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="60d02-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60d02-123">Authorization</span></span>|<span data-ttu-id="60d02-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60d02-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="60d02-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60d02-126">Content-Type</span></span>|<span data-ttu-id="60d02-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60d02-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60d02-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60d02-129">Request body</span></span>
<span data-ttu-id="60d02-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60d02-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="60d02-131">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="60d02-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="60d02-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="60d02-132">Parameter</span></span>|<span data-ttu-id="60d02-133">Тип</span><span class="sxs-lookup"><span data-stu-id="60d02-133">Type</span></span>|<span data-ttu-id="60d02-134">Описание</span><span class="sxs-lookup"><span data-stu-id="60d02-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60d02-135">userIds</span><span class="sxs-lookup"><span data-stu-id="60d02-135">userIds</span></span>|<span data-ttu-id="60d02-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="60d02-136">String collection</span></span>|<span data-ttu-id="60d02-137">Укажите пользовательские интерфейсы, которые необходимо отклонять в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="60d02-137">Specify the userIds to dismiss in the request body.</span></span>|



## <a name="response"></a><span data-ttu-id="60d02-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="60d02-138">Response</span></span>

<span data-ttu-id="60d02-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="60d02-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="60d02-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="60d02-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60d02-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="60d02-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "riskyuser_dismiss"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss
Content-Type: application/json
Content-length: 39

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```


### <a name="response"></a><span data-ttu-id="60d02-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="60d02-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



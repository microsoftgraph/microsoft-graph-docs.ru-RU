---
title: 'пользователь: активироватьServicePlan'
description: Активация плана службы с `servicePlanId` заданным и для данного `skuId` пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 70849865237a82f4a0bb5fcee22263291627c21d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578868"
---
# <a name="user-activateserviceplan"></a><span data-ttu-id="97982-103">пользователь: активироватьServicePlan</span><span class="sxs-lookup"><span data-stu-id="97982-103">user: activateServicePlan</span></span>

<span data-ttu-id="97982-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97982-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97982-105">Активация плана службы с `servicePlanId` заданным и для данного `skuId` пользователя.</span><span class="sxs-lookup"><span data-stu-id="97982-105">Activate a service plan with a given `servicePlanId` and `skuId` for a given user.</span></span>

## <a name="permissions"></a><span data-ttu-id="97982-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97982-106">Permissions</span></span>

<span data-ttu-id="97982-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97982-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97982-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97982-109">Permission type</span></span>|<span data-ttu-id="97982-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97982-110">Permissions (from most to least privileged)</span></span>|
| :--- | :--- |
| <span data-ttu-id="97982-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97982-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97982-112">Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All</span><span class="sxs-lookup"><span data-stu-id="97982-112">Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All</span></span> |
| <span data-ttu-id="97982-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97982-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97982-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97982-114">Not Supported.</span></span> |
| <span data-ttu-id="97982-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="97982-115">Application</span></span> | <span data-ttu-id="97982-116">Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All</span><span class="sxs-lookup"><span data-stu-id="97982-116">Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97982-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97982-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /users/{id | userPrincipalName}/activateServicePlan
```

## <a name="request-headers"></a><span data-ttu-id="97982-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97982-118">Request headers</span></span>

| <span data-ttu-id="97982-119">Имя</span><span class="sxs-lookup"><span data-stu-id="97982-119">Name</span></span> | <span data-ttu-id="97982-120">Описание</span><span class="sxs-lookup"><span data-stu-id="97982-120">Description</span></span> |
| :--- | :--- |
| <span data-ttu-id="97982-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97982-121">Authorization</span></span> | <span data-ttu-id="97982-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97982-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97982-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97982-124">Content-Type</span></span> | <span data-ttu-id="97982-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97982-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97982-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97982-127">Request body</span></span>

<span data-ttu-id="97982-128">В теле запроса укажи объект JSON со следующим параметром:</span><span class="sxs-lookup"><span data-stu-id="97982-128">In the request body, provide a JSON object with the following parameter:</span></span>

| <span data-ttu-id="97982-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="97982-129">Parameter</span></span> | <span data-ttu-id="97982-130">Тип</span><span class="sxs-lookup"><span data-stu-id="97982-130">Type</span></span> | <span data-ttu-id="97982-131">Описание</span><span class="sxs-lookup"><span data-stu-id="97982-131">Description</span></span> |
| :--- | :--- | :--- |
| <span data-ttu-id="97982-132">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="97982-132">servicePlanId</span></span> | <span data-ttu-id="97982-133">Guid</span><span class="sxs-lookup"><span data-stu-id="97982-133">Guid</span></span> | <span data-ttu-id="97982-134">PlanId servicePlan для активации.</span><span class="sxs-lookup"><span data-stu-id="97982-134">PlanId of the ServicePlan to activate.</span></span> |
| <span data-ttu-id="97982-135">skuId</span><span class="sxs-lookup"><span data-stu-id="97982-135">skuId</span></span> | <span data-ttu-id="97982-136">Guid</span><span class="sxs-lookup"><span data-stu-id="97982-136">Guid</span></span> | <span data-ttu-id="97982-137">SkuId SKU, в планах службы.</span><span class="sxs-lookup"><span data-stu-id="97982-137">SkuId of SKU the service plan is on.</span></span> |

## <a name="response"></a><span data-ttu-id="97982-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="97982-138">Response</span></span>

<span data-ttu-id="97982-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="97982-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="97982-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="97982-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="97982-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="97982-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "user_activateserviceplan"
}
-->

``` http
POST https://graph.microsoft.com/beta/me/activateServicePlan
Content-type: application/json
Content-length: 115

{
  "servicePlanId": "28f42d6f-8034-4a0f-9d8a-a218a63b3299",
  "skuId": "465a2a90-5e59-456d-a7b8-127b9fb2e484"
}
```

### <a name="response"></a><span data-ttu-id="97982-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="97982-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```

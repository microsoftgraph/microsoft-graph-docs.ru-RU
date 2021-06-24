---
title: 'организация: активироватьService'
description: Активирует службу для организации.
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6008b7f5a597af5ac65b349af22879b9db1255f4
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109260"
---
# <a name="organization-activateservice"></a><span data-ttu-id="318c5-103">организация: активироватьService</span><span class="sxs-lookup"><span data-stu-id="318c5-103">organization: activateService</span></span>

<span data-ttu-id="318c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="318c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="318c5-105">Активация службы для организации.</span><span class="sxs-lookup"><span data-stu-id="318c5-105">Activate a service for an organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="318c5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="318c5-106">Permissions</span></span>
<span data-ttu-id="318c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="318c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="318c5-109">Чтобы активировать службу для организации, запросчик  должен иметь роль администратора компании со следующими разрешениями.</span><span class="sxs-lookup"><span data-stu-id="318c5-109">In order to activate a service for an organization the requestor needs to have the _Company Administrator_ role with the following permissions.</span></span>

|<span data-ttu-id="318c5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="318c5-110">Permission type</span></span>|<span data-ttu-id="318c5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="318c5-111">Permissions (from least to most privileged)</span></span>|
| :--- | :--- |
| <span data-ttu-id="318c5-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="318c5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="318c5-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="318c5-113">Directory.ReadWrite.All</span></span>|
| <span data-ttu-id="318c5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="318c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="318c5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="318c5-115">Not Supported.</span></span> |
| <span data-ttu-id="318c5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="318c5-116">Application</span></span> | <span data-ttu-id="318c5-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="318c5-117">Directory.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="318c5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="318c5-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/activateService
```

## <a name="request-headers"></a><span data-ttu-id="318c5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="318c5-119">Request headers</span></span>
|<span data-ttu-id="318c5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="318c5-120">Name</span></span>|<span data-ttu-id="318c5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="318c5-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="318c5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="318c5-122">Authorization</span></span>|<span data-ttu-id="318c5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="318c5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="318c5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="318c5-125">Content-Type</span></span>|<span data-ttu-id="318c5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="318c5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="318c5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="318c5-128">Request body</span></span>
<span data-ttu-id="318c5-129">В теле запроса поставляем представление JSON объекта [activateService.](../resources/activateService.md)</span><span class="sxs-lookup"><span data-stu-id="318c5-129">In the request body, supply a JSON representation of the [activateService](../resources/activateService.md) object.</span></span>
<span data-ttu-id="318c5-130">Необходимо определить **службу** или **(servicePlanId** _и_ **skuId),** чтобы это действие было допустимым.</span><span class="sxs-lookup"><span data-stu-id="318c5-130">You must define **service** or (**servicePlanId** _and_ **skuId**) for this action to be valid.</span></span>

| <span data-ttu-id="318c5-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="318c5-131">Property</span></span>         | <span data-ttu-id="318c5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="318c5-132">Type</span></span>         | <span data-ttu-id="318c5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="318c5-133">Description</span></span>                           |
| ----------------- | ------------ | ------------------------------------- |
| <span data-ttu-id="318c5-134">service</span><span class="sxs-lookup"><span data-stu-id="318c5-134">service</span></span>| <span data-ttu-id="318c5-135">String</span><span class="sxs-lookup"><span data-stu-id="318c5-135">String</span></span> | <span data-ttu-id="318c5-136">Имя службы для активации.</span><span class="sxs-lookup"><span data-stu-id="318c5-136">The name of the service to activate.</span></span> |
| <span data-ttu-id="318c5-137">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="318c5-137">servicePlanId</span></span> | <span data-ttu-id="318c5-138">Guid</span><span class="sxs-lookup"><span data-stu-id="318c5-138">Guid</span></span> | <span data-ttu-id="318c5-139">Идентификатор плана для активации плана службы.</span><span class="sxs-lookup"><span data-stu-id="318c5-139">The plan identifier of the service plan to activate.</span></span> |
| <span data-ttu-id="318c5-140">skuId</span><span class="sxs-lookup"><span data-stu-id="318c5-140">skuId</span></span> | <span data-ttu-id="318c5-141">Guid</span><span class="sxs-lookup"><span data-stu-id="318c5-141">Guid</span></span> | <span data-ttu-id="318c5-142">Идентификатор SKU плана службы.</span><span class="sxs-lookup"><span data-stu-id="318c5-142">The SKU identifier of the service plan.</span></span> |

## <a name="response"></a><span data-ttu-id="318c5-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="318c5-143">Response</span></span>

<span data-ttu-id="318c5-144">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="318c5-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="318c5-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="318c5-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="318c5-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="318c5-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "organization_activateservice"
}
-->
``` http
POST https://graph.microsoft.com/beta/organization/{:organizationId}/activateService
Content-Type: application/json

{
    "skuId": "6fd2c87f-b296-42f0-b197-1e91e994b900",
    "servicePlanId": "a23b959c-7ce8-4e57-9140-b90eb88a9e97"
}
```

### <a name="response"></a><span data-ttu-id="318c5-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="318c5-147">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
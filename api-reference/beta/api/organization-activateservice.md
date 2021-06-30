---
title: 'организация: активироватьService'
description: Активирует службу для организации.
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c65d864fcfcabab5616113528f3e347238828bc5
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207678"
---
# <a name="organization-activateservice"></a><span data-ttu-id="e4099-103">организация: активироватьService</span><span class="sxs-lookup"><span data-stu-id="e4099-103">organization: activateService</span></span>

<span data-ttu-id="e4099-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4099-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4099-105">Активация службы для организации.</span><span class="sxs-lookup"><span data-stu-id="e4099-105">Activate a service for an organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4099-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4099-106">Permissions</span></span>
<span data-ttu-id="e4099-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e4099-109">Чтобы активировать службу для организации, запросчик  должен иметь роль администратора компании со следующими разрешениями.</span><span class="sxs-lookup"><span data-stu-id="e4099-109">In order to activate a service for an organization the requestor needs to have the _Company Administrator_ role with the following permissions.</span></span>

|<span data-ttu-id="e4099-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4099-110">Permission type</span></span>|<span data-ttu-id="e4099-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4099-111">Permissions (from least to most privileged)</span></span>|
| :--- | :--- |
| <span data-ttu-id="e4099-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4099-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e4099-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4099-113">Directory.ReadWrite.All</span></span>|
| <span data-ttu-id="e4099-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4099-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4099-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4099-115">Not Supported.</span></span> |
| <span data-ttu-id="e4099-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4099-116">Application</span></span> | <span data-ttu-id="e4099-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4099-117">Directory.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="e4099-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4099-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/activateService
```

## <a name="request-headers"></a><span data-ttu-id="e4099-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4099-119">Request headers</span></span>
|<span data-ttu-id="e4099-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e4099-120">Name</span></span>|<span data-ttu-id="e4099-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e4099-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e4099-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4099-122">Authorization</span></span>|<span data-ttu-id="e4099-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4099-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e4099-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4099-125">Content-Type</span></span>|<span data-ttu-id="e4099-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4099-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4099-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4099-128">Request body</span></span>
<span data-ttu-id="e4099-129">В теле запроса поставляем представление JSON объекта [activateService.](../resources/activateService.md)</span><span class="sxs-lookup"><span data-stu-id="e4099-129">In the request body, supply a JSON representation of the [activateService](../resources/activateService.md) object.</span></span>
<span data-ttu-id="e4099-130">Необходимо определить **службу** или **(servicePlanId** _и_ **skuId),** чтобы это действие было допустимым.</span><span class="sxs-lookup"><span data-stu-id="e4099-130">You must define **service** or (**servicePlanId** _and_ **skuId**) for this action to be valid.</span></span>

| <span data-ttu-id="e4099-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4099-131">Property</span></span>         | <span data-ttu-id="e4099-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e4099-132">Type</span></span>         | <span data-ttu-id="e4099-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e4099-133">Description</span></span>                           |
| ----------------- | ------------ | ------------------------------------- |
| <span data-ttu-id="e4099-134">service</span><span class="sxs-lookup"><span data-stu-id="e4099-134">service</span></span>| <span data-ttu-id="e4099-135">String</span><span class="sxs-lookup"><span data-stu-id="e4099-135">String</span></span> | <span data-ttu-id="e4099-136">Имя службы для активации.</span><span class="sxs-lookup"><span data-stu-id="e4099-136">The name of the service to activate.</span></span> |
| <span data-ttu-id="e4099-137">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="e4099-137">servicePlanId</span></span> | <span data-ttu-id="e4099-138">Guid</span><span class="sxs-lookup"><span data-stu-id="e4099-138">Guid</span></span> | <span data-ttu-id="e4099-139">Идентификатор плана для активации плана службы.</span><span class="sxs-lookup"><span data-stu-id="e4099-139">The plan identifier of the service plan to activate.</span></span> |
| <span data-ttu-id="e4099-140">skuId</span><span class="sxs-lookup"><span data-stu-id="e4099-140">skuId</span></span> | <span data-ttu-id="e4099-141">Guid</span><span class="sxs-lookup"><span data-stu-id="e4099-141">Guid</span></span> | <span data-ttu-id="e4099-142">Идентификатор SKU плана службы.</span><span class="sxs-lookup"><span data-stu-id="e4099-142">The SKU identifier of the service plan.</span></span> |

## <a name="response"></a><span data-ttu-id="e4099-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4099-143">Response</span></span>

<span data-ttu-id="e4099-144">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4099-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e4099-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="e4099-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e4099-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4099-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e4099-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4099-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e4099-148">C#</span><span class="sxs-lookup"><span data-stu-id="e4099-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/organization-activateservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4099-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4099-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/organization-activateservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4099-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4099-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/organization-activateservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4099-151">Java</span><span class="sxs-lookup"><span data-stu-id="e4099-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/organization-activateservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e4099-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4099-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

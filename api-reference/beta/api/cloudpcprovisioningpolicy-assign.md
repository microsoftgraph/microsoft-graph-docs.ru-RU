---
title: 'cloudPcProvisioningPolicy: назначение'
description: Назначьте группе политику продюсинга облачных КОМПЬЮТЕРов.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 46d9877b8a17056aee84f1216c4f38227bdc097c
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082199"
---
# <a name="cloudpcprovisioningpolicy-assign"></a><span data-ttu-id="c7c53-103">cloudPcProvisioningPolicy: назначение</span><span class="sxs-lookup"><span data-stu-id="c7c53-103">cloudPcProvisioningPolicy: assign</span></span>

<span data-ttu-id="c7c53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7c53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7c53-105">Назначение [cloudPcProvisioningPolicy группам](../resources/cloudpcprovisioningpolicy.md) пользователей.</span><span class="sxs-lookup"><span data-stu-id="c7c53-105">Assign [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="c7c53-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7c53-106">Permissions</span></span>

<span data-ttu-id="c7c53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7c53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c53-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7c53-109">Permission type</span></span>|<span data-ttu-id="c7c53-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7c53-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7c53-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7c53-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7c53-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c53-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="c7c53-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7c53-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7c53-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7c53-114">Not supported.</span></span>|
|<span data-ttu-id="c7c53-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c7c53-115">Application</span></span>|<span data-ttu-id="c7c53-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c53-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7c53-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7c53-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c7c53-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7c53-118">Request headers</span></span>

|<span data-ttu-id="c7c53-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c7c53-119">Name</span></span>|<span data-ttu-id="c7c53-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c7c53-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c7c53-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7c53-121">Authorization</span></span>|<span data-ttu-id="c7c53-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7c53-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c7c53-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7c53-124">Content-Type</span></span>|<span data-ttu-id="c7c53-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7c53-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7c53-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7c53-127">Request body</span></span>

<span data-ttu-id="c7c53-128">В теле запроса поставляем представление JSON объекта [cloudPcProvisioningPolicyAssignment.](../resources/cloudpcprovisioningpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7c53-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object.</span></span>

|<span data-ttu-id="c7c53-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="c7c53-129">Parameter</span></span>|<span data-ttu-id="c7c53-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c7c53-130">Type</span></span>|<span data-ttu-id="c7c53-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c7c53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7c53-132">assignments</span><span class="sxs-lookup"><span data-stu-id="c7c53-132">assignments</span></span>|<span data-ttu-id="c7c53-133">[коллекция cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7c53-133">[cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) collection</span></span> | <span data-ttu-id="c7c53-134">Коллекция ресурсов политики обеспечения безопасности облачных КОМПЬЮТЕРов, которые будут назначены соответствующей целевой группе.</span><span class="sxs-lookup"><span data-stu-id="c7c53-134">The collection of cloud PC provisioning policy resources each to be assigned to the corresponding target group.</span></span> <span data-ttu-id="c7c53-135">В Microsoft 365 поддерживаются только группы и группы безопасности в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c7c53-135">Only Microsoft 365 groups and security groups in Azure AD are currently supported.</span></span> |

## <a name="response"></a><span data-ttu-id="c7c53-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7c53-136">Response</span></span>

<span data-ttu-id="c7c53-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c7c53-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c7c53-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="c7c53-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7c53-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7c53-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c7c53-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7c53-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "assign_cloudpcprovisioningpolicy",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "assignments": [
    {
      "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      "target":{
        "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="c7c53-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7c53-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/assign-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7c53-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7c53-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/assign-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c7c53-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7c53-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```

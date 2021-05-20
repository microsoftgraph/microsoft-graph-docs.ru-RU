---
title: 'cloudPcProvisioningPolicy: назначение'
description: Назначьте группе политику продюсинга облачных КОМПЬЮТЕРов.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 86671d0fce531445ac32a370d2e69ba813cc4e22
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546828"
---
# <a name="cloudpcprovisioningpolicy-assign"></a><span data-ttu-id="02dba-103">cloudPcProvisioningPolicy: назначение</span><span class="sxs-lookup"><span data-stu-id="02dba-103">cloudPcProvisioningPolicy: assign</span></span>

<span data-ttu-id="02dba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02dba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02dba-105">Назначение [cloudPcProvisioningPolicy группам](../resources/cloudpcprovisioningpolicy.md) пользователей.</span><span class="sxs-lookup"><span data-stu-id="02dba-105">Assign [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="02dba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02dba-106">Permissions</span></span>

<span data-ttu-id="02dba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02dba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02dba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02dba-109">Permission type</span></span>|<span data-ttu-id="02dba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02dba-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02dba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02dba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02dba-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02dba-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="02dba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02dba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02dba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02dba-114">Not supported.</span></span>|
|<span data-ttu-id="02dba-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="02dba-115">Application</span></span>|<span data-ttu-id="02dba-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02dba-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02dba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02dba-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="02dba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02dba-118">Request headers</span></span>

|<span data-ttu-id="02dba-119">Имя</span><span class="sxs-lookup"><span data-stu-id="02dba-119">Name</span></span>|<span data-ttu-id="02dba-120">Описание</span><span class="sxs-lookup"><span data-stu-id="02dba-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="02dba-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02dba-121">Authorization</span></span>|<span data-ttu-id="02dba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02dba-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="02dba-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02dba-124">Content-Type</span></span>|<span data-ttu-id="02dba-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02dba-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02dba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02dba-127">Request body</span></span>

<span data-ttu-id="02dba-128">В теле запроса поставляем представление JSON объекта [cloudPcProvisioningPolicyAssignment.](../resources/cloudpcprovisioningpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="02dba-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object.</span></span>

<span data-ttu-id="02dba-129">В следующей таблице показаны свойства, необходимые при создании [cloudPcProvisioningPolicyAssignment.](../resources/cloudpcprovisioningpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="02dba-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md).</span></span>

|<span data-ttu-id="02dba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="02dba-130">Property</span></span>|<span data-ttu-id="02dba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="02dba-131">Type</span></span>|<span data-ttu-id="02dba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="02dba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02dba-133">id</span><span class="sxs-lookup"><span data-stu-id="02dba-133">id</span></span>|<span data-ttu-id="02dba-134">String</span><span class="sxs-lookup"><span data-stu-id="02dba-134">String</span></span>|<span data-ttu-id="02dba-135">ID назначения политики обеспечения.</span><span class="sxs-lookup"><span data-stu-id="02dba-135">The ID of the provisioning policy assignment.</span></span> <span data-ttu-id="02dba-136">Если целью является группа пользователей, то ID отображается как {policyId}_{groupId}.</span><span class="sxs-lookup"><span data-stu-id="02dba-136">If target is a user group, then the ID is shown as {policyId}_{groupId}.</span></span> |
|<span data-ttu-id="02dba-137">target</span><span class="sxs-lookup"><span data-stu-id="02dba-137">target</span></span>|[<span data-ttu-id="02dba-138">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="02dba-138">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="02dba-139">Цель назначения для политики обеспечения.</span><span class="sxs-lookup"><span data-stu-id="02dba-139">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="02dba-140">В настоящее время единственной поддерживаемой целевой группой является группа пользователей.</span><span class="sxs-lookup"><span data-stu-id="02dba-140">Currently, the only target supported is a user group.</span></span>|

## <a name="response"></a><span data-ttu-id="02dba-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="02dba-141">Response</span></span>

<span data-ttu-id="02dba-142">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="02dba-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="02dba-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="02dba-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02dba-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="02dba-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="02dba-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="02dba-145">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="02dba-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02dba-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/assign-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02dba-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02dba-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/assign-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02dba-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="02dba-148">Response</span></span>

<span data-ttu-id="02dba-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="02dba-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```

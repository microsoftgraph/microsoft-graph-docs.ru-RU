---
title: 'Клаудпкпровисионингполици: назначение'
description: Назначьте политику подготовки облачных ПК для группы.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: cb6efee682b07d19c6638803aa24e1f489310282
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563438"
---
# <a name="cloudpcprovisioningpolicy-assign"></a><span data-ttu-id="26b28-103">Клаудпкпровисионингполици: назначение</span><span class="sxs-lookup"><span data-stu-id="26b28-103">cloudPcProvisioningPolicy: assign</span></span>

<span data-ttu-id="26b28-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26b28-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26b28-105">Назначьте [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) группам пользователей.</span><span class="sxs-lookup"><span data-stu-id="26b28-105">Assign [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="26b28-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26b28-106">Permissions</span></span>

<span data-ttu-id="26b28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26b28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26b28-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26b28-109">Permission type</span></span>|<span data-ttu-id="26b28-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26b28-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26b28-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26b28-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26b28-112">Клаудпк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="26b28-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="26b28-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26b28-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26b28-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26b28-114">Not supported.</span></span>|
|<span data-ttu-id="26b28-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26b28-115">Application</span></span>|<span data-ttu-id="26b28-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26b28-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26b28-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26b28-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="26b28-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26b28-118">Request headers</span></span>

|<span data-ttu-id="26b28-119">Имя</span><span class="sxs-lookup"><span data-stu-id="26b28-119">Name</span></span>|<span data-ttu-id="26b28-120">Описание</span><span class="sxs-lookup"><span data-stu-id="26b28-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="26b28-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26b28-121">Authorization</span></span>|<span data-ttu-id="26b28-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26b28-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="26b28-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26b28-124">Content-Type</span></span>|<span data-ttu-id="26b28-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26b28-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26b28-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26b28-127">Request body</span></span>

<span data-ttu-id="26b28-128">В тексте запроса добавьте представление объекта [клаудпкпровисионингполициассигнмент](../resources/cloudpcprovisioningpolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26b28-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object.</span></span>

<span data-ttu-id="26b28-129">В следующей таблице приведены свойства, необходимые при создании [клаудпкпровисионингполициассигнмент](../resources/cloudpcprovisioningpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="26b28-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md).</span></span>

|<span data-ttu-id="26b28-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="26b28-130">Property</span></span>|<span data-ttu-id="26b28-131">Тип</span><span class="sxs-lookup"><span data-stu-id="26b28-131">Type</span></span>|<span data-ttu-id="26b28-132">Описание</span><span class="sxs-lookup"><span data-stu-id="26b28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26b28-133">id</span><span class="sxs-lookup"><span data-stu-id="26b28-133">id</span></span>|<span data-ttu-id="26b28-134">String</span><span class="sxs-lookup"><span data-stu-id="26b28-134">String</span></span>|<span data-ttu-id="26b28-135">Идентификатор назначения политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="26b28-135">The ID of the provisioning policy assignment.</span></span> <span data-ttu-id="26b28-136">Если целевой объект — группа пользователей, идентификатор отображается как {Полициид} _ {groupId}.</span><span class="sxs-lookup"><span data-stu-id="26b28-136">If target is a user group, then the ID is shown as {policyId}_{groupId}.</span></span> |
|<span data-ttu-id="26b28-137">target</span><span class="sxs-lookup"><span data-stu-id="26b28-137">target</span></span>|[<span data-ttu-id="26b28-138">клаудпкманажементассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="26b28-138">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="26b28-139">Цель назначения для политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="26b28-139">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="26b28-140">В настоящее время поддерживается только группа пользователей.</span><span class="sxs-lookup"><span data-stu-id="26b28-140">Currently, the only target supported is a user group.</span></span>|

## <a name="response"></a><span data-ttu-id="26b28-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b28-141">Response</span></span>

<span data-ttu-id="26b28-142">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="26b28-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="26b28-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="26b28-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26b28-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="26b28-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="26b28-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="26b28-145">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="26b28-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26b28-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/assign-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26b28-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26b28-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/assign-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26b28-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b28-148">Response</span></span>

<span data-ttu-id="26b28-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26b28-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```

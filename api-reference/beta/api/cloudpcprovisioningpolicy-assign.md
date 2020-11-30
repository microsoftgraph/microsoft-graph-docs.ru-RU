---
title: 'Клаудпкпровисионингполици: назначение'
description: Назначьте политику подготовки облачных ПК для группы.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 3e83fa363eeec142c194865da0bb0bef191aae50
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378479"
---
# <a name="cloudpcprovisioningpolicy-assign"></a><span data-ttu-id="eda48-103">Клаудпкпровисионингполици: назначение</span><span class="sxs-lookup"><span data-stu-id="eda48-103">cloudPcProvisioningPolicy: assign</span></span>

<span data-ttu-id="eda48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eda48-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eda48-105">Назначьте [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) группам пользователей.</span><span class="sxs-lookup"><span data-stu-id="eda48-105">Assign [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) to user groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="eda48-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eda48-106">Permissions</span></span>

<span data-ttu-id="eda48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eda48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eda48-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eda48-109">Permission type</span></span>|<span data-ttu-id="eda48-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eda48-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eda48-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eda48-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eda48-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eda48-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="eda48-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eda48-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eda48-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda48-114">Not supported.</span></span>|
|<span data-ttu-id="eda48-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eda48-115">Application</span></span>|<span data-ttu-id="eda48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda48-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eda48-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eda48-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="eda48-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eda48-118">Request headers</span></span>

|<span data-ttu-id="eda48-119">Имя</span><span class="sxs-lookup"><span data-stu-id="eda48-119">Name</span></span>|<span data-ttu-id="eda48-120">Описание</span><span class="sxs-lookup"><span data-stu-id="eda48-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eda48-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eda48-121">Authorization</span></span>|<span data-ttu-id="eda48-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eda48-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eda48-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eda48-124">Content-Type</span></span>|<span data-ttu-id="eda48-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eda48-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eda48-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eda48-127">Request body</span></span>

<span data-ttu-id="eda48-128">В тексте запроса добавьте представление объекта [клаудпкпровисионингполициассигнмент](../resources/cloudpcprovisioningpolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eda48-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object.</span></span>

<span data-ttu-id="eda48-129">В следующей таблице приведены свойства, необходимые при создании [клаудпкпровисионингполициассигнмент](../resources/cloudpcprovisioningpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="eda48-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md).</span></span>

|<span data-ttu-id="eda48-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eda48-130">Property</span></span>|<span data-ttu-id="eda48-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eda48-131">Type</span></span>|<span data-ttu-id="eda48-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eda48-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eda48-133">id</span><span class="sxs-lookup"><span data-stu-id="eda48-133">id</span></span>|<span data-ttu-id="eda48-134">Строка</span><span class="sxs-lookup"><span data-stu-id="eda48-134">String</span></span>|<span data-ttu-id="eda48-135">Идентификатор назначения политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="eda48-135">The ID of the provisioning policy assignment.</span></span> <span data-ttu-id="eda48-136">Если целевой объект — группа пользователей, идентификатор отображается как {Полициид} _ {groupId}.</span><span class="sxs-lookup"><span data-stu-id="eda48-136">If target is a user group, then the ID is shown as {policyId}_{groupId}.</span></span> |
|<span data-ttu-id="eda48-137">target</span><span class="sxs-lookup"><span data-stu-id="eda48-137">target</span></span>|[<span data-ttu-id="eda48-138">клаудпкманажементассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="eda48-138">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="eda48-139">Цель назначения для политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="eda48-139">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="eda48-140">В настоящее время поддерживается только группа пользователей.</span><span class="sxs-lookup"><span data-stu-id="eda48-140">Currently, the only target supported is a user group.</span></span>|

## <a name="response"></a><span data-ttu-id="eda48-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="eda48-141">Response</span></span>

<span data-ttu-id="eda48-142">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eda48-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="eda48-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="eda48-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eda48-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="eda48-144">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="eda48-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="eda48-145">Response</span></span>

<span data-ttu-id="eda48-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eda48-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```

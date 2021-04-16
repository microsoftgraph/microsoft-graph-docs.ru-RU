---
title: Обновление deviceManagementConfigurationPolicyAssignment
description: Обновление свойств объекта deviceManagementConfigurationPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b3bcb7fc747f22fe94996faacd350f30cb7ae6c6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867058"
---
# <a name="update-devicemanagementconfigurationpolicyassignment"></a><span data-ttu-id="e54d4-103">Обновление deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e54d4-103">Update deviceManagementConfigurationPolicyAssignment</span></span>

<span data-ttu-id="e54d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e54d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e54d4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e54d4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e54d4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e54d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e54d4-107">Обновление свойств объекта [deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e54d4-107">Update the properties of a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e54d4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e54d4-108">Prerequisites</span></span>
<span data-ttu-id="e54d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e54d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e54d4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e54d4-111">Permission type</span></span>|<span data-ttu-id="e54d4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e54d4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e54d4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e54d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e54d4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e54d4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e54d4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e54d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e54d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e54d4-116">Not supported.</span></span>|
|<span data-ttu-id="e54d4-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e54d4-117">Application</span></span>|<span data-ttu-id="e54d4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e54d4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e54d4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e54d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments/{deviceManagementConfigurationPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e54d4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e54d4-120">Request headers</span></span>
|<span data-ttu-id="e54d4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e54d4-121">Header</span></span>|<span data-ttu-id="e54d4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e54d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e54d4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e54d4-123">Authorization</span></span>|<span data-ttu-id="e54d4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e54d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e54d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e54d4-125">Accept</span></span>|<span data-ttu-id="e54d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e54d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e54d4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e54d4-127">Request body</span></span>
<span data-ttu-id="e54d4-128">В теле запроса поставляем представление JSON для [объекта deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e54d4-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

<span data-ttu-id="e54d4-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e54d4-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md).</span></span>

|<span data-ttu-id="e54d4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e54d4-130">Property</span></span>|<span data-ttu-id="e54d4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e54d4-131">Type</span></span>|<span data-ttu-id="e54d4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e54d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e54d4-133">id</span><span class="sxs-lookup"><span data-stu-id="e54d4-133">id</span></span>|<span data-ttu-id="e54d4-134">String</span><span class="sxs-lookup"><span data-stu-id="e54d4-134">String</span></span>|<span data-ttu-id="e54d4-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="e54d4-135">The key of the assignment.</span></span>|
|<span data-ttu-id="e54d4-136">target</span><span class="sxs-lookup"><span data-stu-id="e54d4-136">target</span></span>|[<span data-ttu-id="e54d4-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e54d4-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e54d4-138">Цель назначения для DeviceManagementConfigurationPolicy.</span><span class="sxs-lookup"><span data-stu-id="e54d4-138">The assignment target for the DeviceManagementConfigurationPolicy.</span></span>|



## <a name="response"></a><span data-ttu-id="e54d4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e54d4-139">Response</span></span>
<span data-ttu-id="e54d4-140">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e54d4-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e54d4-141">Пример</span><span class="sxs-lookup"><span data-stu-id="e54d4-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="e54d4-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="e54d4-142">Request</span></span>
<span data-ttu-id="e54d4-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e54d4-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments/{deviceManagementConfigurationPolicyAssignmentId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="e54d4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e54d4-144">Response</span></span>
<span data-ttu-id="e54d4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e54d4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "id": "1f069921-9921-1f06-2199-061f2199061f",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```





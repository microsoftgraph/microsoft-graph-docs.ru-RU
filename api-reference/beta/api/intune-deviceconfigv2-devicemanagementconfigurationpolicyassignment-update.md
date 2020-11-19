---
title: Обновление Девицеманажементконфигуратионполициассигнмент
description: Обновление свойств объекта Девицеманажементконфигуратионполициассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 21272050b9bb01730e422290efe3c0b6e494644f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302162"
---
# <a name="update-devicemanagementconfigurationpolicyassignment"></a><span data-ttu-id="4a5ab-103">Обновление Девицеманажементконфигуратионполициассигнмент</span><span class="sxs-lookup"><span data-stu-id="4a5ab-103">Update deviceManagementConfigurationPolicyAssignment</span></span>

<span data-ttu-id="4a5ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a5ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a5ab-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a5ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a5ab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a5ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a5ab-107">Обновление свойств объекта [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4a5ab-107">Update the properties of a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a5ab-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4a5ab-108">Prerequisites</span></span>
<span data-ttu-id="4a5ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a5ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a5ab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a5ab-111">Permission type</span></span>|<span data-ttu-id="4a5ab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a5ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a5ab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a5ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a5ab-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a5ab-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a5ab-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a5ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a5ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a5ab-116">Not supported.</span></span>|
|<span data-ttu-id="4a5ab-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a5ab-117">Application</span></span>|<span data-ttu-id="4a5ab-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a5ab-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a5ab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a5ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments/{deviceManagementConfigurationPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4a5ab-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4a5ab-120">Request headers</span></span>
|<span data-ttu-id="4a5ab-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a5ab-121">Header</span></span>|<span data-ttu-id="4a5ab-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4a5ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a5ab-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a5ab-123">Authorization</span></span>|<span data-ttu-id="4a5ab-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a5ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a5ab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4a5ab-125">Accept</span></span>|<span data-ttu-id="4a5ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a5ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a5ab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a5ab-127">Request body</span></span>
<span data-ttu-id="4a5ab-128">В тексте запроса добавьте представление объекта [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a5ab-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

<span data-ttu-id="4a5ab-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4a5ab-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md).</span></span>

|<span data-ttu-id="4a5ab-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a5ab-130">Property</span></span>|<span data-ttu-id="4a5ab-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4a5ab-131">Type</span></span>|<span data-ttu-id="4a5ab-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4a5ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a5ab-133">id</span><span class="sxs-lookup"><span data-stu-id="4a5ab-133">id</span></span>|<span data-ttu-id="4a5ab-134">String</span><span class="sxs-lookup"><span data-stu-id="4a5ab-134">String</span></span>|<span data-ttu-id="4a5ab-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="4a5ab-135">The key of the assignment.</span></span>|
|<span data-ttu-id="4a5ab-136">target</span><span class="sxs-lookup"><span data-stu-id="4a5ab-136">target</span></span>|[<span data-ttu-id="4a5ab-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4a5ab-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4a5ab-138">Цель назначения для Девицеманажементконфигуратионполици.</span><span class="sxs-lookup"><span data-stu-id="4a5ab-138">The assignment target for the DeviceManagementConfigurationPolicy.</span></span>|



## <a name="response"></a><span data-ttu-id="4a5ab-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a5ab-139">Response</span></span>
<span data-ttu-id="4a5ab-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a5ab-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a5ab-141">Пример</span><span class="sxs-lookup"><span data-stu-id="4a5ab-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a5ab-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a5ab-142">Request</span></span>
<span data-ttu-id="4a5ab-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a5ab-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments/{deviceManagementConfigurationPolicyAssignmentId}
Content-type: application/json
Content-length: 340

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="4a5ab-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a5ab-144">Response</span></span>
<span data-ttu-id="4a5ab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a5ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 389

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "id": "1f069921-9921-1f06-2199-061f2199061f",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```





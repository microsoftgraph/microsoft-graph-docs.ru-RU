---
title: Создание Девицеманажементконфигуратионполициассигнмент
description: Создание нового объекта Девицеманажементконфигуратионполициассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdacc5f360340e6e07de25183ed53ddce181b15e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302178"
---
# <a name="create-devicemanagementconfigurationpolicyassignment"></a><span data-ttu-id="73406-103">Создание Девицеманажементконфигуратионполициассигнмент</span><span class="sxs-lookup"><span data-stu-id="73406-103">Create deviceManagementConfigurationPolicyAssignment</span></span>

<span data-ttu-id="73406-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73406-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73406-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73406-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73406-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73406-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73406-107">Создание нового объекта [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="73406-107">Create a new [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73406-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="73406-108">Prerequisites</span></span>
<span data-ttu-id="73406-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73406-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73406-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73406-111">Permission type</span></span>|<span data-ttu-id="73406-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73406-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73406-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73406-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73406-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73406-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73406-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73406-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73406-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73406-116">Not supported.</span></span>|
|<span data-ttu-id="73406-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73406-117">Application</span></span>|<span data-ttu-id="73406-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73406-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73406-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73406-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="73406-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="73406-120">Request headers</span></span>
|<span data-ttu-id="73406-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73406-121">Header</span></span>|<span data-ttu-id="73406-122">Значение</span><span class="sxs-lookup"><span data-stu-id="73406-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73406-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73406-123">Authorization</span></span>|<span data-ttu-id="73406-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73406-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73406-125">Accept</span><span class="sxs-lookup"><span data-stu-id="73406-125">Accept</span></span>|<span data-ttu-id="73406-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73406-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73406-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73406-127">Request body</span></span>
<span data-ttu-id="73406-128">В тексте запроса добавьте представление объекта Девицеманажементконфигуратионполициассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73406-128">In the request body, supply a JSON representation for the deviceManagementConfigurationPolicyAssignment object.</span></span>

<span data-ttu-id="73406-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементконфигуратионполициассигнмент.</span><span class="sxs-lookup"><span data-stu-id="73406-129">The following table shows the properties that are required when you create the deviceManagementConfigurationPolicyAssignment.</span></span>

|<span data-ttu-id="73406-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="73406-130">Property</span></span>|<span data-ttu-id="73406-131">Тип</span><span class="sxs-lookup"><span data-stu-id="73406-131">Type</span></span>|<span data-ttu-id="73406-132">Описание</span><span class="sxs-lookup"><span data-stu-id="73406-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73406-133">id</span><span class="sxs-lookup"><span data-stu-id="73406-133">id</span></span>|<span data-ttu-id="73406-134">String</span><span class="sxs-lookup"><span data-stu-id="73406-134">String</span></span>|<span data-ttu-id="73406-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="73406-135">The key of the assignment.</span></span>|
|<span data-ttu-id="73406-136">target</span><span class="sxs-lookup"><span data-stu-id="73406-136">target</span></span>|[<span data-ttu-id="73406-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="73406-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="73406-138">Цель назначения для Девицеманажементконфигуратионполици.</span><span class="sxs-lookup"><span data-stu-id="73406-138">The assignment target for the DeviceManagementConfigurationPolicy.</span></span>|



## <a name="response"></a><span data-ttu-id="73406-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="73406-139">Response</span></span>
<span data-ttu-id="73406-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73406-140">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73406-141">Пример</span><span class="sxs-lookup"><span data-stu-id="73406-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="73406-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="73406-142">Request</span></span>
<span data-ttu-id="73406-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73406-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments
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

### <a name="response"></a><span data-ttu-id="73406-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="73406-144">Response</span></span>
<span data-ttu-id="73406-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73406-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





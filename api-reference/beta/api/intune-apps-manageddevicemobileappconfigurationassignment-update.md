---
title: Обновление объекта managedDeviceMobileAppConfigurationAssignment
description: Обновление свойств объекта managedDeviceMobileAppConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0653273bba098e51134f12702d295dc64a9fd23
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815532"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="7d932-103">Обновление объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7d932-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="7d932-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d932-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d932-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d932-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d932-106">Обновление свойств объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7d932-106">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d932-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7d932-107">Prerequisites</span></span>
<span data-ttu-id="7d932-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d932-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d932-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d932-110">Permission type</span></span>|<span data-ttu-id="7d932-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d932-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d932-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d932-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d932-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d932-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d932-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d932-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d932-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d932-115">Not supported.</span></span>|
|<span data-ttu-id="7d932-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7d932-116">Application</span></span>|<span data-ttu-id="7d932-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d932-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d932-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d932-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7d932-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7d932-119">Request headers</span></span>
|<span data-ttu-id="7d932-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d932-120">Header</span></span>|<span data-ttu-id="7d932-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7d932-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d932-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d932-122">Authorization</span></span>|<span data-ttu-id="7d932-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d932-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d932-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7d932-124">Accept</span></span>|<span data-ttu-id="7d932-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d932-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d932-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d932-126">Request body</span></span>
<span data-ttu-id="7d932-127">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d932-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="7d932-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7d932-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="7d932-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d932-129">Property</span></span>|<span data-ttu-id="7d932-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7d932-130">Type</span></span>|<span data-ttu-id="7d932-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7d932-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d932-132">id</span><span class="sxs-lookup"><span data-stu-id="7d932-132">id</span></span>|<span data-ttu-id="7d932-133">String</span><span class="sxs-lookup"><span data-stu-id="7d932-133">String</span></span>|<span data-ttu-id="7d932-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="7d932-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7d932-135">target</span><span class="sxs-lookup"><span data-stu-id="7d932-135">target</span></span>|[<span data-ttu-id="7d932-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7d932-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7d932-137">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="7d932-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="7d932-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d932-138">Response</span></span>
<span data-ttu-id="7d932-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d932-139">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d932-140">Пример</span><span class="sxs-lookup"><span data-stu-id="7d932-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d932-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d932-141">Request</span></span>
<span data-ttu-id="7d932-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d932-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="7d932-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d932-143">Response</span></span>
<span data-ttu-id="7d932-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d932-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





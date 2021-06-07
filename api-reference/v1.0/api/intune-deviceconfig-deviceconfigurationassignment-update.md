---
title: Обновление объекта deviceConfigurationAssignment
description: Обновление свойств объекта deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a74c2fe13a60a1184b8cd36b6e353c59dce88ce6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748378"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="6ce82-103">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6ce82-103">Update deviceConfigurationAssignment</span></span>

<span data-ttu-id="6ce82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ce82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ce82-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ce82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ce82-106">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6ce82-106">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ce82-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6ce82-107">Prerequisites</span></span>
<span data-ttu-id="6ce82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ce82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ce82-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ce82-110">Permission type</span></span>|<span data-ttu-id="6ce82-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ce82-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ce82-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ce82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ce82-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ce82-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ce82-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ce82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ce82-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ce82-115">Not supported.</span></span>|
|<span data-ttu-id="6ce82-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6ce82-116">Application</span></span>|<span data-ttu-id="6ce82-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ce82-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ce82-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ce82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6ce82-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6ce82-119">Request headers</span></span>
|<span data-ttu-id="6ce82-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ce82-120">Header</span></span>|<span data-ttu-id="6ce82-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6ce82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ce82-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ce82-122">Authorization</span></span>|<span data-ttu-id="6ce82-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ce82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ce82-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6ce82-124">Accept</span></span>|<span data-ttu-id="6ce82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6ce82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ce82-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ce82-126">Request body</span></span>
<span data-ttu-id="6ce82-127">В тексте запроса добавьте представление объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ce82-127">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="6ce82-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6ce82-128">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="6ce82-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ce82-129">Property</span></span>|<span data-ttu-id="6ce82-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6ce82-130">Type</span></span>|<span data-ttu-id="6ce82-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6ce82-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ce82-132">id</span><span class="sxs-lookup"><span data-stu-id="6ce82-132">id</span></span>|<span data-ttu-id="6ce82-133">String</span><span class="sxs-lookup"><span data-stu-id="6ce82-133">String</span></span>|<span data-ttu-id="6ce82-134">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="6ce82-134">The key of the assignment.</span></span>|
|<span data-ttu-id="6ce82-135">target</span><span class="sxs-lookup"><span data-stu-id="6ce82-135">target</span></span>|[<span data-ttu-id="6ce82-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6ce82-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6ce82-137">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="6ce82-137">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="6ce82-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ce82-138">Response</span></span>
<span data-ttu-id="6ce82-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ce82-139">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ce82-140">Пример</span><span class="sxs-lookup"><span data-stu-id="6ce82-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ce82-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ce82-141">Request</span></span>
<span data-ttu-id="6ce82-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ce82-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 221

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="6ce82-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ce82-143">Response</span></span>
<span data-ttu-id="6ce82-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ce82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "Collection Id value"
  }
}
```





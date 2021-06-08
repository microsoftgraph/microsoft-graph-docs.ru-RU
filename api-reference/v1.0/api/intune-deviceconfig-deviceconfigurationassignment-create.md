---
title: Создание объекта deviceConfigurationAssignment
description: Создание объекта deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27b95ab53b3ed38f7e87193cad33cc0986b92172
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757103"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="7ca54-103">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7ca54-103">Create deviceConfigurationAssignment</span></span>

<span data-ttu-id="7ca54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ca54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ca54-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ca54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ca54-106">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7ca54-106">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ca54-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7ca54-107">Prerequisites</span></span>
<span data-ttu-id="7ca54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ca54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ca54-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ca54-110">Permission type</span></span>|<span data-ttu-id="7ca54-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ca54-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ca54-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ca54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ca54-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ca54-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ca54-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ca54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ca54-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ca54-115">Not supported.</span></span>|
|<span data-ttu-id="7ca54-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7ca54-116">Application</span></span>|<span data-ttu-id="7ca54-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ca54-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ca54-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ca54-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7ca54-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7ca54-119">Request headers</span></span>
|<span data-ttu-id="7ca54-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ca54-120">Header</span></span>|<span data-ttu-id="7ca54-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7ca54-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ca54-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ca54-122">Authorization</span></span>|<span data-ttu-id="7ca54-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ca54-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ca54-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7ca54-124">Accept</span></span>|<span data-ttu-id="7ca54-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ca54-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ca54-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ca54-126">Request body</span></span>
<span data-ttu-id="7ca54-127">В тексте запроса добавьте представление объекта deviceConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ca54-127">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="7ca54-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="7ca54-128">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="7ca54-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ca54-129">Property</span></span>|<span data-ttu-id="7ca54-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7ca54-130">Type</span></span>|<span data-ttu-id="7ca54-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7ca54-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ca54-132">id</span><span class="sxs-lookup"><span data-stu-id="7ca54-132">id</span></span>|<span data-ttu-id="7ca54-133">String</span><span class="sxs-lookup"><span data-stu-id="7ca54-133">String</span></span>|<span data-ttu-id="7ca54-134">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="7ca54-134">The key of the assignment.</span></span>|
|<span data-ttu-id="7ca54-135">target</span><span class="sxs-lookup"><span data-stu-id="7ca54-135">target</span></span>|[<span data-ttu-id="7ca54-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7ca54-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7ca54-137">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="7ca54-137">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="7ca54-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ca54-138">Response</span></span>
<span data-ttu-id="7ca54-139">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7ca54-139">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ca54-140">Пример</span><span class="sxs-lookup"><span data-stu-id="7ca54-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ca54-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ca54-141">Request</span></span>
<span data-ttu-id="7ca54-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ca54-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
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

### <a name="response"></a><span data-ttu-id="7ca54-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ca54-143">Response</span></span>
<span data-ttu-id="7ca54-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ca54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





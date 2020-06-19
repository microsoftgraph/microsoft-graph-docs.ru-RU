---
title: Создание Иослобапппровисионингконфигуратионассигнмент
description: Создание нового объекта Иослобапппровисионингконфигуратионассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a061f97491ea006d2655ef2caa9e8c6e78f185c0
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793410"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="524e2-103">Создание Иослобапппровисионингконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="524e2-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="524e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="524e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="524e2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="524e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="524e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="524e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="524e2-107">Создание нового объекта [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="524e2-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="524e2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="524e2-108">Prerequisites</span></span>
<span data-ttu-id="524e2-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="524e2-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="524e2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="524e2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="524e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="524e2-111">Permission type</span></span>|<span data-ttu-id="524e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="524e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="524e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="524e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="524e2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="524e2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="524e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="524e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="524e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="524e2-116">Not supported.</span></span>|
|<span data-ttu-id="524e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="524e2-117">Application</span></span>|<span data-ttu-id="524e2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="524e2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="524e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="524e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="524e2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="524e2-120">Request headers</span></span>
|<span data-ttu-id="524e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="524e2-121">Header</span></span>|<span data-ttu-id="524e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="524e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="524e2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="524e2-123">Authorization</span></span>|<span data-ttu-id="524e2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="524e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="524e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="524e2-125">Accept</span></span>|<span data-ttu-id="524e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="524e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="524e2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="524e2-127">Request body</span></span>
<span data-ttu-id="524e2-128">В тексте запроса добавьте представление объекта Иослобапппровисионингконфигуратионассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="524e2-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="524e2-129">В следующей таблице приведены свойства, необходимые при создании Иослобапппровисионингконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="524e2-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="524e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="524e2-130">Property</span></span>|<span data-ttu-id="524e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="524e2-131">Type</span></span>|<span data-ttu-id="524e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="524e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="524e2-133">id</span><span class="sxs-lookup"><span data-stu-id="524e2-133">id</span></span>|<span data-ttu-id="524e2-134">String</span><span class="sxs-lookup"><span data-stu-id="524e2-134">String</span></span>|<span data-ttu-id="524e2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="524e2-135">Key of the entity.</span></span>|
|<span data-ttu-id="524e2-136">target</span><span class="sxs-lookup"><span data-stu-id="524e2-136">target</span></span>|[<span data-ttu-id="524e2-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="524e2-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="524e2-138">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="524e2-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="524e2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="524e2-139">Response</span></span>
<span data-ttu-id="524e2-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="524e2-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="524e2-141">Пример</span><span class="sxs-lookup"><span data-stu-id="524e2-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="524e2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="524e2-142">Request</span></span>
<span data-ttu-id="524e2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="524e2-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
Content-type: application/json
Content-length: 351

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="524e2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="524e2-144">Response</span></span>
<span data-ttu-id="524e2-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="524e2-145">Here is an example of the response.</span></span> <span data-ttu-id="524e2-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="524e2-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="524e2-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="524e2-147">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 400

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




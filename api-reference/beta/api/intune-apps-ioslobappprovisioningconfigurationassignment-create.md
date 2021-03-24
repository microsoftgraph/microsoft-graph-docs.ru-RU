---
title: Создание iosLobAppProvisioningConfigurationAssignment
description: Создайте новый объект iosLobAppProvisioningConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c478bb6c00408f353c63bedc10a5774b1ff6e9c0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144244"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="af7a2-103">Создание iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="af7a2-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="af7a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af7a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af7a2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af7a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af7a2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af7a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af7a2-107">Создайте новый [объект iosLobAppProvisioningConfigurationAssignment.](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="af7a2-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af7a2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="af7a2-108">Prerequisites</span></span>
<span data-ttu-id="af7a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af7a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af7a2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af7a2-111">Permission type</span></span>|<span data-ttu-id="af7a2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af7a2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af7a2-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af7a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af7a2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af7a2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="af7a2-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af7a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af7a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af7a2-116">Not supported.</span></span>|
|<span data-ttu-id="af7a2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="af7a2-117">Application</span></span>|<span data-ttu-id="af7a2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af7a2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af7a2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af7a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="af7a2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="af7a2-120">Request headers</span></span>
|<span data-ttu-id="af7a2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af7a2-121">Header</span></span>|<span data-ttu-id="af7a2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af7a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af7a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af7a2-123">Authorization</span></span>|<span data-ttu-id="af7a2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af7a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af7a2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af7a2-125">Accept</span></span>|<span data-ttu-id="af7a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af7a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af7a2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af7a2-127">Request body</span></span>
<span data-ttu-id="af7a2-128">В теле запроса поставляем представление JSON для объекта iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="af7a2-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="af7a2-129">В следующей таблице показаны свойства, необходимые при создании iosLobAppProvisioningConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="af7a2-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="af7a2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="af7a2-130">Property</span></span>|<span data-ttu-id="af7a2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="af7a2-131">Type</span></span>|<span data-ttu-id="af7a2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="af7a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af7a2-133">id</span><span class="sxs-lookup"><span data-stu-id="af7a2-133">id</span></span>|<span data-ttu-id="af7a2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="af7a2-134">String</span></span>|<span data-ttu-id="af7a2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="af7a2-135">Key of the entity.</span></span>|
|<span data-ttu-id="af7a2-136">target</span><span class="sxs-lookup"><span data-stu-id="af7a2-136">target</span></span>|[<span data-ttu-id="af7a2-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="af7a2-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="af7a2-138">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="af7a2-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="af7a2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="af7a2-139">Response</span></span>
<span data-ttu-id="af7a2-140">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="af7a2-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af7a2-141">Пример</span><span class="sxs-lookup"><span data-stu-id="af7a2-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="af7a2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="af7a2-142">Request</span></span>
<span data-ttu-id="af7a2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af7a2-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="af7a2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="af7a2-144">Response</span></span>
<span data-ttu-id="af7a2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af7a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





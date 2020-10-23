---
title: Создание Иослобапппровисионингконфигуратионассигнмент
description: Создание нового объекта Иослобапппровисионингконфигуратионассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03e31d3a84dc175935cf9cfcffb757dc056ca898
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700355"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="588db-103">Создание Иослобапппровисионингконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="588db-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="588db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="588db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="588db-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="588db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="588db-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="588db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="588db-107">Создание нового объекта [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="588db-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="588db-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="588db-108">Prerequisites</span></span>
<span data-ttu-id="588db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="588db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="588db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="588db-111">Permission type</span></span>|<span data-ttu-id="588db-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="588db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="588db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="588db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="588db-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="588db-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="588db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="588db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="588db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="588db-116">Not supported.</span></span>|
|<span data-ttu-id="588db-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="588db-117">Application</span></span>|<span data-ttu-id="588db-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="588db-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="588db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="588db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="588db-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="588db-120">Request headers</span></span>
|<span data-ttu-id="588db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="588db-121">Header</span></span>|<span data-ttu-id="588db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="588db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="588db-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="588db-123">Authorization</span></span>|<span data-ttu-id="588db-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="588db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="588db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="588db-125">Accept</span></span>|<span data-ttu-id="588db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="588db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="588db-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="588db-127">Request body</span></span>
<span data-ttu-id="588db-128">В тексте запроса добавьте представление объекта Иослобапппровисионингконфигуратионассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="588db-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="588db-129">В следующей таблице приведены свойства, необходимые при создании Иослобапппровисионингконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="588db-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="588db-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="588db-130">Property</span></span>|<span data-ttu-id="588db-131">Тип</span><span class="sxs-lookup"><span data-stu-id="588db-131">Type</span></span>|<span data-ttu-id="588db-132">Описание</span><span class="sxs-lookup"><span data-stu-id="588db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="588db-133">id</span><span class="sxs-lookup"><span data-stu-id="588db-133">id</span></span>|<span data-ttu-id="588db-134">Строка</span><span class="sxs-lookup"><span data-stu-id="588db-134">String</span></span>|<span data-ttu-id="588db-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="588db-135">Key of the entity.</span></span>|
|<span data-ttu-id="588db-136">target</span><span class="sxs-lookup"><span data-stu-id="588db-136">target</span></span>|[<span data-ttu-id="588db-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="588db-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="588db-138">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="588db-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="588db-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="588db-139">Response</span></span>
<span data-ttu-id="588db-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="588db-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="588db-141">Пример</span><span class="sxs-lookup"><span data-stu-id="588db-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="588db-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="588db-142">Request</span></span>
<span data-ttu-id="588db-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="588db-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="588db-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="588db-144">Response</span></span>
<span data-ttu-id="588db-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="588db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






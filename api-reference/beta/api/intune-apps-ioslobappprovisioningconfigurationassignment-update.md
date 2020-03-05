---
title: Обновление Иослобапппровисионингконфигуратионассигнмент
description: Обновление свойств объекта Иослобапппровисионингконфигуратионассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 184757ab9eb3b98d5e4b24bdf31baf293fd47f15
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445696"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="21bb9-103">Обновление Иослобапппровисионингконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="21bb9-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="21bb9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="21bb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21bb9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21bb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21bb9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21bb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21bb9-107">Обновление свойств объекта [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="21bb9-107">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21bb9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="21bb9-108">Prerequisites</span></span>
<span data-ttu-id="21bb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21bb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21bb9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21bb9-111">Permission type</span></span>|<span data-ttu-id="21bb9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21bb9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21bb9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21bb9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21bb9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21bb9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="21bb9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21bb9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21bb9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21bb9-116">Not supported.</span></span>|
|<span data-ttu-id="21bb9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21bb9-117">Application</span></span>|<span data-ttu-id="21bb9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21bb9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21bb9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21bb9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="21bb9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="21bb9-120">Request headers</span></span>
|<span data-ttu-id="21bb9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21bb9-121">Header</span></span>|<span data-ttu-id="21bb9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="21bb9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21bb9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21bb9-123">Authorization</span></span>|<span data-ttu-id="21bb9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21bb9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21bb9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21bb9-125">Accept</span></span>|<span data-ttu-id="21bb9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21bb9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21bb9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21bb9-127">Request body</span></span>
<span data-ttu-id="21bb9-128">В тексте запроса добавьте представление объекта [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21bb9-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="21bb9-129">В следующей таблице приведены свойства, необходимые при создании [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21bb9-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="21bb9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="21bb9-130">Property</span></span>|<span data-ttu-id="21bb9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="21bb9-131">Type</span></span>|<span data-ttu-id="21bb9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="21bb9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21bb9-133">id</span><span class="sxs-lookup"><span data-stu-id="21bb9-133">id</span></span>|<span data-ttu-id="21bb9-134">String</span><span class="sxs-lookup"><span data-stu-id="21bb9-134">String</span></span>|<span data-ttu-id="21bb9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="21bb9-135">Key of the entity.</span></span>|
|<span data-ttu-id="21bb9-136">target</span><span class="sxs-lookup"><span data-stu-id="21bb9-136">target</span></span>|[<span data-ttu-id="21bb9-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="21bb9-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="21bb9-138">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="21bb9-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="21bb9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="21bb9-139">Response</span></span>
<span data-ttu-id="21bb9-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="21bb9-140">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21bb9-141">Пример</span><span class="sxs-lookup"><span data-stu-id="21bb9-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="21bb9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="21bb9-142">Request</span></span>
<span data-ttu-id="21bb9-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21bb9-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="21bb9-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="21bb9-144">Response</span></span>
<span data-ttu-id="21bb9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21bb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```






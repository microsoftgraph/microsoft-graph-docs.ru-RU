---
title: Создание Иослобапппровисионингконфигуратионассигнмент
description: Создание нового объекта Иослобапппровисионингконфигуратионассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9d2af6426c1449e1680bfa0b789972d372584af0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445717"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="e5fe7-103">Создание Иослобапппровисионингконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="e5fe7-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="e5fe7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e5fe7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5fe7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5fe7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5fe7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5fe7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5fe7-107">Создание нового объекта [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e5fe7-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5fe7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5fe7-108">Prerequisites</span></span>
<span data-ttu-id="e5fe7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5fe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5fe7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5fe7-111">Permission type</span></span>|<span data-ttu-id="e5fe7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5fe7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5fe7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5fe7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5fe7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5fe7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5fe7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5fe7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5fe7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5fe7-116">Not supported.</span></span>|
|<span data-ttu-id="e5fe7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5fe7-117">Application</span></span>|<span data-ttu-id="e5fe7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5fe7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5fe7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5fe7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e5fe7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e5fe7-120">Request headers</span></span>
|<span data-ttu-id="e5fe7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5fe7-121">Header</span></span>|<span data-ttu-id="e5fe7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5fe7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5fe7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5fe7-123">Authorization</span></span>|<span data-ttu-id="e5fe7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5fe7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5fe7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5fe7-125">Accept</span></span>|<span data-ttu-id="e5fe7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5fe7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5fe7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5fe7-127">Request body</span></span>
<span data-ttu-id="e5fe7-128">В тексте запроса добавьте представление объекта Иослобапппровисионингконфигуратионассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5fe7-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="e5fe7-129">В следующей таблице приведены свойства, необходимые при создании Иослобапппровисионингконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="e5fe7-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="e5fe7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5fe7-130">Property</span></span>|<span data-ttu-id="e5fe7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e5fe7-131">Type</span></span>|<span data-ttu-id="e5fe7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e5fe7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5fe7-133">id</span><span class="sxs-lookup"><span data-stu-id="e5fe7-133">id</span></span>|<span data-ttu-id="e5fe7-134">String</span><span class="sxs-lookup"><span data-stu-id="e5fe7-134">String</span></span>|<span data-ttu-id="e5fe7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e5fe7-135">Key of the entity.</span></span>|
|<span data-ttu-id="e5fe7-136">target</span><span class="sxs-lookup"><span data-stu-id="e5fe7-136">target</span></span>|[<span data-ttu-id="e5fe7-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e5fe7-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e5fe7-138">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="e5fe7-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="e5fe7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5fe7-139">Response</span></span>
<span data-ttu-id="e5fe7-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5fe7-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5fe7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="e5fe7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5fe7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5fe7-142">Request</span></span>
<span data-ttu-id="e5fe7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5fe7-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e5fe7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5fe7-144">Response</span></span>
<span data-ttu-id="e5fe7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5fe7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






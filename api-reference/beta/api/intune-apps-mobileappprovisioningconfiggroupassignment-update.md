---
title: Обновление К mobileappprovisioningconfiggroupassignment.
description: Обновление свойств объекта К mobileappprovisioningconfiggroupassignment..
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d3917e60e7e895921c2eed735bf718461b44abb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39934884"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="03240-103">Обновление К mobileappprovisioningconfiggroupassignment.</span><span class="sxs-lookup"><span data-stu-id="03240-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="03240-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03240-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03240-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03240-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03240-106">Обновление свойств объекта [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="03240-106">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03240-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03240-107">Prerequisites</span></span>
<span data-ttu-id="03240-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03240-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03240-110">Permission type</span></span>|<span data-ttu-id="03240-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03240-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03240-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03240-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03240-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03240-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="03240-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03240-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03240-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03240-115">Not supported.</span></span>|
|<span data-ttu-id="03240-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03240-116">Application</span></span>|<span data-ttu-id="03240-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03240-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03240-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03240-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="03240-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03240-119">Request headers</span></span>
|<span data-ttu-id="03240-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03240-120">Header</span></span>|<span data-ttu-id="03240-121">Значение</span><span class="sxs-lookup"><span data-stu-id="03240-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03240-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03240-122">Authorization</span></span>|<span data-ttu-id="03240-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03240-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03240-124">Accept</span><span class="sxs-lookup"><span data-stu-id="03240-124">Accept</span></span>|<span data-ttu-id="03240-125">application/json</span><span class="sxs-lookup"><span data-stu-id="03240-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03240-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03240-126">Request body</span></span>
<span data-ttu-id="03240-127">В тексте запроса добавьте представление объекта [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03240-127">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="03240-128">В следующей таблице приведены свойства, необходимые при создании [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="03240-128">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="03240-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="03240-129">Property</span></span>|<span data-ttu-id="03240-130">Тип</span><span class="sxs-lookup"><span data-stu-id="03240-130">Type</span></span>|<span data-ttu-id="03240-131">Описание</span><span class="sxs-lookup"><span data-stu-id="03240-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03240-132">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="03240-132">targetGroupId</span></span>|<span data-ttu-id="03240-133">Строка</span><span class="sxs-lookup"><span data-stu-id="03240-133">String</span></span>|<span data-ttu-id="03240-134">Идентификатор группы AAD, в которой нацелена конфигурация подготовки приложений.</span><span class="sxs-lookup"><span data-stu-id="03240-134">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="03240-135">id</span><span class="sxs-lookup"><span data-stu-id="03240-135">id</span></span>|<span data-ttu-id="03240-136">Строка</span><span class="sxs-lookup"><span data-stu-id="03240-136">String</span></span>|<span data-ttu-id="03240-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="03240-137">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="03240-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="03240-138">Response</span></span>
<span data-ttu-id="03240-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03240-139">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03240-140">Пример</span><span class="sxs-lookup"><span data-stu-id="03240-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="03240-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="03240-141">Request</span></span>
<span data-ttu-id="03240-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03240-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="03240-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="03240-143">Response</span></span>
<span data-ttu-id="03240-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03240-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```






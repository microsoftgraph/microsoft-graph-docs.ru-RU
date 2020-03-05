---
title: Создание объекта managedDeviceMobileAppConfigurationAssignment
description: Создание объекта managedDeviceMobileAppConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95e75f8c3f4d06a77e4807995727e1624cdf468e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451023"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="0ca8e-103">Создание объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0ca8e-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

<span data-ttu-id="0ca8e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0ca8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ca8e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ca8e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ca8e-107">Создание объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0ca8e-107">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ca8e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0ca8e-108">Prerequisites</span></span>
<span data-ttu-id="0ca8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ca8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ca8e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ca8e-111">Permission type</span></span>|<span data-ttu-id="0ca8e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ca8e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ca8e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ca8e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ca8e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ca8e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0ca8e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ca8e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ca8e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-116">Not supported.</span></span>|
|<span data-ttu-id="0ca8e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ca8e-117">Application</span></span>|<span data-ttu-id="0ca8e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ca8e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ca8e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ca8e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0ca8e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0ca8e-120">Request headers</span></span>
|<span data-ttu-id="0ca8e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ca8e-121">Header</span></span>|<span data-ttu-id="0ca8e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0ca8e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ca8e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ca8e-123">Authorization</span></span>|<span data-ttu-id="0ca8e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ca8e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ca8e-125">Accept</span></span>|<span data-ttu-id="0ca8e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ca8e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ca8e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ca8e-127">Request body</span></span>
<span data-ttu-id="0ca8e-128">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="0ca8e-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="0ca8e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ca8e-130">Property</span></span>|<span data-ttu-id="0ca8e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0ca8e-131">Type</span></span>|<span data-ttu-id="0ca8e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0ca8e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ca8e-133">id</span><span class="sxs-lookup"><span data-stu-id="0ca8e-133">id</span></span>|<span data-ttu-id="0ca8e-134">String</span><span class="sxs-lookup"><span data-stu-id="0ca8e-134">String</span></span>|<span data-ttu-id="0ca8e-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="0ca8e-136">target</span><span class="sxs-lookup"><span data-stu-id="0ca8e-136">target</span></span>|[<span data-ttu-id="0ca8e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0ca8e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0ca8e-138">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="0ca8e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ca8e-139">Response</span></span>
<span data-ttu-id="0ca8e-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-140">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ca8e-141">Пример</span><span class="sxs-lookup"><span data-stu-id="0ca8e-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ca8e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ca8e-142">Request</span></span>
<span data-ttu-id="0ca8e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="0ca8e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ca8e-144">Response</span></span>
<span data-ttu-id="0ca8e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






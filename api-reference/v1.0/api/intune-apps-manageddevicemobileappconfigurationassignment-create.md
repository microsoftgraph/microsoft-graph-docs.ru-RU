---
title: Создание объекта managedDeviceMobileAppConfigurationAssignment
description: Создание объекта managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc6286af6fe2c05fad3752fc626dd3e279058179
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754261"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="37e8b-103">Создание объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="37e8b-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

<span data-ttu-id="37e8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37e8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37e8b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37e8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37e8b-106">Создание объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="37e8b-106">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37e8b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="37e8b-107">Prerequisites</span></span>
<span data-ttu-id="37e8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37e8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37e8b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37e8b-110">Permission type</span></span>|<span data-ttu-id="37e8b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37e8b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37e8b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37e8b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37e8b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37e8b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="37e8b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37e8b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37e8b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37e8b-115">Not supported.</span></span>|
|<span data-ttu-id="37e8b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="37e8b-116">Application</span></span>|<span data-ttu-id="37e8b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37e8b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37e8b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37e8b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="37e8b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="37e8b-119">Request headers</span></span>
|<span data-ttu-id="37e8b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37e8b-120">Header</span></span>|<span data-ttu-id="37e8b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="37e8b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37e8b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="37e8b-122">Authorization</span></span>|<span data-ttu-id="37e8b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37e8b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37e8b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="37e8b-124">Accept</span></span>|<span data-ttu-id="37e8b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37e8b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37e8b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37e8b-126">Request body</span></span>
<span data-ttu-id="37e8b-127">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37e8b-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="37e8b-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="37e8b-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="37e8b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="37e8b-129">Property</span></span>|<span data-ttu-id="37e8b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="37e8b-130">Type</span></span>|<span data-ttu-id="37e8b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="37e8b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37e8b-132">id</span><span class="sxs-lookup"><span data-stu-id="37e8b-132">id</span></span>|<span data-ttu-id="37e8b-133">String</span><span class="sxs-lookup"><span data-stu-id="37e8b-133">String</span></span>|<span data-ttu-id="37e8b-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="37e8b-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="37e8b-135">target</span><span class="sxs-lookup"><span data-stu-id="37e8b-135">target</span></span>|[<span data-ttu-id="37e8b-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="37e8b-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="37e8b-137">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="37e8b-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="37e8b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="37e8b-138">Response</span></span>
<span data-ttu-id="37e8b-139">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37e8b-139">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37e8b-140">Пример</span><span class="sxs-lookup"><span data-stu-id="37e8b-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="37e8b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="37e8b-141">Request</span></span>
<span data-ttu-id="37e8b-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37e8b-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="37e8b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="37e8b-143">Response</span></span>
<span data-ttu-id="37e8b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37e8b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  }
}
```





---
title: Обновление объекта managedDeviceMobileAppConfigurationAssignment
description: Обновление свойств объекта managedDeviceMobileAppConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 794570f4e820e1de54a85a9684da6bdcb630311b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358615"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="24879-103">Обновление объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="24879-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="24879-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24879-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24879-105">Обновление свойств объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="24879-105">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24879-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="24879-106">Prerequisites</span></span>
<span data-ttu-id="24879-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24879-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24879-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24879-109">Permission type</span></span>|<span data-ttu-id="24879-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24879-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24879-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24879-111">Delegated (work or school account)</span></span>|<span data-ttu-id="24879-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24879-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="24879-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24879-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24879-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24879-114">Not supported.</span></span>|
|<span data-ttu-id="24879-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24879-115">Application</span></span>|<span data-ttu-id="24879-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24879-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24879-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24879-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="24879-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24879-118">Request headers</span></span>
|<span data-ttu-id="24879-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24879-119">Header</span></span>|<span data-ttu-id="24879-120">Значение</span><span class="sxs-lookup"><span data-stu-id="24879-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24879-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24879-121">Authorization</span></span>|<span data-ttu-id="24879-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24879-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24879-123">Accept</span><span class="sxs-lookup"><span data-stu-id="24879-123">Accept</span></span>|<span data-ttu-id="24879-124">application/json</span><span class="sxs-lookup"><span data-stu-id="24879-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24879-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24879-125">Request body</span></span>
<span data-ttu-id="24879-126">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24879-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="24879-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="24879-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="24879-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="24879-128">Property</span></span>|<span data-ttu-id="24879-129">Тип</span><span class="sxs-lookup"><span data-stu-id="24879-129">Type</span></span>|<span data-ttu-id="24879-130">Описание</span><span class="sxs-lookup"><span data-stu-id="24879-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24879-131">id</span><span class="sxs-lookup"><span data-stu-id="24879-131">id</span></span>|<span data-ttu-id="24879-132">String</span><span class="sxs-lookup"><span data-stu-id="24879-132">String</span></span>|<span data-ttu-id="24879-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="24879-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="24879-134">target</span><span class="sxs-lookup"><span data-stu-id="24879-134">target</span></span>|[<span data-ttu-id="24879-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="24879-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="24879-136">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="24879-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="24879-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="24879-137">Response</span></span>
<span data-ttu-id="24879-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24879-138">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24879-139">Пример</span><span class="sxs-lookup"><span data-stu-id="24879-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="24879-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="24879-140">Request</span></span>
<span data-ttu-id="24879-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24879-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="24879-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="24879-142">Response</span></span>
<span data-ttu-id="24879-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24879-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





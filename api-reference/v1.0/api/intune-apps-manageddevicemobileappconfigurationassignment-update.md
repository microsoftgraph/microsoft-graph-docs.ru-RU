---
title: Обновление объекта managedDeviceMobileAppConfigurationAssignment
description: Обновление свойств объекта managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dccf48cfefb0e5a9f09fd51e998a1172280f72d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578283"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="46839-103">Обновление объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="46839-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="46839-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46839-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46839-105">Обновление свойств объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="46839-105">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46839-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="46839-106">Prerequisites</span></span>
<span data-ttu-id="46839-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46839-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46839-109">Permission type</span></span>|<span data-ttu-id="46839-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46839-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46839-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46839-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46839-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46839-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46839-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46839-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46839-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46839-114">Not supported.</span></span>|
|<span data-ttu-id="46839-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46839-115">Application</span></span>|<span data-ttu-id="46839-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46839-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46839-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46839-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="46839-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46839-118">Request headers</span></span>
|<span data-ttu-id="46839-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46839-119">Header</span></span>|<span data-ttu-id="46839-120">Значение</span><span class="sxs-lookup"><span data-stu-id="46839-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46839-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46839-121">Authorization</span></span>|<span data-ttu-id="46839-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46839-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46839-123">Accept</span><span class="sxs-lookup"><span data-stu-id="46839-123">Accept</span></span>|<span data-ttu-id="46839-124">application/json</span><span class="sxs-lookup"><span data-stu-id="46839-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46839-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46839-125">Request body</span></span>
<span data-ttu-id="46839-126">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46839-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="46839-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="46839-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="46839-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="46839-128">Property</span></span>|<span data-ttu-id="46839-129">Тип</span><span class="sxs-lookup"><span data-stu-id="46839-129">Type</span></span>|<span data-ttu-id="46839-130">Описание</span><span class="sxs-lookup"><span data-stu-id="46839-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46839-131">id</span><span class="sxs-lookup"><span data-stu-id="46839-131">id</span></span>|<span data-ttu-id="46839-132">String</span><span class="sxs-lookup"><span data-stu-id="46839-132">String</span></span>|<span data-ttu-id="46839-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="46839-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="46839-134">target</span><span class="sxs-lookup"><span data-stu-id="46839-134">target</span></span>|[<span data-ttu-id="46839-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="46839-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="46839-136">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="46839-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="46839-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="46839-137">Response</span></span>
<span data-ttu-id="46839-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46839-138">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46839-139">Пример</span><span class="sxs-lookup"><span data-stu-id="46839-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="46839-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="46839-140">Request</span></span>
<span data-ttu-id="46839-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46839-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="46839-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="46839-142">Response</span></span>
<span data-ttu-id="46839-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46839-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




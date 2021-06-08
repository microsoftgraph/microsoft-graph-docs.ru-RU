---
title: Обновление объекта mobileAppAssignment
description: Обновление свойств объекта mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cdc8e0145a782cc9a5eb87756542e8a7c5efcfb7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759730"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="28ac9-103">Обновление объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="28ac9-103">Update mobileAppAssignment</span></span>

<span data-ttu-id="28ac9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28ac9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28ac9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28ac9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28ac9-106">Обновление свойств объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="28ac9-106">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28ac9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="28ac9-107">Prerequisites</span></span>
<span data-ttu-id="28ac9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28ac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28ac9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28ac9-110">Permission type</span></span>|<span data-ttu-id="28ac9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28ac9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28ac9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28ac9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28ac9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28ac9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="28ac9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28ac9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28ac9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28ac9-115">Not supported.</span></span>|
|<span data-ttu-id="28ac9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="28ac9-116">Application</span></span>|<span data-ttu-id="28ac9-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28ac9-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28ac9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28ac9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="28ac9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="28ac9-119">Request headers</span></span>
|<span data-ttu-id="28ac9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28ac9-120">Header</span></span>|<span data-ttu-id="28ac9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="28ac9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28ac9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28ac9-122">Authorization</span></span>|<span data-ttu-id="28ac9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28ac9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28ac9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="28ac9-124">Accept</span></span>|<span data-ttu-id="28ac9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28ac9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28ac9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28ac9-126">Request body</span></span>
<span data-ttu-id="28ac9-127">В тексте запроса добавьте представление объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28ac9-127">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="28ac9-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="28ac9-128">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="28ac9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="28ac9-129">Property</span></span>|<span data-ttu-id="28ac9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="28ac9-130">Type</span></span>|<span data-ttu-id="28ac9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="28ac9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28ac9-132">id</span><span class="sxs-lookup"><span data-stu-id="28ac9-132">id</span></span>|<span data-ttu-id="28ac9-133">String</span><span class="sxs-lookup"><span data-stu-id="28ac9-133">String</span></span>|<span data-ttu-id="28ac9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="28ac9-134">Key of the entity.</span></span>|
|<span data-ttu-id="28ac9-135">intent</span><span class="sxs-lookup"><span data-stu-id="28ac9-135">intent</span></span>|[<span data-ttu-id="28ac9-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="28ac9-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="28ac9-137">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="28ac9-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="28ac9-138">target</span><span class="sxs-lookup"><span data-stu-id="28ac9-138">target</span></span>|[<span data-ttu-id="28ac9-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="28ac9-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="28ac9-140">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="28ac9-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="28ac9-141">settings</span><span class="sxs-lookup"><span data-stu-id="28ac9-141">settings</span></span>|[<span data-ttu-id="28ac9-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="28ac9-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="28ac9-143">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="28ac9-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="28ac9-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="28ac9-144">Response</span></span>
<span data-ttu-id="28ac9-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28ac9-145">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28ac9-146">Пример</span><span class="sxs-lookup"><span data-stu-id="28ac9-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="28ac9-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="28ac9-147">Request</span></span>
<span data-ttu-id="28ac9-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28ac9-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 324

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="28ac9-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="28ac9-149">Response</span></span>
<span data-ttu-id="28ac9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28ac9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 373

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value"
  }
}
```





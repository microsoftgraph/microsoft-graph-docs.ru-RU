---
title: Обновление Виндовсупдатестате
description: Обновление свойств объекта Виндовсупдатестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27b486f909e7bfcd11c4d354d5a60160e79024bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966949"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="88a54-103">Обновление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="88a54-103">Update windowsUpdateState</span></span>

<span data-ttu-id="88a54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88a54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88a54-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88a54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88a54-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88a54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88a54-107">Обновление свойств объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="88a54-107">Update the properties of a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88a54-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="88a54-108">Prerequisites</span></span>
<span data-ttu-id="88a54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88a54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88a54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88a54-111">Permission type</span></span>|<span data-ttu-id="88a54-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88a54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88a54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88a54-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="88a54-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="88a54-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="88a54-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a54-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="88a54-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="88a54-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="88a54-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a54-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88a54-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88a54-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88a54-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88a54-119">Not supported.</span></span>|
|<span data-ttu-id="88a54-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88a54-120">Application</span></span>||
| <span data-ttu-id="88a54-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="88a54-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="88a54-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a54-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="88a54-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="88a54-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="88a54-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a54-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88a54-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88a54-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="88a54-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="88a54-126">Request headers</span></span>
|<span data-ttu-id="88a54-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88a54-127">Header</span></span>|<span data-ttu-id="88a54-128">Значение</span><span class="sxs-lookup"><span data-stu-id="88a54-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88a54-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="88a54-129">Authorization</span></span>|<span data-ttu-id="88a54-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88a54-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88a54-131">Accept</span><span class="sxs-lookup"><span data-stu-id="88a54-131">Accept</span></span>|<span data-ttu-id="88a54-132">application/json</span><span class="sxs-lookup"><span data-stu-id="88a54-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88a54-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="88a54-133">Request body</span></span>
<span data-ttu-id="88a54-134">В тексте запроса добавьте представление объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88a54-134">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="88a54-135">В следующей таблице приведены свойства, необходимые при создании [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="88a54-135">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

|<span data-ttu-id="88a54-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="88a54-136">Property</span></span>|<span data-ttu-id="88a54-137">Тип</span><span class="sxs-lookup"><span data-stu-id="88a54-137">Type</span></span>|<span data-ttu-id="88a54-138">Описание</span><span class="sxs-lookup"><span data-stu-id="88a54-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88a54-139">id</span><span class="sxs-lookup"><span data-stu-id="88a54-139">id</span></span>|<span data-ttu-id="88a54-140">String</span><span class="sxs-lookup"><span data-stu-id="88a54-140">String</span></span>|<span data-ttu-id="88a54-141">Это идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="88a54-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="88a54-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="88a54-142">deviceId</span></span>|<span data-ttu-id="88a54-143">String</span><span class="sxs-lookup"><span data-stu-id="88a54-143">String</span></span>|<span data-ttu-id="88a54-144">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="88a54-144">The id of the device.</span></span>|
|<span data-ttu-id="88a54-145">userId</span><span class="sxs-lookup"><span data-stu-id="88a54-145">userId</span></span>|<span data-ttu-id="88a54-146">String</span><span class="sxs-lookup"><span data-stu-id="88a54-146">String</span></span>|<span data-ttu-id="88a54-147">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="88a54-147">The id of the user.</span></span>|
|<span data-ttu-id="88a54-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="88a54-148">deviceDisplayName</span></span>|<span data-ttu-id="88a54-149">String</span><span class="sxs-lookup"><span data-stu-id="88a54-149">String</span></span>|<span data-ttu-id="88a54-150">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="88a54-150">Device display name.</span></span>|
|<span data-ttu-id="88a54-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="88a54-151">userPrincipalName</span></span>|<span data-ttu-id="88a54-152">String</span><span class="sxs-lookup"><span data-stu-id="88a54-152">String</span></span>|<span data-ttu-id="88a54-153">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="88a54-153">User principal name.</span></span>|
|<span data-ttu-id="88a54-154">status</span><span class="sxs-lookup"><span data-stu-id="88a54-154">status</span></span>|[<span data-ttu-id="88a54-155">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="88a54-155">windowsUpdateStatus</span></span>](../resources/intune-shared-windowsupdatestatus.md)|<span data-ttu-id="88a54-156">Состояние Windows удпате.</span><span class="sxs-lookup"><span data-stu-id="88a54-156">Windows udpate status.</span></span> <span data-ttu-id="88a54-157">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="88a54-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="88a54-158">куалитюпдатеверсион</span><span class="sxs-lookup"><span data-stu-id="88a54-158">qualityUpdateVersion</span></span>|<span data-ttu-id="88a54-159">String</span><span class="sxs-lookup"><span data-stu-id="88a54-159">String</span></span>|<span data-ttu-id="88a54-160">Версия устройства для обновления качества.</span><span class="sxs-lookup"><span data-stu-id="88a54-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="88a54-161">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="88a54-161">featureUpdateVersion</span></span>|<span data-ttu-id="88a54-162">String</span><span class="sxs-lookup"><span data-stu-id="88a54-162">String</span></span>|<span data-ttu-id="88a54-163">Текущая версия обновления компонентов устройства.</span><span class="sxs-lookup"><span data-stu-id="88a54-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="88a54-164">ластскандатетиме</span><span class="sxs-lookup"><span data-stu-id="88a54-164">lastScanDateTime</span></span>|<span data-ttu-id="88a54-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88a54-165">DateTimeOffset</span></span>|<span data-ttu-id="88a54-166">Дата и время, когда агент обновления Windows успешно выполнил сканирование.</span><span class="sxs-lookup"><span data-stu-id="88a54-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="88a54-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="88a54-167">lastSyncDateTime</span></span>|<span data-ttu-id="88a54-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88a54-168">DateTimeOffset</span></span>|<span data-ttu-id="88a54-169">Дата и время последней синхронизации устройства с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="88a54-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="88a54-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="88a54-170">Response</span></span>
<span data-ttu-id="88a54-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88a54-171">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88a54-172">Пример</span><span class="sxs-lookup"><span data-stu-id="88a54-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="88a54-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="88a54-173">Request</span></span>
<span data-ttu-id="88a54-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88a54-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
Content-type: application/json
Content-length: 504

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a><span data-ttu-id="88a54-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="88a54-175">Response</span></span>
<span data-ttu-id="88a54-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88a54-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "3d92af00-af00-3d92-00af-923d00af923d",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```










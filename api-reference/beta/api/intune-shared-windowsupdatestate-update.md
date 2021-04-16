---
title: Обновление windowsUpdateState
description: Обновление свойств объекта WindowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eb09a2b39c5810385b51b25c00909ca6aa800f25
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866951"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="01634-103">Обновление windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="01634-103">Update windowsUpdateState</span></span>

<span data-ttu-id="01634-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01634-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01634-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01634-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01634-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01634-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01634-107">Обновление свойств объекта [WindowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)</span><span class="sxs-lookup"><span data-stu-id="01634-107">Update the properties of a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01634-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01634-108">Prerequisites</span></span>
<span data-ttu-id="01634-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01634-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01634-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01634-111">Permission type</span></span>|<span data-ttu-id="01634-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01634-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01634-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01634-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="01634-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="01634-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="01634-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01634-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="01634-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="01634-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="01634-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01634-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01634-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01634-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01634-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01634-119">Not supported.</span></span>|
|<span data-ttu-id="01634-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="01634-120">Application</span></span>||
| <span data-ttu-id="01634-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="01634-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="01634-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01634-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="01634-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="01634-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="01634-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01634-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01634-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01634-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="01634-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="01634-126">Request headers</span></span>
|<span data-ttu-id="01634-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01634-127">Header</span></span>|<span data-ttu-id="01634-128">Значение</span><span class="sxs-lookup"><span data-stu-id="01634-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01634-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01634-129">Authorization</span></span>|<span data-ttu-id="01634-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01634-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01634-131">Accept</span><span class="sxs-lookup"><span data-stu-id="01634-131">Accept</span></span>|<span data-ttu-id="01634-132">application/json</span><span class="sxs-lookup"><span data-stu-id="01634-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01634-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01634-133">Request body</span></span>
<span data-ttu-id="01634-134">В теле запроса укажи представление JSON для [объекта WindowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)</span><span class="sxs-lookup"><span data-stu-id="01634-134">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="01634-135">В следующей таблице показаны свойства, необходимые при создании [windowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)</span><span class="sxs-lookup"><span data-stu-id="01634-135">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

|<span data-ttu-id="01634-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="01634-136">Property</span></span>|<span data-ttu-id="01634-137">Тип</span><span class="sxs-lookup"><span data-stu-id="01634-137">Type</span></span>|<span data-ttu-id="01634-138">Описание</span><span class="sxs-lookup"><span data-stu-id="01634-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01634-139">id</span><span class="sxs-lookup"><span data-stu-id="01634-139">id</span></span>|<span data-ttu-id="01634-140">String</span><span class="sxs-lookup"><span data-stu-id="01634-140">String</span></span>|<span data-ttu-id="01634-141">Это Id объекта.</span><span class="sxs-lookup"><span data-stu-id="01634-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="01634-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="01634-142">deviceId</span></span>|<span data-ttu-id="01634-143">String</span><span class="sxs-lookup"><span data-stu-id="01634-143">String</span></span>|<span data-ttu-id="01634-144">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="01634-144">The id of the device.</span></span>|
|<span data-ttu-id="01634-145">userId</span><span class="sxs-lookup"><span data-stu-id="01634-145">userId</span></span>|<span data-ttu-id="01634-146">String</span><span class="sxs-lookup"><span data-stu-id="01634-146">String</span></span>|<span data-ttu-id="01634-147">ID пользователя.</span><span class="sxs-lookup"><span data-stu-id="01634-147">The id of the user.</span></span>|
|<span data-ttu-id="01634-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="01634-148">deviceDisplayName</span></span>|<span data-ttu-id="01634-149">String</span><span class="sxs-lookup"><span data-stu-id="01634-149">String</span></span>|<span data-ttu-id="01634-150">Имя отображения устройства.</span><span class="sxs-lookup"><span data-stu-id="01634-150">Device display name.</span></span>|
|<span data-ttu-id="01634-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="01634-151">userPrincipalName</span></span>|<span data-ttu-id="01634-152">String</span><span class="sxs-lookup"><span data-stu-id="01634-152">String</span></span>|<span data-ttu-id="01634-153">Имя основного пользователя.</span><span class="sxs-lookup"><span data-stu-id="01634-153">User principal name.</span></span>|
|<span data-ttu-id="01634-154">status</span><span class="sxs-lookup"><span data-stu-id="01634-154">status</span></span>|[<span data-ttu-id="01634-155">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="01634-155">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="01634-156">Состояние udpate Windows.</span><span class="sxs-lookup"><span data-stu-id="01634-156">Windows udpate status.</span></span> <span data-ttu-id="01634-157">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="01634-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="01634-158">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="01634-158">qualityUpdateVersion</span></span>|<span data-ttu-id="01634-159">String</span><span class="sxs-lookup"><span data-stu-id="01634-159">String</span></span>|<span data-ttu-id="01634-160">Версия обновления качества устройства.</span><span class="sxs-lookup"><span data-stu-id="01634-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="01634-161">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="01634-161">featureUpdateVersion</span></span>|<span data-ttu-id="01634-162">String</span><span class="sxs-lookup"><span data-stu-id="01634-162">String</span></span>|<span data-ttu-id="01634-163">Текущая версия обновления функций устройства.</span><span class="sxs-lookup"><span data-stu-id="01634-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="01634-164">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="01634-164">lastScanDateTime</span></span>|<span data-ttu-id="01634-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01634-165">DateTimeOffset</span></span>|<span data-ttu-id="01634-166">Время даты успешного сканирования агентом обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="01634-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="01634-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="01634-167">lastSyncDateTime</span></span>|<span data-ttu-id="01634-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01634-168">DateTimeOffset</span></span>|<span data-ttu-id="01634-169">Последний раз, когда устройство синхронизируется с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="01634-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="01634-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="01634-170">Response</span></span>
<span data-ttu-id="01634-171">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsUpdateState](../resources/intune-shared-windowsupdatestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="01634-171">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01634-172">Пример</span><span class="sxs-lookup"><span data-stu-id="01634-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="01634-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="01634-173">Request</span></span>
<span data-ttu-id="01634-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01634-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01634-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="01634-175">Response</span></span>
<span data-ttu-id="01634-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01634-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








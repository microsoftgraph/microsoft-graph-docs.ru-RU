---
title: Создание windowsUpdateState
description: Создайте новый объект WindowsUpdateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e53a4bdc6bb07c9761cabeff5eec9886130bc942
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448013"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="a588c-103">Создание windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="a588c-103">Create windowsUpdateState</span></span>

<span data-ttu-id="a588c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a588c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a588c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a588c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a588c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a588c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a588c-107">Создайте [новый объект WindowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)</span><span class="sxs-lookup"><span data-stu-id="a588c-107">Create a new [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a588c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a588c-108">Prerequisites</span></span>
<span data-ttu-id="a588c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a588c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a588c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a588c-111">Permission type</span></span>|<span data-ttu-id="a588c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a588c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a588c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a588c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a588c-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="a588c-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a588c-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a588c-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="a588c-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="a588c-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="a588c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a588c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a588c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a588c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a588c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a588c-119">Not supported.</span></span>|
|<span data-ttu-id="a588c-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="a588c-120">Application</span></span>||
| <span data-ttu-id="a588c-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="a588c-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a588c-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a588c-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="a588c-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="a588c-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="a588c-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a588c-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a588c-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a588c-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="a588c-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a588c-126">Request headers</span></span>
|<span data-ttu-id="a588c-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a588c-127">Header</span></span>|<span data-ttu-id="a588c-128">Значение</span><span class="sxs-lookup"><span data-stu-id="a588c-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a588c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="a588c-129">Authorization</span></span>|<span data-ttu-id="a588c-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a588c-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a588c-131">Accept</span><span class="sxs-lookup"><span data-stu-id="a588c-131">Accept</span></span>|<span data-ttu-id="a588c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="a588c-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a588c-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a588c-133">Request body</span></span>
<span data-ttu-id="a588c-134">В теле запроса укажи представление JSON для объекта WindowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="a588c-134">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="a588c-135">В следующей таблице показаны свойства, необходимые при создании windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="a588c-135">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="a588c-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="a588c-136">Property</span></span>|<span data-ttu-id="a588c-137">Тип</span><span class="sxs-lookup"><span data-stu-id="a588c-137">Type</span></span>|<span data-ttu-id="a588c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="a588c-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a588c-139">id</span><span class="sxs-lookup"><span data-stu-id="a588c-139">id</span></span>|<span data-ttu-id="a588c-140">String</span><span class="sxs-lookup"><span data-stu-id="a588c-140">String</span></span>|<span data-ttu-id="a588c-141">Это Id объекта.</span><span class="sxs-lookup"><span data-stu-id="a588c-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="a588c-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="a588c-142">deviceId</span></span>|<span data-ttu-id="a588c-143">String</span><span class="sxs-lookup"><span data-stu-id="a588c-143">String</span></span>|<span data-ttu-id="a588c-144">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="a588c-144">The id of the device.</span></span>|
|<span data-ttu-id="a588c-145">userId</span><span class="sxs-lookup"><span data-stu-id="a588c-145">userId</span></span>|<span data-ttu-id="a588c-146">String</span><span class="sxs-lookup"><span data-stu-id="a588c-146">String</span></span>|<span data-ttu-id="a588c-147">ID пользователя.</span><span class="sxs-lookup"><span data-stu-id="a588c-147">The id of the user.</span></span>|
|<span data-ttu-id="a588c-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a588c-148">deviceDisplayName</span></span>|<span data-ttu-id="a588c-149">String</span><span class="sxs-lookup"><span data-stu-id="a588c-149">String</span></span>|<span data-ttu-id="a588c-150">Имя отображения устройства.</span><span class="sxs-lookup"><span data-stu-id="a588c-150">Device display name.</span></span>|
|<span data-ttu-id="a588c-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a588c-151">userPrincipalName</span></span>|<span data-ttu-id="a588c-152">String</span><span class="sxs-lookup"><span data-stu-id="a588c-152">String</span></span>|<span data-ttu-id="a588c-153">Имя основного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a588c-153">User principal name.</span></span>|
|<span data-ttu-id="a588c-154">status</span><span class="sxs-lookup"><span data-stu-id="a588c-154">status</span></span>|[<span data-ttu-id="a588c-155">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="a588c-155">windowsUpdateStatus</span></span>](../resources/intune-shared-windowsupdatestatus.md)|<span data-ttu-id="a588c-156">Состояние udpate Windows.</span><span class="sxs-lookup"><span data-stu-id="a588c-156">Windows udpate status.</span></span> <span data-ttu-id="a588c-157">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a588c-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="a588c-158">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="a588c-158">qualityUpdateVersion</span></span>|<span data-ttu-id="a588c-159">String</span><span class="sxs-lookup"><span data-stu-id="a588c-159">String</span></span>|<span data-ttu-id="a588c-160">Версия обновления качества устройства.</span><span class="sxs-lookup"><span data-stu-id="a588c-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="a588c-161">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="a588c-161">featureUpdateVersion</span></span>|<span data-ttu-id="a588c-162">String</span><span class="sxs-lookup"><span data-stu-id="a588c-162">String</span></span>|<span data-ttu-id="a588c-163">Текущая версия обновления функций устройства.</span><span class="sxs-lookup"><span data-stu-id="a588c-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="a588c-164">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a588c-164">lastScanDateTime</span></span>|<span data-ttu-id="a588c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a588c-165">DateTimeOffset</span></span>|<span data-ttu-id="a588c-166">Время даты успешного сканирования агентом обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="a588c-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="a588c-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a588c-167">lastSyncDateTime</span></span>|<span data-ttu-id="a588c-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a588c-168">DateTimeOffset</span></span>|<span data-ttu-id="a588c-169">Последний раз, когда устройство синхронизируется с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="a588c-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="a588c-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="a588c-170">Response</span></span>
<span data-ttu-id="a588c-171">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект WindowsUpdateState](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a588c-171">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a588c-172">Пример</span><span class="sxs-lookup"><span data-stu-id="a588c-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="a588c-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="a588c-173">Request</span></span>
<span data-ttu-id="a588c-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a588c-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
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

### <a name="response"></a><span data-ttu-id="a588c-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="a588c-175">Response</span></span>
<span data-ttu-id="a588c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a588c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








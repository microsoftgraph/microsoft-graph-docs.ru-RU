---
title: Обновление Виндовсупдатестате
description: Обновление свойств объекта Виндовсупдатестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8d9168a22fcff105cbf2603ebccaaf4b9c0d8cf5
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124025"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="6c3fd-103">Обновление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="6c3fd-103">Update windowsUpdateState</span></span>

<span data-ttu-id="6c3fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c3fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c3fd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c3fd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c3fd-107">Обновление свойств объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="6c3fd-107">Update the properties of a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c3fd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6c3fd-108">Prerequisites</span></span>
<span data-ttu-id="6c3fd-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6c3fd-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c3fd-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c3fd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c3fd-111">Permission type</span></span>|<span data-ttu-id="6c3fd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c3fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c3fd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c3fd-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6c3fd-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="6c3fd-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6c3fd-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c3fd-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="6c3fd-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="6c3fd-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="6c3fd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c3fd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c3fd-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c3fd-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c3fd-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-119">Not supported.</span></span>|
|<span data-ttu-id="6c3fd-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c3fd-120">Application</span></span>||
| <span data-ttu-id="6c3fd-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="6c3fd-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6c3fd-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c3fd-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="6c3fd-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="6c3fd-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="6c3fd-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c3fd-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c3fd-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c3fd-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="6c3fd-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6c3fd-126">Request headers</span></span>
|<span data-ttu-id="6c3fd-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c3fd-127">Header</span></span>|<span data-ttu-id="6c3fd-128">Значение</span><span class="sxs-lookup"><span data-stu-id="6c3fd-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c3fd-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c3fd-129">Authorization</span></span>|<span data-ttu-id="6c3fd-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c3fd-131">Accept</span><span class="sxs-lookup"><span data-stu-id="6c3fd-131">Accept</span></span>|<span data-ttu-id="6c3fd-132">application/json</span><span class="sxs-lookup"><span data-stu-id="6c3fd-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c3fd-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c3fd-133">Request body</span></span>
<span data-ttu-id="6c3fd-134">В тексте запроса добавьте представление объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-134">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="6c3fd-135">В следующей таблице приведены свойства, необходимые при создании [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="6c3fd-135">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

|<span data-ttu-id="6c3fd-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c3fd-136">Property</span></span>|<span data-ttu-id="6c3fd-137">Тип</span><span class="sxs-lookup"><span data-stu-id="6c3fd-137">Type</span></span>|<span data-ttu-id="6c3fd-138">Описание</span><span class="sxs-lookup"><span data-stu-id="6c3fd-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c3fd-139">id</span><span class="sxs-lookup"><span data-stu-id="6c3fd-139">id</span></span>|<span data-ttu-id="6c3fd-140">Строка</span><span class="sxs-lookup"><span data-stu-id="6c3fd-140">String</span></span>|<span data-ttu-id="6c3fd-141">Это идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="6c3fd-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="6c3fd-142">deviceId</span></span>|<span data-ttu-id="6c3fd-143">String</span><span class="sxs-lookup"><span data-stu-id="6c3fd-143">String</span></span>|<span data-ttu-id="6c3fd-144">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-144">The id of the device.</span></span>|
|<span data-ttu-id="6c3fd-145">userId</span><span class="sxs-lookup"><span data-stu-id="6c3fd-145">userId</span></span>|<span data-ttu-id="6c3fd-146">String</span><span class="sxs-lookup"><span data-stu-id="6c3fd-146">String</span></span>|<span data-ttu-id="6c3fd-147">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-147">The id of the user.</span></span>|
|<span data-ttu-id="6c3fd-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6c3fd-148">deviceDisplayName</span></span>|<span data-ttu-id="6c3fd-149">String</span><span class="sxs-lookup"><span data-stu-id="6c3fd-149">String</span></span>|<span data-ttu-id="6c3fd-150">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-150">Device display name.</span></span>|
|<span data-ttu-id="6c3fd-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6c3fd-151">userPrincipalName</span></span>|<span data-ttu-id="6c3fd-152">Строка</span><span class="sxs-lookup"><span data-stu-id="6c3fd-152">String</span></span>|<span data-ttu-id="6c3fd-153">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-153">User principal name.</span></span>|
|<span data-ttu-id="6c3fd-154">status</span><span class="sxs-lookup"><span data-stu-id="6c3fd-154">status</span></span>|[<span data-ttu-id="6c3fd-155">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="6c3fd-155">windowsUpdateStatus</span></span>](../resources/intune-shared-windowsupdatestatus.md)|<span data-ttu-id="6c3fd-156">Состояние Windows удпате.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-156">Windows udpate status.</span></span> <span data-ttu-id="6c3fd-157">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="6c3fd-158">куалитюпдатеверсион</span><span class="sxs-lookup"><span data-stu-id="6c3fd-158">qualityUpdateVersion</span></span>|<span data-ttu-id="6c3fd-159">String</span><span class="sxs-lookup"><span data-stu-id="6c3fd-159">String</span></span>|<span data-ttu-id="6c3fd-160">Версия устройства для обновления качества.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="6c3fd-161">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="6c3fd-161">featureUpdateVersion</span></span>|<span data-ttu-id="6c3fd-162">String</span><span class="sxs-lookup"><span data-stu-id="6c3fd-162">String</span></span>|<span data-ttu-id="6c3fd-163">Текущая версия обновления компонентов устройства.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="6c3fd-164">ластскандатетиме</span><span class="sxs-lookup"><span data-stu-id="6c3fd-164">lastScanDateTime</span></span>|<span data-ttu-id="6c3fd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c3fd-165">DateTimeOffset</span></span>|<span data-ttu-id="6c3fd-166">Дата и время, когда агент обновления Windows успешно выполнил сканирование.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="6c3fd-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6c3fd-167">lastSyncDateTime</span></span>|<span data-ttu-id="6c3fd-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c3fd-168">DateTimeOffset</span></span>|<span data-ttu-id="6c3fd-169">Дата и время последней синхронизации устройства с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="6c3fd-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c3fd-170">Response</span></span>
<span data-ttu-id="6c3fd-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-171">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c3fd-172">Пример</span><span class="sxs-lookup"><span data-stu-id="6c3fd-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c3fd-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c3fd-173">Request</span></span>
<span data-ttu-id="6c3fd-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6c3fd-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c3fd-175">Response</span></span>
<span data-ttu-id="6c3fd-176">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-176">Here is an example of the response.</span></span> <span data-ttu-id="6c3fd-177">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-177">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6c3fd-178">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6c3fd-178">All of the properties will be returned from an actual call.</span></span>
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







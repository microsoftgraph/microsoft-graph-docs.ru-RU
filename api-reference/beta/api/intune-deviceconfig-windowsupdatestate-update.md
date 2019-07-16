---
title: Обновление Виндовсупдатестате
description: Обновление свойств объекта Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f003e5066e0e2b31b1b629067ffacc92efdd36de
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726173"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="64c63-103">Обновление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="64c63-103">Update windowsUpdateState</span></span>

> <span data-ttu-id="64c63-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64c63-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64c63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64c63-106">Обновление свойств объекта [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="64c63-106">Update the properties of a [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64c63-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="64c63-107">Prerequisites</span></span>
<span data-ttu-id="64c63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64c63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64c63-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64c63-110">Permission type</span></span>|<span data-ttu-id="64c63-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64c63-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64c63-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64c63-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64c63-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c63-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64c63-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64c63-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64c63-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c63-115">Not supported.</span></span>|
|<span data-ttu-id="64c63-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64c63-116">Application</span></span>|<span data-ttu-id="64c63-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c63-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64c63-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64c63-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="64c63-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64c63-119">Request headers</span></span>
|<span data-ttu-id="64c63-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64c63-120">Header</span></span>|<span data-ttu-id="64c63-121">Значение</span><span class="sxs-lookup"><span data-stu-id="64c63-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64c63-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64c63-122">Authorization</span></span>|<span data-ttu-id="64c63-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64c63-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64c63-124">Accept</span><span class="sxs-lookup"><span data-stu-id="64c63-124">Accept</span></span>|<span data-ttu-id="64c63-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64c63-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64c63-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64c63-126">Request body</span></span>
<span data-ttu-id="64c63-127">В тексте запроса добавьте представление объекта [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64c63-127">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="64c63-128">В следующей таблице приведены свойства, необходимые при создании [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="64c63-128">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md).</span></span>

|<span data-ttu-id="64c63-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="64c63-129">Property</span></span>|<span data-ttu-id="64c63-130">Тип</span><span class="sxs-lookup"><span data-stu-id="64c63-130">Type</span></span>|<span data-ttu-id="64c63-131">Описание</span><span class="sxs-lookup"><span data-stu-id="64c63-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64c63-132">id</span><span class="sxs-lookup"><span data-stu-id="64c63-132">id</span></span>|<span data-ttu-id="64c63-133">Строка</span><span class="sxs-lookup"><span data-stu-id="64c63-133">String</span></span>|<span data-ttu-id="64c63-134">Это идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="64c63-134">This is Id of the entity.</span></span>|
|<span data-ttu-id="64c63-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="64c63-135">deviceId</span></span>|<span data-ttu-id="64c63-136">String</span><span class="sxs-lookup"><span data-stu-id="64c63-136">String</span></span>|<span data-ttu-id="64c63-137">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="64c63-137">The id of the device.</span></span>|
|<span data-ttu-id="64c63-138">userId</span><span class="sxs-lookup"><span data-stu-id="64c63-138">userId</span></span>|<span data-ttu-id="64c63-139">String</span><span class="sxs-lookup"><span data-stu-id="64c63-139">String</span></span>|<span data-ttu-id="64c63-140">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="64c63-140">The id of the user.</span></span>|
|<span data-ttu-id="64c63-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="64c63-141">deviceDisplayName</span></span>|<span data-ttu-id="64c63-142">String</span><span class="sxs-lookup"><span data-stu-id="64c63-142">String</span></span>|<span data-ttu-id="64c63-143">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="64c63-143">Device display name.</span></span>|
|<span data-ttu-id="64c63-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="64c63-144">userPrincipalName</span></span>|<span data-ttu-id="64c63-145">Строка</span><span class="sxs-lookup"><span data-stu-id="64c63-145">String</span></span>|<span data-ttu-id="64c63-146">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="64c63-146">User principal name.</span></span>|
|<span data-ttu-id="64c63-147">status</span><span class="sxs-lookup"><span data-stu-id="64c63-147">status</span></span>|[<span data-ttu-id="64c63-148">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="64c63-148">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="64c63-149">Состояние Windows удпате.</span><span class="sxs-lookup"><span data-stu-id="64c63-149">Windows udpate status.</span></span> <span data-ttu-id="64c63-150">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="64c63-150">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="64c63-151">Куалитюпдатеверсион</span><span class="sxs-lookup"><span data-stu-id="64c63-151">qualityUpdateVersion</span></span>|<span data-ttu-id="64c63-152">String</span><span class="sxs-lookup"><span data-stu-id="64c63-152">String</span></span>|<span data-ttu-id="64c63-153">Версия устройства для обновления качества.</span><span class="sxs-lookup"><span data-stu-id="64c63-153">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="64c63-154">Феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="64c63-154">featureUpdateVersion</span></span>|<span data-ttu-id="64c63-155">String</span><span class="sxs-lookup"><span data-stu-id="64c63-155">String</span></span>|<span data-ttu-id="64c63-156">Текущая версия обновления компонентов устройства.</span><span class="sxs-lookup"><span data-stu-id="64c63-156">The current feature update version of the device.</span></span>|
|<span data-ttu-id="64c63-157">Ластскандатетиме</span><span class="sxs-lookup"><span data-stu-id="64c63-157">lastScanDateTime</span></span>|<span data-ttu-id="64c63-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64c63-158">DateTimeOffset</span></span>|<span data-ttu-id="64c63-159">Дата и время, когда агент обновления Windows успешно выполнил сканирование.</span><span class="sxs-lookup"><span data-stu-id="64c63-159">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="64c63-160">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="64c63-160">lastSyncDateTime</span></span>|<span data-ttu-id="64c63-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64c63-161">DateTimeOffset</span></span>|<span data-ttu-id="64c63-162">Дата и время последней синхронизации устройства с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="64c63-162">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="64c63-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c63-163">Response</span></span>
<span data-ttu-id="64c63-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64c63-164">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64c63-165">Пример</span><span class="sxs-lookup"><span data-stu-id="64c63-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="64c63-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="64c63-166">Request</span></span>
<span data-ttu-id="64c63-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64c63-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="64c63-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c63-168">Response</span></span>
<span data-ttu-id="64c63-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64c63-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






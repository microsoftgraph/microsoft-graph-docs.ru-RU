---
title: Обновление Виндовсупдатестате
description: Обновление свойств объекта Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35a56a0dea3174a7f196a3cee62a46edd35eafce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344135"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="978d6-103">Обновление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="978d6-103">Update windowsUpdateState</span></span>

> <span data-ttu-id="978d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="978d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="978d6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="978d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="978d6-106">Обновление свойств объекта [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="978d6-106">Update the properties of a [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="978d6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="978d6-107">Prerequisites</span></span>
<span data-ttu-id="978d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="978d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="978d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="978d6-110">Permission type</span></span>|<span data-ttu-id="978d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="978d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="978d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="978d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="978d6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="978d6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="978d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="978d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="978d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="978d6-115">Not supported.</span></span>|
|<span data-ttu-id="978d6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="978d6-116">Application</span></span>|<span data-ttu-id="978d6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="978d6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="978d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="978d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="978d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="978d6-119">Request headers</span></span>
|<span data-ttu-id="978d6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="978d6-120">Header</span></span>|<span data-ttu-id="978d6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="978d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="978d6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="978d6-122">Authorization</span></span>|<span data-ttu-id="978d6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="978d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="978d6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="978d6-124">Accept</span></span>|<span data-ttu-id="978d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="978d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="978d6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="978d6-126">Request body</span></span>
<span data-ttu-id="978d6-127">В тексте запроса добавьте представление объекта [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="978d6-127">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="978d6-128">В следующей таблице приведены свойства, необходимые при создании [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="978d6-128">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md).</span></span>

|<span data-ttu-id="978d6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="978d6-129">Property</span></span>|<span data-ttu-id="978d6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="978d6-130">Type</span></span>|<span data-ttu-id="978d6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="978d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="978d6-132">id</span><span class="sxs-lookup"><span data-stu-id="978d6-132">id</span></span>|<span data-ttu-id="978d6-133">Строка</span><span class="sxs-lookup"><span data-stu-id="978d6-133">String</span></span>|<span data-ttu-id="978d6-134">Это идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="978d6-134">This is Id of the entity.</span></span>|
|<span data-ttu-id="978d6-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="978d6-135">deviceId</span></span>|<span data-ttu-id="978d6-136">String</span><span class="sxs-lookup"><span data-stu-id="978d6-136">String</span></span>|<span data-ttu-id="978d6-137">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="978d6-137">The id of the device.</span></span>|
|<span data-ttu-id="978d6-138">userId</span><span class="sxs-lookup"><span data-stu-id="978d6-138">userId</span></span>|<span data-ttu-id="978d6-139">String</span><span class="sxs-lookup"><span data-stu-id="978d6-139">String</span></span>|<span data-ttu-id="978d6-140">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="978d6-140">The id of the user.</span></span>|
|<span data-ttu-id="978d6-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="978d6-141">deviceDisplayName</span></span>|<span data-ttu-id="978d6-142">String</span><span class="sxs-lookup"><span data-stu-id="978d6-142">String</span></span>|<span data-ttu-id="978d6-143">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="978d6-143">Device display name.</span></span>|
|<span data-ttu-id="978d6-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="978d6-144">userPrincipalName</span></span>|<span data-ttu-id="978d6-145">Строка</span><span class="sxs-lookup"><span data-stu-id="978d6-145">String</span></span>|<span data-ttu-id="978d6-146">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="978d6-146">User principal name.</span></span>|
|<span data-ttu-id="978d6-147">status</span><span class="sxs-lookup"><span data-stu-id="978d6-147">status</span></span>|[<span data-ttu-id="978d6-148">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="978d6-148">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="978d6-149">Состояние Windows удпате.</span><span class="sxs-lookup"><span data-stu-id="978d6-149">Windows udpate status.</span></span> <span data-ttu-id="978d6-150">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="978d6-150">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="978d6-151">куалитюпдатеверсион</span><span class="sxs-lookup"><span data-stu-id="978d6-151">qualityUpdateVersion</span></span>|<span data-ttu-id="978d6-152">String</span><span class="sxs-lookup"><span data-stu-id="978d6-152">String</span></span>|<span data-ttu-id="978d6-153">Версия устройства для обновления качества.</span><span class="sxs-lookup"><span data-stu-id="978d6-153">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="978d6-154">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="978d6-154">featureUpdateVersion</span></span>|<span data-ttu-id="978d6-155">String</span><span class="sxs-lookup"><span data-stu-id="978d6-155">String</span></span>|<span data-ttu-id="978d6-156">Текущая версия обновления компонентов устройства.</span><span class="sxs-lookup"><span data-stu-id="978d6-156">The current feature update version of the device.</span></span>|
|<span data-ttu-id="978d6-157">ластскандатетиме</span><span class="sxs-lookup"><span data-stu-id="978d6-157">lastScanDateTime</span></span>|<span data-ttu-id="978d6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="978d6-158">DateTimeOffset</span></span>|<span data-ttu-id="978d6-159">Дата и время, когда агент обновления Windows успешно выполнил сканирование.</span><span class="sxs-lookup"><span data-stu-id="978d6-159">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="978d6-160">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="978d6-160">lastSyncDateTime</span></span>|<span data-ttu-id="978d6-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="978d6-161">DateTimeOffset</span></span>|<span data-ttu-id="978d6-162">Дата и время последней синхронизации устройства с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="978d6-162">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="978d6-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="978d6-163">Response</span></span>
<span data-ttu-id="978d6-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="978d6-164">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="978d6-165">Пример</span><span class="sxs-lookup"><span data-stu-id="978d6-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="978d6-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="978d6-166">Request</span></span>
<span data-ttu-id="978d6-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="978d6-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="978d6-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="978d6-168">Response</span></span>
<span data-ttu-id="978d6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="978d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







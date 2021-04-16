---
title: Создание userExperienceAnalyticsNotAutopilotReadyDevice
description: Создание нового объекта userExperienceAnalyticsNotAutopilotReadyDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1473c0a856636dc5373239c1bed4c2caed9ea78b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865224"
---
# <a name="create-userexperienceanalyticsnotautopilotreadydevice"></a><span data-ttu-id="d1f03-103">Создание userExperienceAnalyticsNotAutopilotReadyDevice</span><span class="sxs-lookup"><span data-stu-id="d1f03-103">Create userExperienceAnalyticsNotAutopilotReadyDevice</span></span>

<span data-ttu-id="d1f03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1f03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1f03-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1f03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1f03-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1f03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1f03-107">Создание нового [объекта userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)</span><span class="sxs-lookup"><span data-stu-id="d1f03-107">Create a new [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1f03-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d1f03-108">Prerequisites</span></span>
<span data-ttu-id="d1f03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1f03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1f03-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1f03-111">Permission type</span></span>|<span data-ttu-id="d1f03-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1f03-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1f03-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1f03-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1f03-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1f03-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d1f03-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1f03-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1f03-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1f03-116">Not supported.</span></span>|
|<span data-ttu-id="d1f03-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d1f03-117">Application</span></span>|<span data-ttu-id="d1f03-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1f03-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1f03-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1f03-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
```

## <a name="request-headers"></a><span data-ttu-id="d1f03-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d1f03-120">Request headers</span></span>
|<span data-ttu-id="d1f03-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1f03-121">Header</span></span>|<span data-ttu-id="d1f03-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d1f03-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1f03-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1f03-123">Authorization</span></span>|<span data-ttu-id="d1f03-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1f03-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1f03-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d1f03-125">Accept</span></span>|<span data-ttu-id="d1f03-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1f03-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1f03-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1f03-127">Request body</span></span>
<span data-ttu-id="d1f03-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsNotAutopilotReadyDevice.</span><span class="sxs-lookup"><span data-stu-id="d1f03-128">In the request body, supply a JSON representation for the userExperienceAnalyticsNotAutopilotReadyDevice object.</span></span>

<span data-ttu-id="d1f03-129">В следующей таблице показаны свойства, необходимые при создании пользователяExperienceAnalyticsNotAutopilotReadyDevice.</span><span class="sxs-lookup"><span data-stu-id="d1f03-129">The following table shows the properties that are required when you create the userExperienceAnalyticsNotAutopilotReadyDevice.</span></span>

|<span data-ttu-id="d1f03-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1f03-130">Property</span></span>|<span data-ttu-id="d1f03-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d1f03-131">Type</span></span>|<span data-ttu-id="d1f03-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f03-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1f03-133">id</span><span class="sxs-lookup"><span data-stu-id="d1f03-133">id</span></span>|<span data-ttu-id="d1f03-134">String</span><span class="sxs-lookup"><span data-stu-id="d1f03-134">String</span></span>|<span data-ttu-id="d1f03-135">Уникальный идентификатор устройства intune аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="d1f03-135">The unique identifier of the user experience analytics intune device.</span></span>|
|<span data-ttu-id="d1f03-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="d1f03-136">deviceName</span></span>|<span data-ttu-id="d1f03-137">String</span><span class="sxs-lookup"><span data-stu-id="d1f03-137">String</span></span>|<span data-ttu-id="d1f03-138">Имя устройства intune.</span><span class="sxs-lookup"><span data-stu-id="d1f03-138">The intune device's name.</span></span>|
|<span data-ttu-id="d1f03-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d1f03-139">serialNumber</span></span>|<span data-ttu-id="d1f03-140">String</span><span class="sxs-lookup"><span data-stu-id="d1f03-140">String</span></span>|<span data-ttu-id="d1f03-141">Серийный номер устройства intune.</span><span class="sxs-lookup"><span data-stu-id="d1f03-141">The intune device's serial number.</span></span>|
|<span data-ttu-id="d1f03-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="d1f03-142">manufacturer</span></span>|<span data-ttu-id="d1f03-143">String</span><span class="sxs-lookup"><span data-stu-id="d1f03-143">String</span></span>|<span data-ttu-id="d1f03-144">Производитель устройства intune.</span><span class="sxs-lookup"><span data-stu-id="d1f03-144">The intune device's manufacturer.</span></span>|
|<span data-ttu-id="d1f03-145">model</span><span class="sxs-lookup"><span data-stu-id="d1f03-145">model</span></span>|<span data-ttu-id="d1f03-146">String</span><span class="sxs-lookup"><span data-stu-id="d1f03-146">String</span></span>|<span data-ttu-id="d1f03-147">Модель устройства intune.</span><span class="sxs-lookup"><span data-stu-id="d1f03-147">The intune device's model.</span></span>|
|<span data-ttu-id="d1f03-148">managedBy</span><span class="sxs-lookup"><span data-stu-id="d1f03-148">managedBy</span></span>|<span data-ttu-id="d1f03-149">String</span><span class="sxs-lookup"><span data-stu-id="d1f03-149">String</span></span>|<span data-ttu-id="d1f03-150">Устройство intune управляется.</span><span class="sxs-lookup"><span data-stu-id="d1f03-150">The intune device's managed by.</span></span>|
|<span data-ttu-id="d1f03-151">autoPilotRegistered</span><span class="sxs-lookup"><span data-stu-id="d1f03-151">autoPilotRegistered</span></span>|<span data-ttu-id="d1f03-152">Логический</span><span class="sxs-lookup"><span data-stu-id="d1f03-152">Boolean</span></span>|<span data-ttu-id="d1f03-153">Автопилотрегистер устройства intune.</span><span class="sxs-lookup"><span data-stu-id="d1f03-153">The intune device's autopilotRegistered.</span></span>|
|<span data-ttu-id="d1f03-154">autoPilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="d1f03-154">autoPilotProfileAssigned</span></span>|<span data-ttu-id="d1f03-155">Логический</span><span class="sxs-lookup"><span data-stu-id="d1f03-155">Boolean</span></span>|<span data-ttu-id="d1f03-156">Автопилот Устройства intuneProfileAssigned.</span><span class="sxs-lookup"><span data-stu-id="d1f03-156">The intune device's autopilotProfileAssigned.</span></span>|
|<span data-ttu-id="d1f03-157">azureAdRegistered</span><span class="sxs-lookup"><span data-stu-id="d1f03-157">azureAdRegistered</span></span>|<span data-ttu-id="d1f03-158">Логический</span><span class="sxs-lookup"><span data-stu-id="d1f03-158">Boolean</span></span>|<span data-ttu-id="d1f03-159">Устройство intune azureAdRegistered.</span><span class="sxs-lookup"><span data-stu-id="d1f03-159">The intune device's azureAdRegistered.</span></span>|
|<span data-ttu-id="d1f03-160">azureAdJoinType</span><span class="sxs-lookup"><span data-stu-id="d1f03-160">azureAdJoinType</span></span>|<span data-ttu-id="d1f03-161">String</span><span class="sxs-lookup"><span data-stu-id="d1f03-161">String</span></span>|<span data-ttu-id="d1f03-162">Azure Ad ad для устройства intune присоединяется кType.</span><span class="sxs-lookup"><span data-stu-id="d1f03-162">The intune device's azure Ad joinType.</span></span>|



## <a name="response"></a><span data-ttu-id="d1f03-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1f03-163">Response</span></span>
<span data-ttu-id="d1f03-164">В случае успеха этот метод возвращает код ответа и `201 Created` [объект userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d1f03-164">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1f03-165">Пример</span><span class="sxs-lookup"><span data-stu-id="d1f03-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1f03-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1f03-166">Request</span></span>
<span data-ttu-id="d1f03-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1f03-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
Content-type: application/json
Content-length: 421

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdJoinType": "Azure Ad Join Type value"
}
```

### <a name="response"></a><span data-ttu-id="d1f03-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1f03-168">Response</span></span>
<span data-ttu-id="d1f03-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1f03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 470

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "id": "11c3ffd7-ffd7-11c3-d7ff-c311d7ffc311",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdJoinType": "Azure Ad Join Type value"
}
```





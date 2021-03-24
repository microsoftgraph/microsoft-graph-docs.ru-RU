---
title: Создание deviceManagementIntentDeviceSettingStateSummary
description: Создайте новый объект deviceManagementIntentDeviceSettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f4598dc4faeaf6a7cae417d6e7182d3dc7e5ce0d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128756"
---
# <a name="create-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="1e9a8-103">Создание deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="1e9a8-103">Create deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="1e9a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e9a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e9a8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e9a8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e9a8-107">Создайте новый [объект deviceManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="1e9a8-107">Create a new [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e9a8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1e9a8-108">Prerequisites</span></span>
<span data-ttu-id="1e9a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e9a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e9a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e9a8-111">Permission type</span></span>|<span data-ttu-id="1e9a8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e9a8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e9a8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e9a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e9a8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e9a8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e9a8-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e9a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e9a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-116">Not supported.</span></span>|
|<span data-ttu-id="1e9a8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1e9a8-117">Application</span></span>|<span data-ttu-id="1e9a8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e9a8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e9a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e9a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="1e9a8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1e9a8-120">Request headers</span></span>
|<span data-ttu-id="1e9a8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e9a8-121">Header</span></span>|<span data-ttu-id="1e9a8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1e9a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e9a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e9a8-123">Authorization</span></span>|<span data-ttu-id="1e9a8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e9a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e9a8-125">Accept</span></span>|<span data-ttu-id="1e9a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e9a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e9a8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e9a8-127">Request body</span></span>
<span data-ttu-id="1e9a8-128">В корпусе запроса поставляем представление JSON для объекта deviceManagementIntentDeviceSettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-128">In the request body, supply a JSON representation for the deviceManagementIntentDeviceSettingStateSummary object.</span></span>

<span data-ttu-id="1e9a8-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementIntentDeviceSettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-129">The following table shows the properties that are required when you create the deviceManagementIntentDeviceSettingStateSummary.</span></span>

|<span data-ttu-id="1e9a8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e9a8-130">Property</span></span>|<span data-ttu-id="1e9a8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1e9a8-131">Type</span></span>|<span data-ttu-id="1e9a8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1e9a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e9a8-133">id</span><span class="sxs-lookup"><span data-stu-id="1e9a8-133">id</span></span>|<span data-ttu-id="1e9a8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1e9a8-134">String</span></span>|<span data-ttu-id="1e9a8-135">The ID</span><span class="sxs-lookup"><span data-stu-id="1e9a8-135">The ID</span></span>|
|<span data-ttu-id="1e9a8-136">settingName</span><span class="sxs-lookup"><span data-stu-id="1e9a8-136">settingName</span></span>|<span data-ttu-id="1e9a8-137">String</span><span class="sxs-lookup"><span data-stu-id="1e9a8-137">String</span></span>|<span data-ttu-id="1e9a8-138">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="1e9a8-138">Name of a setting</span></span>|
|<span data-ttu-id="1e9a8-139">compliantCount</span><span class="sxs-lookup"><span data-stu-id="1e9a8-139">compliantCount</span></span>|<span data-ttu-id="1e9a8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1e9a8-140">Int32</span></span>|<span data-ttu-id="1e9a8-141">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-141">Number of compliant devices</span></span>|
|<span data-ttu-id="1e9a8-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="1e9a8-142">conflictCount</span></span>|<span data-ttu-id="1e9a8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1e9a8-143">Int32</span></span>|<span data-ttu-id="1e9a8-144">Количество устройств в конфликте</span><span class="sxs-lookup"><span data-stu-id="1e9a8-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="1e9a8-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="1e9a8-145">errorCount</span></span>|<span data-ttu-id="1e9a8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1e9a8-146">Int32</span></span>|<span data-ttu-id="1e9a8-147">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-147">Number of error devices</span></span>|
|<span data-ttu-id="1e9a8-148">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="1e9a8-148">nonCompliantCount</span></span>|<span data-ttu-id="1e9a8-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1e9a8-149">Int32</span></span>|<span data-ttu-id="1e9a8-150">Число устройств, не совместимых с соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="1e9a8-150">Number of non compliant devices</span></span>|
|<span data-ttu-id="1e9a8-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1e9a8-151">notApplicableCount</span></span>|<span data-ttu-id="1e9a8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1e9a8-152">Int32</span></span>|<span data-ttu-id="1e9a8-153">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-153">Number of not applicable devices</span></span>|
|<span data-ttu-id="1e9a8-154">исправленоКоунт</span><span class="sxs-lookup"><span data-stu-id="1e9a8-154">remediatedCount</span></span>|<span data-ttu-id="1e9a8-155">Int32</span><span class="sxs-lookup"><span data-stu-id="1e9a8-155">Int32</span></span>|<span data-ttu-id="1e9a8-156">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-156">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="1e9a8-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e9a8-157">Response</span></span>
<span data-ttu-id="1e9a8-158">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-158">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e9a8-159">Пример</span><span class="sxs-lookup"><span data-stu-id="1e9a8-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e9a8-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e9a8-160">Request</span></span>
<span data-ttu-id="1e9a8-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
Content-type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```

### <a name="response"></a><span data-ttu-id="1e9a8-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e9a8-162">Response</span></span>
<span data-ttu-id="1e9a8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e9a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 329

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "d3d3a75f-a75f-d3d3-5fa7-d3d35fa7d3d3",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```





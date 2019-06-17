---
title: Создание Девицеманажементинтентдевицесеттингстатесуммари
description: Создание нового объекта Девицеманажементинтентдевицесеттингстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91ca4f510a70af4fff6790450a209ebec462726c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960330"
---
# <a name="create-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="b7f86-103">Создание Девицеманажементинтентдевицесеттингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="b7f86-103">Create deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="b7f86-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7f86-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7f86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7f86-106">Создание нового объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b7f86-106">Create a new [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7f86-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b7f86-107">Prerequisites</span></span>
<span data-ttu-id="b7f86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7f86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7f86-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7f86-110">Permission type</span></span>|<span data-ttu-id="b7f86-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7f86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7f86-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7f86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7f86-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7f86-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7f86-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7f86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7f86-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f86-115">Not supported.</span></span>|
|<span data-ttu-id="b7f86-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7f86-116">Application</span></span>|<span data-ttu-id="b7f86-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f86-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7f86-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7f86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="b7f86-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7f86-119">Request headers</span></span>
|<span data-ttu-id="b7f86-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7f86-120">Header</span></span>|<span data-ttu-id="b7f86-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b7f86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7f86-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7f86-122">Authorization</span></span>|<span data-ttu-id="b7f86-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7f86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7f86-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b7f86-124">Accept</span></span>|<span data-ttu-id="b7f86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7f86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7f86-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7f86-126">Request body</span></span>
<span data-ttu-id="b7f86-127">В тексте запроса добавьте представление объекта Девицеманажементинтентдевицесеттингстатесуммари в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7f86-127">In the request body, supply a JSON representation for the deviceManagementIntentDeviceSettingStateSummary object.</span></span>

<span data-ttu-id="b7f86-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтентдевицесеттингстатесуммари.</span><span class="sxs-lookup"><span data-stu-id="b7f86-128">The following table shows the properties that are required when you create the deviceManagementIntentDeviceSettingStateSummary.</span></span>

|<span data-ttu-id="b7f86-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7f86-129">Property</span></span>|<span data-ttu-id="b7f86-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b7f86-130">Type</span></span>|<span data-ttu-id="b7f86-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b7f86-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7f86-132">id</span><span class="sxs-lookup"><span data-stu-id="b7f86-132">id</span></span>|<span data-ttu-id="b7f86-133">String</span><span class="sxs-lookup"><span data-stu-id="b7f86-133">String</span></span>|<span data-ttu-id="b7f86-134">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="b7f86-134">The ID</span></span>|
|<span data-ttu-id="b7f86-135">settingName</span><span class="sxs-lookup"><span data-stu-id="b7f86-135">settingName</span></span>|<span data-ttu-id="b7f86-136">String</span><span class="sxs-lookup"><span data-stu-id="b7f86-136">String</span></span>|<span data-ttu-id="b7f86-137">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="b7f86-137">Name of a setting</span></span>|
|<span data-ttu-id="b7f86-138">Комплианткаунт</span><span class="sxs-lookup"><span data-stu-id="b7f86-138">compliantCount</span></span>|<span data-ttu-id="b7f86-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f86-139">Int32</span></span>|<span data-ttu-id="b7f86-140">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="b7f86-140">Number of compliant devices</span></span>|
|<span data-ttu-id="b7f86-141">conflictCount</span><span class="sxs-lookup"><span data-stu-id="b7f86-141">conflictCount</span></span>|<span data-ttu-id="b7f86-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f86-142">Int32</span></span>|<span data-ttu-id="b7f86-143">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="b7f86-143">Number of devices in conflict</span></span>|
|<span data-ttu-id="b7f86-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="b7f86-144">errorCount</span></span>|<span data-ttu-id="b7f86-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f86-145">Int32</span></span>|<span data-ttu-id="b7f86-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="b7f86-146">Number of error devices</span></span>|
|<span data-ttu-id="b7f86-147">Нонкомплианткаунт</span><span class="sxs-lookup"><span data-stu-id="b7f86-147">nonCompliantCount</span></span>|<span data-ttu-id="b7f86-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f86-148">Int32</span></span>|<span data-ttu-id="b7f86-149">Количество устройств, не соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="b7f86-149">Number of non compliant devices</span></span>|
|<span data-ttu-id="b7f86-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b7f86-150">notApplicableCount</span></span>|<span data-ttu-id="b7f86-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f86-151">Int32</span></span>|<span data-ttu-id="b7f86-152">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="b7f86-152">Number of not applicable devices</span></span>|
|<span data-ttu-id="b7f86-153">Ремедиатедкаунт</span><span class="sxs-lookup"><span data-stu-id="b7f86-153">remediatedCount</span></span>|<span data-ttu-id="b7f86-154">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f86-154">Int32</span></span>|<span data-ttu-id="b7f86-155">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="b7f86-155">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="b7f86-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7f86-156">Response</span></span>
<span data-ttu-id="b7f86-157">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7f86-157">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7f86-158">Пример</span><span class="sxs-lookup"><span data-stu-id="b7f86-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7f86-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7f86-159">Request</span></span>
<span data-ttu-id="b7f86-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7f86-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b7f86-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7f86-161">Response</span></span>
<span data-ttu-id="b7f86-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7f86-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






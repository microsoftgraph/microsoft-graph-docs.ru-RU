---
title: Update softwareUpdateStatusSummary
description: Обновление свойств объекта softwareUpdateStatusSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a5ccdbd9488d0fbac6408730aa9da2879cbe48e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986870"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="1fad7-103">Update softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="1fad7-103">Update softwareUpdateStatusSummary</span></span>

<span data-ttu-id="1fad7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fad7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fad7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fad7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fad7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1fad7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fad7-107">Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="1fad7-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fad7-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1fad7-108">Prerequisites</span></span>
<span data-ttu-id="1fad7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fad7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fad7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fad7-111">Permission type</span></span>|<span data-ttu-id="1fad7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fad7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fad7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fad7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fad7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fad7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1fad7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fad7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fad7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fad7-116">Not supported.</span></span>|
|<span data-ttu-id="1fad7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fad7-117">Application</span></span>|<span data-ttu-id="1fad7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fad7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fad7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fad7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="1fad7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1fad7-120">Request headers</span></span>
|<span data-ttu-id="1fad7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1fad7-121">Header</span></span>|<span data-ttu-id="1fad7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1fad7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fad7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fad7-123">Authorization</span></span>|<span data-ttu-id="1fad7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fad7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fad7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1fad7-125">Accept</span></span>|<span data-ttu-id="1fad7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fad7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fad7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1fad7-127">Request body</span></span>
<span data-ttu-id="1fad7-128">В теле запроса добавьте представление объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fad7-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="1fad7-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="1fad7-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="1fad7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fad7-130">Property</span></span>|<span data-ttu-id="1fad7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1fad7-131">Type</span></span>|<span data-ttu-id="1fad7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1fad7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fad7-133">id</span><span class="sxs-lookup"><span data-stu-id="1fad7-133">id</span></span>|<span data-ttu-id="1fad7-134">String</span><span class="sxs-lookup"><span data-stu-id="1fad7-134">String</span></span>|<span data-ttu-id="1fad7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1fad7-135">Key of the entity.</span></span>|
|<span data-ttu-id="1fad7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1fad7-136">displayName</span></span>|<span data-ttu-id="1fad7-137">String</span><span class="sxs-lookup"><span data-stu-id="1fad7-137">String</span></span>|<span data-ttu-id="1fad7-138">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="1fad7-138">The name of the policy.</span></span>|
|<span data-ttu-id="1fad7-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-139">compliantDeviceCount</span></span>|<span data-ttu-id="1fad7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-140">Int32</span></span>|<span data-ttu-id="1fad7-141">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="1fad7-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="1fad7-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="1fad7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-143">Int32</span></span>|<span data-ttu-id="1fad7-144">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="1fad7-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="1fad7-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-145">remediatedDeviceCount</span></span>|<span data-ttu-id="1fad7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-146">Int32</span></span>|<span data-ttu-id="1fad7-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="1fad7-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="1fad7-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-148">errorDeviceCount</span></span>|<span data-ttu-id="1fad7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-149">Int32</span></span>|<span data-ttu-id="1fad7-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="1fad7-150">Number of devices had error.</span></span>|
|<span data-ttu-id="1fad7-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-151">unknownDeviceCount</span></span>|<span data-ttu-id="1fad7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-152">Int32</span></span>|<span data-ttu-id="1fad7-153">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="1fad7-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="1fad7-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-154">conflictDeviceCount</span></span>|<span data-ttu-id="1fad7-155">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-155">Int32</span></span>|<span data-ttu-id="1fad7-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="1fad7-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="1fad7-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="1fad7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-158">Int32</span></span>|<span data-ttu-id="1fad7-159">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="1fad7-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="1fad7-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-160">compliantUserCount</span></span>|<span data-ttu-id="1fad7-161">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-161">Int32</span></span>|<span data-ttu-id="1fad7-162">Количество пользователей, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="1fad7-162">Number of compliant users.</span></span>|
|<span data-ttu-id="1fad7-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-163">nonCompliantUserCount</span></span>|<span data-ttu-id="1fad7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-164">Int32</span></span>|<span data-ttu-id="1fad7-165">Количество пользователей, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="1fad7-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="1fad7-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-166">remediatedUserCount</span></span>|<span data-ttu-id="1fad7-167">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-167">Int32</span></span>|<span data-ttu-id="1fad7-168">Количество исправленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="1fad7-168">Number of remediated users.</span></span>|
|<span data-ttu-id="1fad7-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-169">errorUserCount</span></span>|<span data-ttu-id="1fad7-170">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-170">Int32</span></span>|<span data-ttu-id="1fad7-171">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="1fad7-171">Number of users had error.</span></span>|
|<span data-ttu-id="1fad7-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-172">unknownUserCount</span></span>|<span data-ttu-id="1fad7-173">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-173">Int32</span></span>|<span data-ttu-id="1fad7-174">Количество неизвестных пользователей.</span><span class="sxs-lookup"><span data-stu-id="1fad7-174">Number of unknown users.</span></span>|
|<span data-ttu-id="1fad7-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-175">conflictUserCount</span></span>|<span data-ttu-id="1fad7-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-176">Int32</span></span>|<span data-ttu-id="1fad7-177">Количество конфликтующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="1fad7-177">Number of conflict users.</span></span>|
|<span data-ttu-id="1fad7-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="1fad7-178">notApplicableUserCount</span></span>|<span data-ttu-id="1fad7-179">Int32</span><span class="sxs-lookup"><span data-stu-id="1fad7-179">Int32</span></span>|<span data-ttu-id="1fad7-180">Количество неприменимых пользователей.</span><span class="sxs-lookup"><span data-stu-id="1fad7-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="1fad7-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="1fad7-181">Response</span></span>
<span data-ttu-id="1fad7-182">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1fad7-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fad7-183">Пример</span><span class="sxs-lookup"><span data-stu-id="1fad7-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fad7-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fad7-184">Request</span></span>
<span data-ttu-id="1fad7-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fad7-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

### <a name="response"></a><span data-ttu-id="1fad7-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fad7-186">Response</span></span>
<span data-ttu-id="1fad7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fad7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```







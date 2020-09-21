---
title: Update softwareUpdateStatusSummary
description: Обновление свойств объекта softwareUpdateStatusSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2b052b2a1a4dd7ca75a4151251ce079248bce87
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968159"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="dabb6-103">Update softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="dabb6-103">Update softwareUpdateStatusSummary</span></span>

<span data-ttu-id="dabb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dabb6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dabb6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dabb6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dabb6-106">Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="dabb6-106">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dabb6-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dabb6-107">Prerequisites</span></span>
<span data-ttu-id="dabb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dabb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dabb6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dabb6-110">Permission type</span></span>|<span data-ttu-id="dabb6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dabb6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dabb6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dabb6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dabb6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dabb6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dabb6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dabb6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dabb6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dabb6-115">Not supported.</span></span>|
|<span data-ttu-id="dabb6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dabb6-116">Application</span></span>|<span data-ttu-id="dabb6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dabb6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dabb6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dabb6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="dabb6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dabb6-119">Request headers</span></span>
|<span data-ttu-id="dabb6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dabb6-120">Header</span></span>|<span data-ttu-id="dabb6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dabb6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dabb6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dabb6-122">Authorization</span></span>|<span data-ttu-id="dabb6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dabb6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dabb6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dabb6-124">Accept</span></span>|<span data-ttu-id="dabb6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dabb6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dabb6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dabb6-126">Request body</span></span>
<span data-ttu-id="dabb6-127">В теле запроса добавьте представление объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dabb6-127">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="dabb6-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="dabb6-128">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="dabb6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dabb6-129">Property</span></span>|<span data-ttu-id="dabb6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dabb6-130">Type</span></span>|<span data-ttu-id="dabb6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dabb6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dabb6-132">id</span><span class="sxs-lookup"><span data-stu-id="dabb6-132">id</span></span>|<span data-ttu-id="dabb6-133">String</span><span class="sxs-lookup"><span data-stu-id="dabb6-133">String</span></span>|<span data-ttu-id="dabb6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dabb6-134">Key of the entity.</span></span>|
|<span data-ttu-id="dabb6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="dabb6-135">displayName</span></span>|<span data-ttu-id="dabb6-136">String</span><span class="sxs-lookup"><span data-stu-id="dabb6-136">String</span></span>|<span data-ttu-id="dabb6-137">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="dabb6-137">The name of the policy.</span></span>|
|<span data-ttu-id="dabb6-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-138">compliantDeviceCount</span></span>|<span data-ttu-id="dabb6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-139">Int32</span></span>|<span data-ttu-id="dabb6-140">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="dabb6-140">Number of compliant devices.</span></span>|
|<span data-ttu-id="dabb6-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="dabb6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-142">Int32</span></span>|<span data-ttu-id="dabb6-143">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="dabb6-143">Number of non compliant devices.</span></span>|
|<span data-ttu-id="dabb6-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-144">remediatedDeviceCount</span></span>|<span data-ttu-id="dabb6-145">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-145">Int32</span></span>|<span data-ttu-id="dabb6-146">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="dabb6-146">Number of remediated devices.</span></span>|
|<span data-ttu-id="dabb6-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-147">errorDeviceCount</span></span>|<span data-ttu-id="dabb6-148">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-148">Int32</span></span>|<span data-ttu-id="dabb6-149">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="dabb6-149">Number of devices had error.</span></span>|
|<span data-ttu-id="dabb6-150">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-150">unknownDeviceCount</span></span>|<span data-ttu-id="dabb6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-151">Int32</span></span>|<span data-ttu-id="dabb6-152">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="dabb6-152">Number of unknown devices.</span></span>|
|<span data-ttu-id="dabb6-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-153">conflictDeviceCount</span></span>|<span data-ttu-id="dabb6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-154">Int32</span></span>|<span data-ttu-id="dabb6-155">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="dabb6-155">Number of conflict devices.</span></span>|
|<span data-ttu-id="dabb6-156">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-156">notApplicableDeviceCount</span></span>|<span data-ttu-id="dabb6-157">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-157">Int32</span></span>|<span data-ttu-id="dabb6-158">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="dabb6-158">Number of not applicable devices.</span></span>|
|<span data-ttu-id="dabb6-159">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-159">compliantUserCount</span></span>|<span data-ttu-id="dabb6-160">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-160">Int32</span></span>|<span data-ttu-id="dabb6-161">Количество пользователей, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="dabb6-161">Number of compliant users.</span></span>|
|<span data-ttu-id="dabb6-162">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-162">nonCompliantUserCount</span></span>|<span data-ttu-id="dabb6-163">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-163">Int32</span></span>|<span data-ttu-id="dabb6-164">Количество пользователей, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="dabb6-164">Number of non compliant users.</span></span>|
|<span data-ttu-id="dabb6-165">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-165">remediatedUserCount</span></span>|<span data-ttu-id="dabb6-166">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-166">Int32</span></span>|<span data-ttu-id="dabb6-167">Количество исправленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="dabb6-167">Number of remediated users.</span></span>|
|<span data-ttu-id="dabb6-168">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-168">errorUserCount</span></span>|<span data-ttu-id="dabb6-169">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-169">Int32</span></span>|<span data-ttu-id="dabb6-170">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="dabb6-170">Number of users had error.</span></span>|
|<span data-ttu-id="dabb6-171">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-171">unknownUserCount</span></span>|<span data-ttu-id="dabb6-172">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-172">Int32</span></span>|<span data-ttu-id="dabb6-173">Количество неизвестных пользователей.</span><span class="sxs-lookup"><span data-stu-id="dabb6-173">Number of unknown users.</span></span>|
|<span data-ttu-id="dabb6-174">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-174">conflictUserCount</span></span>|<span data-ttu-id="dabb6-175">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-175">Int32</span></span>|<span data-ttu-id="dabb6-176">Количество конфликтующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="dabb6-176">Number of conflict users.</span></span>|
|<span data-ttu-id="dabb6-177">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="dabb6-177">notApplicableUserCount</span></span>|<span data-ttu-id="dabb6-178">Int32</span><span class="sxs-lookup"><span data-stu-id="dabb6-178">Int32</span></span>|<span data-ttu-id="dabb6-179">Количество неприменимых пользователей.</span><span class="sxs-lookup"><span data-stu-id="dabb6-179">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="dabb6-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="dabb6-180">Response</span></span>
<span data-ttu-id="dabb6-181">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dabb6-181">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dabb6-182">Пример</span><span class="sxs-lookup"><span data-stu-id="dabb6-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="dabb6-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="dabb6-183">Request</span></span>
<span data-ttu-id="dabb6-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dabb6-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
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

### <a name="response"></a><span data-ttu-id="dabb6-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="dabb6-185">Response</span></span>
<span data-ttu-id="dabb6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dabb6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










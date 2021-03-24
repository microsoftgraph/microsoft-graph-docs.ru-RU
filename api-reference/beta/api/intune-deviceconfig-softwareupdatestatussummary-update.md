---
title: Update softwareUpdateStatusSummary
description: Обновление свойств объекта softwareUpdateStatusSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a35c52de0da15a20c4607ae7626f9c989795a41d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137058"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="3ca45-103">Update softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="3ca45-103">Update softwareUpdateStatusSummary</span></span>

<span data-ttu-id="3ca45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ca45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ca45-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ca45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ca45-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ca45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ca45-107">Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="3ca45-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ca45-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3ca45-108">Prerequisites</span></span>
<span data-ttu-id="3ca45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ca45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ca45-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ca45-111">Permission type</span></span>|<span data-ttu-id="3ca45-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ca45-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ca45-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ca45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ca45-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ca45-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3ca45-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ca45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ca45-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ca45-116">Not supported.</span></span>|
|<span data-ttu-id="3ca45-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3ca45-117">Application</span></span>|<span data-ttu-id="3ca45-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ca45-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ca45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ca45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="3ca45-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3ca45-120">Request headers</span></span>
|<span data-ttu-id="3ca45-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ca45-121">Header</span></span>|<span data-ttu-id="3ca45-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3ca45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ca45-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ca45-123">Authorization</span></span>|<span data-ttu-id="3ca45-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ca45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ca45-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3ca45-125">Accept</span></span>|<span data-ttu-id="3ca45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ca45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ca45-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ca45-127">Request body</span></span>
<span data-ttu-id="3ca45-128">В теле запроса добавьте представление объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ca45-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="3ca45-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="3ca45-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="3ca45-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ca45-130">Property</span></span>|<span data-ttu-id="3ca45-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3ca45-131">Type</span></span>|<span data-ttu-id="3ca45-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3ca45-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ca45-133">id</span><span class="sxs-lookup"><span data-stu-id="3ca45-133">id</span></span>|<span data-ttu-id="3ca45-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3ca45-134">String</span></span>|<span data-ttu-id="3ca45-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3ca45-135">Key of the entity.</span></span>|
|<span data-ttu-id="3ca45-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3ca45-136">displayName</span></span>|<span data-ttu-id="3ca45-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3ca45-137">String</span></span>|<span data-ttu-id="3ca45-138">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="3ca45-138">The name of the policy.</span></span>|
|<span data-ttu-id="3ca45-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-139">compliantDeviceCount</span></span>|<span data-ttu-id="3ca45-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-140">Int32</span></span>|<span data-ttu-id="3ca45-141">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="3ca45-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="3ca45-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="3ca45-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-143">Int32</span></span>|<span data-ttu-id="3ca45-144">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="3ca45-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="3ca45-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-145">remediatedDeviceCount</span></span>|<span data-ttu-id="3ca45-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-146">Int32</span></span>|<span data-ttu-id="3ca45-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="3ca45-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="3ca45-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-148">errorDeviceCount</span></span>|<span data-ttu-id="3ca45-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-149">Int32</span></span>|<span data-ttu-id="3ca45-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="3ca45-150">Number of devices had error.</span></span>|
|<span data-ttu-id="3ca45-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-151">unknownDeviceCount</span></span>|<span data-ttu-id="3ca45-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-152">Int32</span></span>|<span data-ttu-id="3ca45-153">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="3ca45-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="3ca45-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-154">conflictDeviceCount</span></span>|<span data-ttu-id="3ca45-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-155">Int32</span></span>|<span data-ttu-id="3ca45-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="3ca45-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="3ca45-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="3ca45-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-158">Int32</span></span>|<span data-ttu-id="3ca45-159">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="3ca45-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="3ca45-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-160">compliantUserCount</span></span>|<span data-ttu-id="3ca45-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-161">Int32</span></span>|<span data-ttu-id="3ca45-162">Количество пользователей, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="3ca45-162">Number of compliant users.</span></span>|
|<span data-ttu-id="3ca45-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-163">nonCompliantUserCount</span></span>|<span data-ttu-id="3ca45-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-164">Int32</span></span>|<span data-ttu-id="3ca45-165">Количество пользователей, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="3ca45-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="3ca45-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-166">remediatedUserCount</span></span>|<span data-ttu-id="3ca45-167">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-167">Int32</span></span>|<span data-ttu-id="3ca45-168">Количество исправленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="3ca45-168">Number of remediated users.</span></span>|
|<span data-ttu-id="3ca45-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-169">errorUserCount</span></span>|<span data-ttu-id="3ca45-170">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-170">Int32</span></span>|<span data-ttu-id="3ca45-171">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="3ca45-171">Number of users had error.</span></span>|
|<span data-ttu-id="3ca45-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-172">unknownUserCount</span></span>|<span data-ttu-id="3ca45-173">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-173">Int32</span></span>|<span data-ttu-id="3ca45-174">Количество неизвестных пользователей.</span><span class="sxs-lookup"><span data-stu-id="3ca45-174">Number of unknown users.</span></span>|
|<span data-ttu-id="3ca45-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-175">conflictUserCount</span></span>|<span data-ttu-id="3ca45-176">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-176">Int32</span></span>|<span data-ttu-id="3ca45-177">Количество конфликтующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="3ca45-177">Number of conflict users.</span></span>|
|<span data-ttu-id="3ca45-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="3ca45-178">notApplicableUserCount</span></span>|<span data-ttu-id="3ca45-179">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca45-179">Int32</span></span>|<span data-ttu-id="3ca45-180">Количество неприменимых пользователей.</span><span class="sxs-lookup"><span data-stu-id="3ca45-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="3ca45-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ca45-181">Response</span></span>
<span data-ttu-id="3ca45-182">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3ca45-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ca45-183">Пример</span><span class="sxs-lookup"><span data-stu-id="3ca45-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ca45-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ca45-184">Request</span></span>
<span data-ttu-id="3ca45-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ca45-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3ca45-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ca45-186">Response</span></span>
<span data-ttu-id="3ca45-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ca45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





---
title: Update softwareUpdateStatusSummary
description: Обновление свойств объекта softwareUpdateStatusSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8a3ceff462e9e2ee32ec1a7a32b3b1f5dd129b41
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734975"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="f9823-103">Update softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="f9823-103">Update softwareUpdateStatusSummary</span></span>

<span data-ttu-id="f9823-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9823-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9823-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9823-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9823-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9823-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9823-107">Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="f9823-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9823-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f9823-108">Prerequisites</span></span>
<span data-ttu-id="f9823-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9823-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9823-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9823-111">Permission type</span></span>|<span data-ttu-id="f9823-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9823-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9823-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9823-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9823-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9823-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9823-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9823-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9823-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9823-116">Not supported.</span></span>|
|<span data-ttu-id="f9823-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9823-117">Application</span></span>|<span data-ttu-id="f9823-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9823-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9823-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9823-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="f9823-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f9823-120">Request headers</span></span>
|<span data-ttu-id="f9823-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9823-121">Header</span></span>|<span data-ttu-id="f9823-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f9823-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9823-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9823-123">Authorization</span></span>|<span data-ttu-id="f9823-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9823-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9823-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f9823-125">Accept</span></span>|<span data-ttu-id="f9823-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9823-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9823-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f9823-127">Request body</span></span>
<span data-ttu-id="f9823-128">В теле запроса добавьте представление объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9823-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="f9823-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="f9823-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="f9823-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9823-130">Property</span></span>|<span data-ttu-id="f9823-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f9823-131">Type</span></span>|<span data-ttu-id="f9823-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f9823-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9823-133">id</span><span class="sxs-lookup"><span data-stu-id="f9823-133">id</span></span>|<span data-ttu-id="f9823-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f9823-134">String</span></span>|<span data-ttu-id="f9823-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f9823-135">Key of the entity.</span></span>|
|<span data-ttu-id="f9823-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f9823-136">displayName</span></span>|<span data-ttu-id="f9823-137">Строка</span><span class="sxs-lookup"><span data-stu-id="f9823-137">String</span></span>|<span data-ttu-id="f9823-138">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="f9823-138">The name of the policy.</span></span>|
|<span data-ttu-id="f9823-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9823-139">compliantDeviceCount</span></span>|<span data-ttu-id="f9823-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-140">Int32</span></span>|<span data-ttu-id="f9823-141">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="f9823-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="f9823-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9823-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f9823-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-143">Int32</span></span>|<span data-ttu-id="f9823-144">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="f9823-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="f9823-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9823-145">remediatedDeviceCount</span></span>|<span data-ttu-id="f9823-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-146">Int32</span></span>|<span data-ttu-id="f9823-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="f9823-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="f9823-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9823-148">errorDeviceCount</span></span>|<span data-ttu-id="f9823-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-149">Int32</span></span>|<span data-ttu-id="f9823-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="f9823-150">Number of devices had error.</span></span>|
|<span data-ttu-id="f9823-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9823-151">unknownDeviceCount</span></span>|<span data-ttu-id="f9823-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-152">Int32</span></span>|<span data-ttu-id="f9823-153">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="f9823-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="f9823-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9823-154">conflictDeviceCount</span></span>|<span data-ttu-id="f9823-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-155">Int32</span></span>|<span data-ttu-id="f9823-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="f9823-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="f9823-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9823-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="f9823-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-158">Int32</span></span>|<span data-ttu-id="f9823-159">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="f9823-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="f9823-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="f9823-160">compliantUserCount</span></span>|<span data-ttu-id="f9823-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-161">Int32</span></span>|<span data-ttu-id="f9823-162">Количество пользователей, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="f9823-162">Number of compliant users.</span></span>|
|<span data-ttu-id="f9823-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="f9823-163">nonCompliantUserCount</span></span>|<span data-ttu-id="f9823-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-164">Int32</span></span>|<span data-ttu-id="f9823-165">Количество пользователей, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="f9823-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="f9823-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="f9823-166">remediatedUserCount</span></span>|<span data-ttu-id="f9823-167">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-167">Int32</span></span>|<span data-ttu-id="f9823-168">Количество исправленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f9823-168">Number of remediated users.</span></span>|
|<span data-ttu-id="f9823-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="f9823-169">errorUserCount</span></span>|<span data-ttu-id="f9823-170">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-170">Int32</span></span>|<span data-ttu-id="f9823-171">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="f9823-171">Number of users had error.</span></span>|
|<span data-ttu-id="f9823-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="f9823-172">unknownUserCount</span></span>|<span data-ttu-id="f9823-173">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-173">Int32</span></span>|<span data-ttu-id="f9823-174">Количество неизвестных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f9823-174">Number of unknown users.</span></span>|
|<span data-ttu-id="f9823-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="f9823-175">conflictUserCount</span></span>|<span data-ttu-id="f9823-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-176">Int32</span></span>|<span data-ttu-id="f9823-177">Количество конфликтующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="f9823-177">Number of conflict users.</span></span>|
|<span data-ttu-id="f9823-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="f9823-178">notApplicableUserCount</span></span>|<span data-ttu-id="f9823-179">Int32</span><span class="sxs-lookup"><span data-stu-id="f9823-179">Int32</span></span>|<span data-ttu-id="f9823-180">Количество неприменимых пользователей.</span><span class="sxs-lookup"><span data-stu-id="f9823-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="f9823-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9823-181">Response</span></span>
<span data-ttu-id="f9823-182">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f9823-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9823-183">Пример</span><span class="sxs-lookup"><span data-stu-id="f9823-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9823-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9823-184">Request</span></span>
<span data-ttu-id="f9823-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9823-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9823-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9823-186">Response</span></span>
<span data-ttu-id="f9823-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9823-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






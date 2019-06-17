---
title: Update softwareUpdateStatusSummary
description: Обновление свойств объекта softwareUpdateStatusSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dca339e9b9ca29635d5b31bbd631488b0ecd1f87
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962808"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="c56f2-103">Update softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="c56f2-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="c56f2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c56f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c56f2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c56f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c56f2-106">Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="c56f2-106">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c56f2-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c56f2-107">Prerequisites</span></span>
<span data-ttu-id="c56f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c56f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c56f2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c56f2-110">Permission type</span></span>|<span data-ttu-id="c56f2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c56f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c56f2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c56f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c56f2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c56f2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c56f2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c56f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c56f2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c56f2-115">Not supported.</span></span>|
|<span data-ttu-id="c56f2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c56f2-116">Application</span></span>|<span data-ttu-id="c56f2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c56f2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c56f2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c56f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="c56f2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c56f2-119">Request headers</span></span>
|<span data-ttu-id="c56f2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c56f2-120">Header</span></span>|<span data-ttu-id="c56f2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c56f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c56f2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c56f2-122">Authorization</span></span>|<span data-ttu-id="c56f2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c56f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c56f2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c56f2-124">Accept</span></span>|<span data-ttu-id="c56f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c56f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c56f2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c56f2-126">Request body</span></span>
<span data-ttu-id="c56f2-127">В теле запроса добавьте представление объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c56f2-127">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="c56f2-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="c56f2-128">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="c56f2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c56f2-129">Property</span></span>|<span data-ttu-id="c56f2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c56f2-130">Type</span></span>|<span data-ttu-id="c56f2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c56f2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c56f2-132">id</span><span class="sxs-lookup"><span data-stu-id="c56f2-132">id</span></span>|<span data-ttu-id="c56f2-133">String</span><span class="sxs-lookup"><span data-stu-id="c56f2-133">String</span></span>|<span data-ttu-id="c56f2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c56f2-134">Key of the entity.</span></span>|
|<span data-ttu-id="c56f2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c56f2-135">displayName</span></span>|<span data-ttu-id="c56f2-136">Строка</span><span class="sxs-lookup"><span data-stu-id="c56f2-136">String</span></span>|<span data-ttu-id="c56f2-137">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="c56f2-137">The name of the policy.</span></span>|
|<span data-ttu-id="c56f2-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-138">compliantDeviceCount</span></span>|<span data-ttu-id="c56f2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-139">Int32</span></span>|<span data-ttu-id="c56f2-140">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="c56f2-140">Number of compliant devices.</span></span>|
|<span data-ttu-id="c56f2-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c56f2-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-142">Int32</span></span>|<span data-ttu-id="c56f2-143">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="c56f2-143">Number of non compliant devices.</span></span>|
|<span data-ttu-id="c56f2-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-144">remediatedDeviceCount</span></span>|<span data-ttu-id="c56f2-145">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-145">Int32</span></span>|<span data-ttu-id="c56f2-146">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="c56f2-146">Number of remediated devices.</span></span>|
|<span data-ttu-id="c56f2-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-147">errorDeviceCount</span></span>|<span data-ttu-id="c56f2-148">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-148">Int32</span></span>|<span data-ttu-id="c56f2-149">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="c56f2-149">Number of devices had error.</span></span>|
|<span data-ttu-id="c56f2-150">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-150">unknownDeviceCount</span></span>|<span data-ttu-id="c56f2-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-151">Int32</span></span>|<span data-ttu-id="c56f2-152">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="c56f2-152">Number of unknown devices.</span></span>|
|<span data-ttu-id="c56f2-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-153">conflictDeviceCount</span></span>|<span data-ttu-id="c56f2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-154">Int32</span></span>|<span data-ttu-id="c56f2-155">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="c56f2-155">Number of conflict devices.</span></span>|
|<span data-ttu-id="c56f2-156">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-156">notApplicableDeviceCount</span></span>|<span data-ttu-id="c56f2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-157">Int32</span></span>|<span data-ttu-id="c56f2-158">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="c56f2-158">Number of not applicable devices.</span></span>|
|<span data-ttu-id="c56f2-159">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-159">compliantUserCount</span></span>|<span data-ttu-id="c56f2-160">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-160">Int32</span></span>|<span data-ttu-id="c56f2-161">Количество пользователей, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="c56f2-161">Number of compliant users.</span></span>|
|<span data-ttu-id="c56f2-162">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-162">nonCompliantUserCount</span></span>|<span data-ttu-id="c56f2-163">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-163">Int32</span></span>|<span data-ttu-id="c56f2-164">Количество пользователей, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="c56f2-164">Number of non compliant users.</span></span>|
|<span data-ttu-id="c56f2-165">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-165">remediatedUserCount</span></span>|<span data-ttu-id="c56f2-166">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-166">Int32</span></span>|<span data-ttu-id="c56f2-167">Количество исправленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="c56f2-167">Number of remediated users.</span></span>|
|<span data-ttu-id="c56f2-168">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-168">errorUserCount</span></span>|<span data-ttu-id="c56f2-169">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-169">Int32</span></span>|<span data-ttu-id="c56f2-170">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="c56f2-170">Number of users had error.</span></span>|
|<span data-ttu-id="c56f2-171">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-171">unknownUserCount</span></span>|<span data-ttu-id="c56f2-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-172">Int32</span></span>|<span data-ttu-id="c56f2-173">Количество неизвестных пользователей.</span><span class="sxs-lookup"><span data-stu-id="c56f2-173">Number of unknown users.</span></span>|
|<span data-ttu-id="c56f2-174">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-174">conflictUserCount</span></span>|<span data-ttu-id="c56f2-175">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-175">Int32</span></span>|<span data-ttu-id="c56f2-176">Количество конфликтующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="c56f2-176">Number of conflict users.</span></span>|
|<span data-ttu-id="c56f2-177">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="c56f2-177">notApplicableUserCount</span></span>|<span data-ttu-id="c56f2-178">Int32</span><span class="sxs-lookup"><span data-stu-id="c56f2-178">Int32</span></span>|<span data-ttu-id="c56f2-179">Количество неприменимых пользователей.</span><span class="sxs-lookup"><span data-stu-id="c56f2-179">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="c56f2-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="c56f2-180">Response</span></span>
<span data-ttu-id="c56f2-181">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c56f2-181">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c56f2-182">Пример</span><span class="sxs-lookup"><span data-stu-id="c56f2-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="c56f2-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="c56f2-183">Request</span></span>
<span data-ttu-id="c56f2-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c56f2-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c56f2-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="c56f2-185">Response</span></span>
<span data-ttu-id="c56f2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c56f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






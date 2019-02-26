---
title: Update softwareUpdateStatusSummary
description: Обновление свойств объекта softwareUpdateStatusSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76475402e0bb240606cfff0ed25b4502b2feb206
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145096"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="6be8b-103">Update softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="6be8b-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="6be8b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6be8b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6be8b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6be8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6be8b-106">Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="6be8b-106">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6be8b-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6be8b-107">Prerequisites</span></span>
<span data-ttu-id="6be8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6be8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6be8b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6be8b-110">Permission type</span></span>|<span data-ttu-id="6be8b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6be8b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6be8b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6be8b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6be8b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6be8b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6be8b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6be8b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6be8b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6be8b-115">Not supported.</span></span>|
|<span data-ttu-id="6be8b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6be8b-116">Application</span></span>|<span data-ttu-id="6be8b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6be8b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6be8b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6be8b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="6be8b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6be8b-119">Request headers</span></span>
|<span data-ttu-id="6be8b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6be8b-120">Header</span></span>|<span data-ttu-id="6be8b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6be8b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6be8b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6be8b-122">Authorization</span></span>|<span data-ttu-id="6be8b-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6be8b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6be8b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6be8b-124">Accept</span></span>|<span data-ttu-id="6be8b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6be8b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6be8b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6be8b-126">Request body</span></span>
<span data-ttu-id="6be8b-127">В теле запроса добавьте представление объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6be8b-127">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="6be8b-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="6be8b-128">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="6be8b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6be8b-129">Property</span></span>|<span data-ttu-id="6be8b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6be8b-130">Type</span></span>|<span data-ttu-id="6be8b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6be8b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6be8b-132">id</span><span class="sxs-lookup"><span data-stu-id="6be8b-132">id</span></span>|<span data-ttu-id="6be8b-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6be8b-133">String</span></span>|<span data-ttu-id="6be8b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6be8b-134">Key of the entity.</span></span>|
|<span data-ttu-id="6be8b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6be8b-135">displayName</span></span>|<span data-ttu-id="6be8b-136">String</span><span class="sxs-lookup"><span data-stu-id="6be8b-136">String</span></span>|<span data-ttu-id="6be8b-137">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="6be8b-137">The name of the policy.</span></span>|
|<span data-ttu-id="6be8b-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-138">compliantDeviceCount</span></span>|<span data-ttu-id="6be8b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-139">Int32</span></span>|<span data-ttu-id="6be8b-140">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="6be8b-140">Number of compliant devices.</span></span>|
|<span data-ttu-id="6be8b-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="6be8b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-142">Int32</span></span>|<span data-ttu-id="6be8b-143">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="6be8b-143">Number of non compliant devices.</span></span>|
|<span data-ttu-id="6be8b-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-144">remediatedDeviceCount</span></span>|<span data-ttu-id="6be8b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-145">Int32</span></span>|<span data-ttu-id="6be8b-146">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="6be8b-146">Number of remediated devices.</span></span>|
|<span data-ttu-id="6be8b-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-147">errorDeviceCount</span></span>|<span data-ttu-id="6be8b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-148">Int32</span></span>|<span data-ttu-id="6be8b-149">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="6be8b-149">Number of devices had error.</span></span>|
|<span data-ttu-id="6be8b-150">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-150">unknownDeviceCount</span></span>|<span data-ttu-id="6be8b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-151">Int32</span></span>|<span data-ttu-id="6be8b-152">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="6be8b-152">Number of unknown devices.</span></span>|
|<span data-ttu-id="6be8b-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-153">conflictDeviceCount</span></span>|<span data-ttu-id="6be8b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-154">Int32</span></span>|<span data-ttu-id="6be8b-155">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="6be8b-155">Number of conflict devices.</span></span>|
|<span data-ttu-id="6be8b-156">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-156">notApplicableDeviceCount</span></span>|<span data-ttu-id="6be8b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-157">Int32</span></span>|<span data-ttu-id="6be8b-158">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="6be8b-158">Number of not applicable devices.</span></span>|
|<span data-ttu-id="6be8b-159">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-159">compliantUserCount</span></span>|<span data-ttu-id="6be8b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-160">Int32</span></span>|<span data-ttu-id="6be8b-161">Количество пользователей, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="6be8b-161">Number of compliant users.</span></span>|
|<span data-ttu-id="6be8b-162">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-162">nonCompliantUserCount</span></span>|<span data-ttu-id="6be8b-163">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-163">Int32</span></span>|<span data-ttu-id="6be8b-164">Количество пользователей, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="6be8b-164">Number of non compliant users.</span></span>|
|<span data-ttu-id="6be8b-165">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-165">remediatedUserCount</span></span>|<span data-ttu-id="6be8b-166">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-166">Int32</span></span>|<span data-ttu-id="6be8b-167">Количество исправленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6be8b-167">Number of remediated users.</span></span>|
|<span data-ttu-id="6be8b-168">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-168">errorUserCount</span></span>|<span data-ttu-id="6be8b-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-169">Int32</span></span>|<span data-ttu-id="6be8b-170">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="6be8b-170">Number of users had error.</span></span>|
|<span data-ttu-id="6be8b-171">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-171">unknownUserCount</span></span>|<span data-ttu-id="6be8b-172">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-172">Int32</span></span>|<span data-ttu-id="6be8b-173">Количество неизвестных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6be8b-173">Number of unknown users.</span></span>|
|<span data-ttu-id="6be8b-174">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-174">conflictUserCount</span></span>|<span data-ttu-id="6be8b-175">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-175">Int32</span></span>|<span data-ttu-id="6be8b-176">Количество конфликтующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="6be8b-176">Number of conflict users.</span></span>|
|<span data-ttu-id="6be8b-177">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="6be8b-177">notApplicableUserCount</span></span>|<span data-ttu-id="6be8b-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6be8b-178">Int32</span></span>|<span data-ttu-id="6be8b-179">Количество неприменимых пользователей.</span><span class="sxs-lookup"><span data-stu-id="6be8b-179">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="6be8b-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="6be8b-180">Response</span></span>
<span data-ttu-id="6be8b-181">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6be8b-181">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6be8b-182">Пример</span><span class="sxs-lookup"><span data-stu-id="6be8b-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="6be8b-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="6be8b-183">Request</span></span>
<span data-ttu-id="6be8b-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6be8b-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6be8b-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="6be8b-185">Response</span></span>
<span data-ttu-id="6be8b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6be8b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





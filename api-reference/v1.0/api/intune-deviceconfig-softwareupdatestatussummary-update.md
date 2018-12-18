---
title: Update softwareUpdateStatusSummary
description: Обновление свойств объекта softwareUpdateStatusSummary.
author: tfitzmac
ms.openlocfilehash: a08efea3a4552e97b638336eb70165c16e58055a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317754"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="bbc6f-103">Update softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="bbc6f-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="bbc6f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbc6f-105">Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="bbc6f-105">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bbc6f-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bbc6f-106">Prerequisites</span></span>
<span data-ttu-id="bbc6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbc6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbc6f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbc6f-109">Permission type</span></span>|<span data-ttu-id="bbc6f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbc6f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbc6f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbc6f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bbc6f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbc6f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bbc6f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbc6f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbc6f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-114">Not supported.</span></span>|
|<span data-ttu-id="bbc6f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbc6f-115">Application</span></span>|<span data-ttu-id="bbc6f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbc6f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbc6f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="bbc6f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbc6f-118">Request headers</span></span>
|<span data-ttu-id="bbc6f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bbc6f-119">Header</span></span>|<span data-ttu-id="bbc6f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bbc6f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbc6f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbc6f-121">Authorization</span></span>|<span data-ttu-id="bbc6f-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bbc6f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbc6f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bbc6f-123">Accept</span></span>|<span data-ttu-id="bbc6f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bbc6f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbc6f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bbc6f-125">Request body</span></span>
<span data-ttu-id="bbc6f-126">В теле запроса добавьте представление объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-126">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="bbc6f-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="bbc6f-127">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="bbc6f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbc6f-128">Property</span></span>|<span data-ttu-id="bbc6f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bbc6f-129">Type</span></span>|<span data-ttu-id="bbc6f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bbc6f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbc6f-131">id</span><span class="sxs-lookup"><span data-stu-id="bbc6f-131">id</span></span>|<span data-ttu-id="bbc6f-132">Строка</span><span class="sxs-lookup"><span data-stu-id="bbc6f-132">String</span></span>|<span data-ttu-id="bbc6f-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-133">Key of the entity.</span></span>|
|<span data-ttu-id="bbc6f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="bbc6f-134">displayName</span></span>|<span data-ttu-id="bbc6f-135">String</span><span class="sxs-lookup"><span data-stu-id="bbc6f-135">String</span></span>|<span data-ttu-id="bbc6f-136">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-136">The name of the policy.</span></span>|
|<span data-ttu-id="bbc6f-137">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-137">compliantDeviceCount</span></span>|<span data-ttu-id="bbc6f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-138">Int32</span></span>|<span data-ttu-id="bbc6f-139">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-139">Number of compliant devices.</span></span>|
|<span data-ttu-id="bbc6f-140">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-140">nonCompliantDeviceCount</span></span>|<span data-ttu-id="bbc6f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-141">Int32</span></span>|<span data-ttu-id="bbc6f-142">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-142">Number of non compliant devices.</span></span>|
|<span data-ttu-id="bbc6f-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-143">remediatedDeviceCount</span></span>|<span data-ttu-id="bbc6f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-144">Int32</span></span>|<span data-ttu-id="bbc6f-145">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-145">Number of remediated devices.</span></span>|
|<span data-ttu-id="bbc6f-146">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-146">errorDeviceCount</span></span>|<span data-ttu-id="bbc6f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-147">Int32</span></span>|<span data-ttu-id="bbc6f-148">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-148">Number of devices had error.</span></span>|
|<span data-ttu-id="bbc6f-149">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-149">unknownDeviceCount</span></span>|<span data-ttu-id="bbc6f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-150">Int32</span></span>|<span data-ttu-id="bbc6f-151">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="bbc6f-151">Number of unknown devices.</span></span>|
|<span data-ttu-id="bbc6f-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-152">conflictDeviceCount</span></span>|<span data-ttu-id="bbc6f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-153">Int32</span></span>|<span data-ttu-id="bbc6f-154">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-154">Number of conflict devices.</span></span>|
|<span data-ttu-id="bbc6f-155">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-155">notApplicableDeviceCount</span></span>|<span data-ttu-id="bbc6f-156">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-156">Int32</span></span>|<span data-ttu-id="bbc6f-157">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-157">Number of not applicable devices.</span></span>|
|<span data-ttu-id="bbc6f-158">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-158">compliantUserCount</span></span>|<span data-ttu-id="bbc6f-159">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-159">Int32</span></span>|<span data-ttu-id="bbc6f-160">Количество пользователей, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-160">Number of compliant users.</span></span>|
|<span data-ttu-id="bbc6f-161">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-161">nonCompliantUserCount</span></span>|<span data-ttu-id="bbc6f-162">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-162">Int32</span></span>|<span data-ttu-id="bbc6f-163">Количество пользователей, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-163">Number of non compliant users.</span></span>|
|<span data-ttu-id="bbc6f-164">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-164">remediatedUserCount</span></span>|<span data-ttu-id="bbc6f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-165">Int32</span></span>|<span data-ttu-id="bbc6f-166">Количество исправленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-166">Number of remediated users.</span></span>|
|<span data-ttu-id="bbc6f-167">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-167">errorUserCount</span></span>|<span data-ttu-id="bbc6f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-168">Int32</span></span>|<span data-ttu-id="bbc6f-169">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-169">Number of users had error.</span></span>|
|<span data-ttu-id="bbc6f-170">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-170">unknownUserCount</span></span>|<span data-ttu-id="bbc6f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-171">Int32</span></span>|<span data-ttu-id="bbc6f-172">Количество неизвестных пользователей.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-172">Number of unknown users.</span></span>|
|<span data-ttu-id="bbc6f-173">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-173">conflictUserCount</span></span>|<span data-ttu-id="bbc6f-174">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-174">Int32</span></span>|<span data-ttu-id="bbc6f-175">Количество конфликтующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-175">Number of conflict users.</span></span>|
|<span data-ttu-id="bbc6f-176">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="bbc6f-176">notApplicableUserCount</span></span>|<span data-ttu-id="bbc6f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc6f-177">Int32</span></span>|<span data-ttu-id="bbc6f-178">Количество неприменимых пользователей.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-178">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="bbc6f-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="bbc6f-179">Response</span></span>
<span data-ttu-id="bbc6f-180">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-180">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbc6f-181">Пример</span><span class="sxs-lookup"><span data-stu-id="bbc6f-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="bbc6f-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbc6f-182">Request</span></span>
<span data-ttu-id="bbc6f-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bbc6f-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="bbc6f-184">Response</span></span>
<span data-ttu-id="bbc6f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bbc6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




---
title: Update softwareUpdateStatusSummary
description: Обновление свойств объекта softwareUpdateStatusSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c1437e55807e2fba92efb7dab3b908f8bae88487
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837298"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="0456b-103">Update softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="0456b-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="0456b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0456b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0456b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0456b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0456b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0456b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0456b-107">Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="0456b-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0456b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0456b-108">Prerequisites</span></span>
<span data-ttu-id="0456b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0456b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0456b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0456b-111">Permission type</span></span>|<span data-ttu-id="0456b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0456b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0456b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0456b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0456b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0456b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0456b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0456b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0456b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0456b-116">Not supported.</span></span>|
|<span data-ttu-id="0456b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0456b-117">Application</span></span>|<span data-ttu-id="0456b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0456b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0456b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0456b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="0456b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0456b-120">Request headers</span></span>
|<span data-ttu-id="0456b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0456b-121">Header</span></span>|<span data-ttu-id="0456b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0456b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0456b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0456b-123">Authorization</span></span>|<span data-ttu-id="0456b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0456b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0456b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0456b-125">Accept</span></span>|<span data-ttu-id="0456b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0456b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0456b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0456b-127">Request body</span></span>
<span data-ttu-id="0456b-128">В теле запроса добавьте представление объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0456b-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="0456b-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="0456b-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="0456b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0456b-130">Property</span></span>|<span data-ttu-id="0456b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0456b-131">Type</span></span>|<span data-ttu-id="0456b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0456b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0456b-133">id</span><span class="sxs-lookup"><span data-stu-id="0456b-133">id</span></span>|<span data-ttu-id="0456b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0456b-134">String</span></span>|<span data-ttu-id="0456b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0456b-135">Key of the entity.</span></span>|
|<span data-ttu-id="0456b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0456b-136">displayName</span></span>|<span data-ttu-id="0456b-137">String</span><span class="sxs-lookup"><span data-stu-id="0456b-137">String</span></span>|<span data-ttu-id="0456b-138">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="0456b-138">The name of the policy.</span></span>|
|<span data-ttu-id="0456b-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0456b-139">compliantDeviceCount</span></span>|<span data-ttu-id="0456b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-140">Int32</span></span>|<span data-ttu-id="0456b-141">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="0456b-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="0456b-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0456b-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="0456b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-143">Int32</span></span>|<span data-ttu-id="0456b-144">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="0456b-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="0456b-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0456b-145">remediatedDeviceCount</span></span>|<span data-ttu-id="0456b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-146">Int32</span></span>|<span data-ttu-id="0456b-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="0456b-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="0456b-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0456b-148">errorDeviceCount</span></span>|<span data-ttu-id="0456b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-149">Int32</span></span>|<span data-ttu-id="0456b-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="0456b-150">Number of devices had error.</span></span>|
|<span data-ttu-id="0456b-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0456b-151">unknownDeviceCount</span></span>|<span data-ttu-id="0456b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-152">Int32</span></span>|<span data-ttu-id="0456b-153">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="0456b-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="0456b-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0456b-154">conflictDeviceCount</span></span>|<span data-ttu-id="0456b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-155">Int32</span></span>|<span data-ttu-id="0456b-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="0456b-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="0456b-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0456b-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="0456b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-158">Int32</span></span>|<span data-ttu-id="0456b-159">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="0456b-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="0456b-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="0456b-160">compliantUserCount</span></span>|<span data-ttu-id="0456b-161">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-161">Int32</span></span>|<span data-ttu-id="0456b-162">Количество пользователей, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="0456b-162">Number of compliant users.</span></span>|
|<span data-ttu-id="0456b-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="0456b-163">nonCompliantUserCount</span></span>|<span data-ttu-id="0456b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-164">Int32</span></span>|<span data-ttu-id="0456b-165">Количество пользователей, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="0456b-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="0456b-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="0456b-166">remediatedUserCount</span></span>|<span data-ttu-id="0456b-167">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-167">Int32</span></span>|<span data-ttu-id="0456b-168">Количество исправленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="0456b-168">Number of remediated users.</span></span>|
|<span data-ttu-id="0456b-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="0456b-169">errorUserCount</span></span>|<span data-ttu-id="0456b-170">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-170">Int32</span></span>|<span data-ttu-id="0456b-171">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="0456b-171">Number of users had error.</span></span>|
|<span data-ttu-id="0456b-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="0456b-172">unknownUserCount</span></span>|<span data-ttu-id="0456b-173">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-173">Int32</span></span>|<span data-ttu-id="0456b-174">Количество неизвестных пользователей.</span><span class="sxs-lookup"><span data-stu-id="0456b-174">Number of unknown users.</span></span>|
|<span data-ttu-id="0456b-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="0456b-175">conflictUserCount</span></span>|<span data-ttu-id="0456b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-176">Int32</span></span>|<span data-ttu-id="0456b-177">Количество конфликтующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="0456b-177">Number of conflict users.</span></span>|
|<span data-ttu-id="0456b-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="0456b-178">notApplicableUserCount</span></span>|<span data-ttu-id="0456b-179">Int32</span><span class="sxs-lookup"><span data-stu-id="0456b-179">Int32</span></span>|<span data-ttu-id="0456b-180">Количество неприменимых пользователей.</span><span class="sxs-lookup"><span data-stu-id="0456b-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="0456b-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="0456b-181">Response</span></span>
<span data-ttu-id="0456b-182">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0456b-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0456b-183">Пример</span><span class="sxs-lookup"><span data-stu-id="0456b-183">Example</span></span>
### <a name="request"></a><span data-ttu-id="0456b-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="0456b-184">Request</span></span>
<span data-ttu-id="0456b-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0456b-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 452

{
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

### <a name="response"></a><span data-ttu-id="0456b-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="0456b-186">Response</span></span>
<span data-ttu-id="0456b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0456b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






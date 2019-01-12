---
title: Update softwareUpdateStatusSummary
description: Обновление свойств объекта softwareUpdateStatusSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9696daa56c723a8bc6d5ef9d3d674ce16c6e2667
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984817"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="66a79-103">Update softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="66a79-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="66a79-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="66a79-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66a79-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66a79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66a79-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="66a79-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66a79-107">Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="66a79-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66a79-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="66a79-108">Prerequisites</span></span>
<span data-ttu-id="66a79-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66a79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66a79-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66a79-111">Permission type</span></span>|<span data-ttu-id="66a79-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="66a79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66a79-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66a79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66a79-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66a79-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66a79-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66a79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66a79-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66a79-116">Not supported.</span></span>|
|<span data-ttu-id="66a79-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66a79-117">Application</span></span>|<span data-ttu-id="66a79-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66a79-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66a79-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66a79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="66a79-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66a79-120">Request headers</span></span>
|<span data-ttu-id="66a79-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66a79-121">Header</span></span>|<span data-ttu-id="66a79-122">Значение</span><span class="sxs-lookup"><span data-stu-id="66a79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66a79-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66a79-123">Authorization</span></span>|<span data-ttu-id="66a79-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="66a79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66a79-125">Accept</span><span class="sxs-lookup"><span data-stu-id="66a79-125">Accept</span></span>|<span data-ttu-id="66a79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66a79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66a79-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="66a79-127">Request body</span></span>
<span data-ttu-id="66a79-128">В теле запроса добавьте представление объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66a79-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="66a79-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="66a79-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="66a79-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="66a79-130">Property</span></span>|<span data-ttu-id="66a79-131">Тип</span><span class="sxs-lookup"><span data-stu-id="66a79-131">Type</span></span>|<span data-ttu-id="66a79-132">Описание</span><span class="sxs-lookup"><span data-stu-id="66a79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66a79-133">id</span><span class="sxs-lookup"><span data-stu-id="66a79-133">id</span></span>|<span data-ttu-id="66a79-134">String</span><span class="sxs-lookup"><span data-stu-id="66a79-134">String</span></span>|<span data-ttu-id="66a79-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="66a79-135">Key of the entity.</span></span>|
|<span data-ttu-id="66a79-136">displayName</span><span class="sxs-lookup"><span data-stu-id="66a79-136">displayName</span></span>|<span data-ttu-id="66a79-137">String</span><span class="sxs-lookup"><span data-stu-id="66a79-137">String</span></span>|<span data-ttu-id="66a79-138">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="66a79-138">The name of the policy.</span></span>|
|<span data-ttu-id="66a79-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="66a79-139">compliantDeviceCount</span></span>|<span data-ttu-id="66a79-140">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-140">Int32</span></span>|<span data-ttu-id="66a79-141">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="66a79-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="66a79-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="66a79-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="66a79-143">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-143">Int32</span></span>|<span data-ttu-id="66a79-144">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="66a79-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="66a79-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="66a79-145">remediatedDeviceCount</span></span>|<span data-ttu-id="66a79-146">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-146">Int32</span></span>|<span data-ttu-id="66a79-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="66a79-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="66a79-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="66a79-148">errorDeviceCount</span></span>|<span data-ttu-id="66a79-149">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-149">Int32</span></span>|<span data-ttu-id="66a79-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="66a79-150">Number of devices had error.</span></span>|
|<span data-ttu-id="66a79-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="66a79-151">unknownDeviceCount</span></span>|<span data-ttu-id="66a79-152">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-152">Int32</span></span>|<span data-ttu-id="66a79-153">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="66a79-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="66a79-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="66a79-154">conflictDeviceCount</span></span>|<span data-ttu-id="66a79-155">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-155">Int32</span></span>|<span data-ttu-id="66a79-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="66a79-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="66a79-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="66a79-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="66a79-158">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-158">Int32</span></span>|<span data-ttu-id="66a79-159">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="66a79-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="66a79-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="66a79-160">compliantUserCount</span></span>|<span data-ttu-id="66a79-161">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-161">Int32</span></span>|<span data-ttu-id="66a79-162">Количество пользователей, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="66a79-162">Number of compliant users.</span></span>|
|<span data-ttu-id="66a79-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="66a79-163">nonCompliantUserCount</span></span>|<span data-ttu-id="66a79-164">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-164">Int32</span></span>|<span data-ttu-id="66a79-165">Количество пользователей, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="66a79-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="66a79-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="66a79-166">remediatedUserCount</span></span>|<span data-ttu-id="66a79-167">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-167">Int32</span></span>|<span data-ttu-id="66a79-168">Количество исправленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="66a79-168">Number of remediated users.</span></span>|
|<span data-ttu-id="66a79-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="66a79-169">errorUserCount</span></span>|<span data-ttu-id="66a79-170">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-170">Int32</span></span>|<span data-ttu-id="66a79-171">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="66a79-171">Number of users had error.</span></span>|
|<span data-ttu-id="66a79-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="66a79-172">unknownUserCount</span></span>|<span data-ttu-id="66a79-173">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-173">Int32</span></span>|<span data-ttu-id="66a79-174">Количество неизвестных пользователей.</span><span class="sxs-lookup"><span data-stu-id="66a79-174">Number of unknown users.</span></span>|
|<span data-ttu-id="66a79-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="66a79-175">conflictUserCount</span></span>|<span data-ttu-id="66a79-176">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-176">Int32</span></span>|<span data-ttu-id="66a79-177">Количество конфликтующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="66a79-177">Number of conflict users.</span></span>|
|<span data-ttu-id="66a79-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="66a79-178">notApplicableUserCount</span></span>|<span data-ttu-id="66a79-179">Int32</span><span class="sxs-lookup"><span data-stu-id="66a79-179">Int32</span></span>|<span data-ttu-id="66a79-180">Количество неприменимых пользователей.</span><span class="sxs-lookup"><span data-stu-id="66a79-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="66a79-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="66a79-181">Response</span></span>
<span data-ttu-id="66a79-182">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="66a79-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66a79-183">Пример</span><span class="sxs-lookup"><span data-stu-id="66a79-183">Example</span></span>
### <a name="request"></a><span data-ttu-id="66a79-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="66a79-184">Request</span></span>
<span data-ttu-id="66a79-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66a79-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="66a79-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="66a79-186">Response</span></span>
<span data-ttu-id="66a79-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="66a79-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






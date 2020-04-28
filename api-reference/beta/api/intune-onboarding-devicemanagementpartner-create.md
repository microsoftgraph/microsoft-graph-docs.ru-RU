---
title: Создание объекта deviceManagementPartner
description: Создание объекта deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f72b4ebb0fd4e2eada34aa1dce39383ae9a01ec4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463659"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="00df1-103">Создание объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="00df1-103">Create deviceManagementPartner</span></span>

<span data-ttu-id="00df1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00df1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00df1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00df1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00df1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00df1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00df1-107">Создание объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="00df1-107">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00df1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="00df1-108">Prerequisites</span></span>
<span data-ttu-id="00df1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00df1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00df1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00df1-111">Permission type</span></span>|<span data-ttu-id="00df1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00df1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00df1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00df1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00df1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00df1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="00df1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00df1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00df1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00df1-116">Not supported.</span></span>|
|<span data-ttu-id="00df1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00df1-117">Application</span></span>|<span data-ttu-id="00df1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00df1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00df1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00df1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="00df1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="00df1-120">Request headers</span></span>
|<span data-ttu-id="00df1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00df1-121">Header</span></span>|<span data-ttu-id="00df1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00df1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00df1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00df1-123">Authorization</span></span>|<span data-ttu-id="00df1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00df1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00df1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00df1-125">Accept</span></span>|<span data-ttu-id="00df1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00df1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00df1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00df1-127">Request body</span></span>
<span data-ttu-id="00df1-128">В теле запроса добавьте представление объекта deviceManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00df1-128">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="00df1-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="00df1-129">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="00df1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="00df1-130">Property</span></span>|<span data-ttu-id="00df1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="00df1-131">Type</span></span>|<span data-ttu-id="00df1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="00df1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00df1-133">id</span><span class="sxs-lookup"><span data-stu-id="00df1-133">id</span></span>|<span data-ttu-id="00df1-134">String</span><span class="sxs-lookup"><span data-stu-id="00df1-134">String</span></span>|<span data-ttu-id="00df1-135">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="00df1-135">Id of the entity</span></span>|
|<span data-ttu-id="00df1-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="00df1-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="00df1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00df1-137">DateTimeOffset</span></span>|<span data-ttu-id="00df1-138">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="00df1-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="00df1-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="00df1-139">partnerState</span></span>|[<span data-ttu-id="00df1-140">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="00df1-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="00df1-141">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="00df1-141">Partner state of this tenant.</span></span> <span data-ttu-id="00df1-142">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="00df1-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="00df1-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="00df1-143">partnerAppType</span></span>|[<span data-ttu-id="00df1-144">девицеманажементпартнерапптипе</span><span class="sxs-lookup"><span data-stu-id="00df1-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="00df1-145">Тип партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="00df1-145">Partner App type.</span></span> <span data-ttu-id="00df1-146">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="00df1-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="00df1-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="00df1-147">singleTenantAppId</span></span>|<span data-ttu-id="00df1-148">String</span><span class="sxs-lookup"><span data-stu-id="00df1-148">String</span></span>|<span data-ttu-id="00df1-149">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="00df1-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="00df1-150">displayName</span><span class="sxs-lookup"><span data-stu-id="00df1-150">displayName</span></span>|<span data-ttu-id="00df1-151">Строка</span><span class="sxs-lookup"><span data-stu-id="00df1-151">String</span></span>|<span data-ttu-id="00df1-152">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="00df1-152">Partner display name</span></span>|
|<span data-ttu-id="00df1-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="00df1-153">isConfigured</span></span>|<span data-ttu-id="00df1-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="00df1-154">Boolean</span></span>|<span data-ttu-id="00df1-155">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="00df1-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="00df1-156">вхенпартнердевицесвиллберемовед</span><span class="sxs-lookup"><span data-stu-id="00df1-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="00df1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00df1-157">DateTimeOffset</span></span>|<span data-ttu-id="00df1-158">Дата и время в формате UTC, когда партнерские устройства будет удален.</span><span class="sxs-lookup"><span data-stu-id="00df1-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="00df1-159">Это скоро станет обселете.</span><span class="sxs-lookup"><span data-stu-id="00df1-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="00df1-160">вхенпартнердевицесвиллбемаркедаснонкомплиант</span><span class="sxs-lookup"><span data-stu-id="00df1-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="00df1-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00df1-161">DateTimeOffset</span></span>|<span data-ttu-id="00df1-162">Дата и время в формате UTC, когда партнерские устройства будет помечен как несоответствующий.</span><span class="sxs-lookup"><span data-stu-id="00df1-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="00df1-163">Это скоро станет обселете.</span><span class="sxs-lookup"><span data-stu-id="00df1-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="00df1-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="00df1-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="00df1-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00df1-165">DateTimeOffset</span></span>|<span data-ttu-id="00df1-166">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства</span><span class="sxs-lookup"><span data-stu-id="00df1-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="00df1-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="00df1-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="00df1-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00df1-168">DateTimeOffset</span></span>|<span data-ttu-id="00df1-169">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям</span><span class="sxs-lookup"><span data-stu-id="00df1-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|
|<span data-ttu-id="00df1-170">граупсрекуирингпартнеренроллмент</span><span class="sxs-lookup"><span data-stu-id="00df1-170">groupsRequiringPartnerEnrollment</span></span>|<span data-ttu-id="00df1-171">Коллекция [девицеманажементпартнерассигнмент](../resources/intune-onboarding-devicemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="00df1-171">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="00df1-172">Группы пользователей, указывающие, осуществляется ли регистрация через партнера.</span><span class="sxs-lookup"><span data-stu-id="00df1-172">User groups that specifies whether enrollment is through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="00df1-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="00df1-173">Response</span></span>
<span data-ttu-id="00df1-174">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="00df1-174">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00df1-175">Пример</span><span class="sxs-lookup"><span data-stu-id="00df1-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="00df1-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="00df1-176">Request</span></span>
<span data-ttu-id="00df1-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00df1-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
Content-type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="00df1-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="00df1-178">Response</span></span>
<span data-ttu-id="00df1-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00df1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 946

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```




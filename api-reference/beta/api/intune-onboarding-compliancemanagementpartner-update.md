---
title: Обновление Комплианцеманажементпартнер
description: Обновление свойств объекта Комплианцеманажементпартнер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e588f476bb56faff1793c979005bfe8574665ff1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48721558"
---
# <a name="update-compliancemanagementpartner"></a><span data-ttu-id="548c0-103">Обновление Комплианцеманажементпартнер</span><span class="sxs-lookup"><span data-stu-id="548c0-103">Update complianceManagementPartner</span></span>

<span data-ttu-id="548c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="548c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="548c0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="548c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="548c0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="548c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="548c0-107">Обновление свойств объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="548c0-107">Update the properties of a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="548c0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="548c0-108">Prerequisites</span></span>
<span data-ttu-id="548c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="548c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="548c0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="548c0-111">Permission type</span></span>|<span data-ttu-id="548c0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="548c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="548c0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="548c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="548c0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="548c0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="548c0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="548c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="548c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="548c0-116">Not supported.</span></span>|
|<span data-ttu-id="548c0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="548c0-117">Application</span></span>|<span data-ttu-id="548c0-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="548c0-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="548c0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="548c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="548c0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="548c0-120">Request headers</span></span>
|<span data-ttu-id="548c0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="548c0-121">Header</span></span>|<span data-ttu-id="548c0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="548c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="548c0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="548c0-123">Authorization</span></span>|<span data-ttu-id="548c0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="548c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="548c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="548c0-125">Accept</span></span>|<span data-ttu-id="548c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="548c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="548c0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="548c0-127">Request body</span></span>
<span data-ttu-id="548c0-128">В тексте запроса добавьте представление объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="548c0-128">In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

<span data-ttu-id="548c0-129">В следующей таблице приведены свойства, необходимые при создании [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="548c0-129">The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

|<span data-ttu-id="548c0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="548c0-130">Property</span></span>|<span data-ttu-id="548c0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="548c0-131">Type</span></span>|<span data-ttu-id="548c0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="548c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="548c0-133">id</span><span class="sxs-lookup"><span data-stu-id="548c0-133">id</span></span>|<span data-ttu-id="548c0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="548c0-134">String</span></span>|<span data-ttu-id="548c0-135">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="548c0-135">Id of the entity</span></span>|
|<span data-ttu-id="548c0-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="548c0-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="548c0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="548c0-137">DateTimeOffset</span></span>|<span data-ttu-id="548c0-138">Метка времени последнего пакета пульса после того, как администратор направил соответствие партнеру управления соответствием</span><span class="sxs-lookup"><span data-stu-id="548c0-138">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="548c0-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="548c0-139">partnerState</span></span>|[<span data-ttu-id="548c0-140">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="548c0-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="548c0-141">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="548c0-141">Partner state of this tenant.</span></span> <span data-ttu-id="548c0-142">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="548c0-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="548c0-143">displayName</span><span class="sxs-lookup"><span data-stu-id="548c0-143">displayName</span></span>|<span data-ttu-id="548c0-144">Строка</span><span class="sxs-lookup"><span data-stu-id="548c0-144">String</span></span>|<span data-ttu-id="548c0-145">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="548c0-145">Partner display name</span></span>|
|<span data-ttu-id="548c0-146">макосонбоардед</span><span class="sxs-lookup"><span data-stu-id="548c0-146">macOsOnboarded</span></span>|<span data-ttu-id="548c0-147">Логический</span><span class="sxs-lookup"><span data-stu-id="548c0-147">Boolean</span></span>|<span data-ttu-id="548c0-148">Партнер, подключенный к устройствам Mac.</span><span class="sxs-lookup"><span data-stu-id="548c0-148">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="548c0-149">виндовсонбоардед</span><span class="sxs-lookup"><span data-stu-id="548c0-149">windowsOnboarded</span></span>|<span data-ttu-id="548c0-150">Логический</span><span class="sxs-lookup"><span data-stu-id="548c0-150">Boolean</span></span>|<span data-ttu-id="548c0-151">Партнер, направленный на устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="548c0-151">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="548c0-152">андроидонбоардед</span><span class="sxs-lookup"><span data-stu-id="548c0-152">androidOnboarded</span></span>|<span data-ttu-id="548c0-153">Логический</span><span class="sxs-lookup"><span data-stu-id="548c0-153">Boolean</span></span>|<span data-ttu-id="548c0-154">Партнер, направленный на устройства с Android.</span><span class="sxs-lookup"><span data-stu-id="548c0-154">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="548c0-155">иосонбоардед</span><span class="sxs-lookup"><span data-stu-id="548c0-155">iosOnboarded</span></span>|<span data-ttu-id="548c0-156">Логический</span><span class="sxs-lookup"><span data-stu-id="548c0-156">Boolean</span></span>|<span data-ttu-id="548c0-157">Партнер, подключенный к устройствам iOS.</span><span class="sxs-lookup"><span data-stu-id="548c0-157">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="548c0-158">макосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="548c0-158">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="548c0-159">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="548c0-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="548c0-160">Группы пользователей, которые регистрируют устройства Mac через партнера.</span><span class="sxs-lookup"><span data-stu-id="548c0-160">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="548c0-161">виндовсенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="548c0-161">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="548c0-162">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="548c0-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="548c0-163">Группы пользователей, которые регистрируют устройства Windows с помощью партнера.</span><span class="sxs-lookup"><span data-stu-id="548c0-163">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="548c0-164">андроиденроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="548c0-164">androidEnrollmentAssignments</span></span>|<span data-ttu-id="548c0-165">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="548c0-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="548c0-166">Группы пользователей, которые регистрируют устройства с Android через партнера.</span><span class="sxs-lookup"><span data-stu-id="548c0-166">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="548c0-167">иосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="548c0-167">iosEnrollmentAssignments</span></span>|<span data-ttu-id="548c0-168">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="548c0-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="548c0-169">Группы пользователей, которые регистрируют устройства с iOS через партнера.</span><span class="sxs-lookup"><span data-stu-id="548c0-169">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="548c0-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="548c0-170">Response</span></span>
<span data-ttu-id="548c0-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="548c0-171">If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="548c0-172">Пример</span><span class="sxs-lookup"><span data-stu-id="548c0-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="548c0-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="548c0-173">Request</span></span>
<span data-ttu-id="548c0-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="548c0-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
Content-type: application/json
Content-length: 1944

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
  "windowsOnboarded": true,
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="548c0-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="548c0-175">Response</span></span>
<span data-ttu-id="548c0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="548c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1993

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
  "windowsOnboarded": true,
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```






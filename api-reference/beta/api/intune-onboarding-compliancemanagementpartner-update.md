---
title: Обновление Комплианцеманажементпартнер
description: Обновление свойств объекта Комплианцеманажементпартнер.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 646fb55f08abe1fc6d6b0745b2fbf1affcb82aa2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941885"
---
# <a name="update-compliancemanagementpartner"></a><span data-ttu-id="4bf69-103">Обновление Комплианцеманажементпартнер</span><span class="sxs-lookup"><span data-stu-id="4bf69-103">Update complianceManagementPartner</span></span>

> <span data-ttu-id="4bf69-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bf69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bf69-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4bf69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bf69-106">Обновление свойств объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="4bf69-106">Update the properties of a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bf69-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4bf69-107">Prerequisites</span></span>
<span data-ttu-id="4bf69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bf69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bf69-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bf69-110">Permission type</span></span>|<span data-ttu-id="4bf69-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bf69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bf69-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bf69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4bf69-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bf69-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4bf69-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bf69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bf69-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bf69-115">Not supported.</span></span>|
|<span data-ttu-id="4bf69-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bf69-116">Application</span></span>|<span data-ttu-id="4bf69-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bf69-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bf69-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bf69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="4bf69-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4bf69-119">Request headers</span></span>
|<span data-ttu-id="4bf69-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4bf69-120">Header</span></span>|<span data-ttu-id="4bf69-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4bf69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bf69-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4bf69-122">Authorization</span></span>|<span data-ttu-id="4bf69-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bf69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bf69-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4bf69-124">Accept</span></span>|<span data-ttu-id="4bf69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4bf69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bf69-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4bf69-126">Request body</span></span>
<span data-ttu-id="4bf69-127">В тексте запроса добавьте представление объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bf69-127">In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

<span data-ttu-id="4bf69-128">В следующей таблице приведены свойства, необходимые при создании [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="4bf69-128">The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

|<span data-ttu-id="4bf69-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bf69-129">Property</span></span>|<span data-ttu-id="4bf69-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4bf69-130">Type</span></span>|<span data-ttu-id="4bf69-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4bf69-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bf69-132">id</span><span class="sxs-lookup"><span data-stu-id="4bf69-132">id</span></span>|<span data-ttu-id="4bf69-133">String</span><span class="sxs-lookup"><span data-stu-id="4bf69-133">String</span></span>|<span data-ttu-id="4bf69-134">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="4bf69-134">Id of the entity</span></span>|
|<span data-ttu-id="4bf69-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="4bf69-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="4bf69-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bf69-136">DateTimeOffset</span></span>|<span data-ttu-id="4bf69-137">Метка времени последнего пакета пульса после того, как администратор направил соответствие партнеру управления соответствием</span><span class="sxs-lookup"><span data-stu-id="4bf69-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="4bf69-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="4bf69-138">partnerState</span></span>|[<span data-ttu-id="4bf69-139">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="4bf69-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="4bf69-140">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="4bf69-140">Partner state of this tenant.</span></span> <span data-ttu-id="4bf69-141">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="4bf69-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="4bf69-142">displayName</span><span class="sxs-lookup"><span data-stu-id="4bf69-142">displayName</span></span>|<span data-ttu-id="4bf69-143">Строка</span><span class="sxs-lookup"><span data-stu-id="4bf69-143">String</span></span>|<span data-ttu-id="4bf69-144">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="4bf69-144">Partner display name</span></span>|
|<span data-ttu-id="4bf69-145">макосонбоардед</span><span class="sxs-lookup"><span data-stu-id="4bf69-145">macOsOnboarded</span></span>|<span data-ttu-id="4bf69-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bf69-146">Boolean</span></span>|<span data-ttu-id="4bf69-147">Партнер, подключенный к устройствам Mac.</span><span class="sxs-lookup"><span data-stu-id="4bf69-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="4bf69-148">виндовсонбоардед</span><span class="sxs-lookup"><span data-stu-id="4bf69-148">windowsOnboarded</span></span>|<span data-ttu-id="4bf69-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bf69-149">Boolean</span></span>|<span data-ttu-id="4bf69-150">Партнер, направленный на устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="4bf69-150">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="4bf69-151">андроидонбоардед</span><span class="sxs-lookup"><span data-stu-id="4bf69-151">androidOnboarded</span></span>|<span data-ttu-id="4bf69-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bf69-152">Boolean</span></span>|<span data-ttu-id="4bf69-153">Партнер, направленный на устройства с Android.</span><span class="sxs-lookup"><span data-stu-id="4bf69-153">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="4bf69-154">иосонбоардед</span><span class="sxs-lookup"><span data-stu-id="4bf69-154">iosOnboarded</span></span>|<span data-ttu-id="4bf69-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bf69-155">Boolean</span></span>|<span data-ttu-id="4bf69-156">Партнер, подключенный к устройствам iOS.</span><span class="sxs-lookup"><span data-stu-id="4bf69-156">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="4bf69-157">макосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="4bf69-157">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="4bf69-158">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4bf69-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="4bf69-159">Группы пользователей, которые регистрируют устройства Mac через партнера.</span><span class="sxs-lookup"><span data-stu-id="4bf69-159">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="4bf69-160">виндовсенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="4bf69-160">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="4bf69-161">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4bf69-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="4bf69-162">Группы пользователей, которые регистрируют устройства Windows с помощью партнера.</span><span class="sxs-lookup"><span data-stu-id="4bf69-162">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="4bf69-163">андроиденроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="4bf69-163">androidEnrollmentAssignments</span></span>|<span data-ttu-id="4bf69-164">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4bf69-164">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="4bf69-165">Группы пользователей, которые регистрируют устройства с Android через партнера.</span><span class="sxs-lookup"><span data-stu-id="4bf69-165">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="4bf69-166">иосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="4bf69-166">iosEnrollmentAssignments</span></span>|<span data-ttu-id="4bf69-167">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4bf69-167">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="4bf69-168">Группы пользователей, которые регистрируют устройства с iOS через партнера.</span><span class="sxs-lookup"><span data-stu-id="4bf69-168">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="4bf69-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bf69-169">Response</span></span>
<span data-ttu-id="4bf69-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4bf69-170">If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bf69-171">Пример</span><span class="sxs-lookup"><span data-stu-id="4bf69-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bf69-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bf69-172">Request</span></span>
<span data-ttu-id="4bf69-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bf69-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
Content-type: application/json
Content-length: 1244

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4bf69-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bf69-174">Response</span></span>
<span data-ttu-id="4bf69-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4bf69-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1293

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```






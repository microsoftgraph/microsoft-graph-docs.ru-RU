---
title: Обновление Комплианцеманажементпартнер
description: Обновление свойств объекта Комплианцеманажементпартнер.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 816b0c24c104432852ce81e2b4151fcfab694e26
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803051"
---
# <a name="update-compliancemanagementpartner"></a><span data-ttu-id="51746-103">Обновление Комплианцеманажементпартнер</span><span class="sxs-lookup"><span data-stu-id="51746-103">Update complianceManagementPartner</span></span>

> <span data-ttu-id="51746-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51746-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51746-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51746-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51746-106">Обновление свойств объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="51746-106">Update the properties of a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51746-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51746-107">Prerequisites</span></span>
<span data-ttu-id="51746-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51746-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51746-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51746-110">Permission type</span></span>|<span data-ttu-id="51746-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51746-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51746-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51746-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51746-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51746-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="51746-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51746-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51746-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51746-115">Not supported.</span></span>|
|<span data-ttu-id="51746-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="51746-116">Application</span></span>|<span data-ttu-id="51746-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51746-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51746-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51746-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="51746-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="51746-119">Request headers</span></span>
|<span data-ttu-id="51746-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51746-120">Header</span></span>|<span data-ttu-id="51746-121">Значение</span><span class="sxs-lookup"><span data-stu-id="51746-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51746-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51746-122">Authorization</span></span>|<span data-ttu-id="51746-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51746-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51746-124">Accept</span><span class="sxs-lookup"><span data-stu-id="51746-124">Accept</span></span>|<span data-ttu-id="51746-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51746-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51746-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51746-126">Request body</span></span>
<span data-ttu-id="51746-127">В тексте запроса добавьте представление объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51746-127">In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

<span data-ttu-id="51746-128">В следующей таблице приведены свойства, необходимые при создании [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="51746-128">The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

|<span data-ttu-id="51746-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="51746-129">Property</span></span>|<span data-ttu-id="51746-130">Тип</span><span class="sxs-lookup"><span data-stu-id="51746-130">Type</span></span>|<span data-ttu-id="51746-131">Описание</span><span class="sxs-lookup"><span data-stu-id="51746-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51746-132">id</span><span class="sxs-lookup"><span data-stu-id="51746-132">id</span></span>|<span data-ttu-id="51746-133">String</span><span class="sxs-lookup"><span data-stu-id="51746-133">String</span></span>|<span data-ttu-id="51746-134">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="51746-134">Id of the entity</span></span>|
|<span data-ttu-id="51746-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="51746-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="51746-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51746-136">DateTimeOffset</span></span>|<span data-ttu-id="51746-137">Метка времени последнего пакета пульса после того, как администратор направил соответствие партнеру управления соответствием</span><span class="sxs-lookup"><span data-stu-id="51746-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="51746-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="51746-138">partnerState</span></span>|[<span data-ttu-id="51746-139">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="51746-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="51746-140">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="51746-140">Partner state of this tenant.</span></span> <span data-ttu-id="51746-141">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="51746-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="51746-142">displayName</span><span class="sxs-lookup"><span data-stu-id="51746-142">displayName</span></span>|<span data-ttu-id="51746-143">Строка</span><span class="sxs-lookup"><span data-stu-id="51746-143">String</span></span>|<span data-ttu-id="51746-144">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="51746-144">Partner display name</span></span>|
|<span data-ttu-id="51746-145">макосонбоардед</span><span class="sxs-lookup"><span data-stu-id="51746-145">macOsOnboarded</span></span>|<span data-ttu-id="51746-146">Логический</span><span class="sxs-lookup"><span data-stu-id="51746-146">Boolean</span></span>|<span data-ttu-id="51746-147">Партнер, подключенный к устройствам Mac.</span><span class="sxs-lookup"><span data-stu-id="51746-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="51746-148">виндовсонбоардед</span><span class="sxs-lookup"><span data-stu-id="51746-148">windowsOnboarded</span></span>|<span data-ttu-id="51746-149">Логический</span><span class="sxs-lookup"><span data-stu-id="51746-149">Boolean</span></span>|<span data-ttu-id="51746-150">Партнер, направленный на устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="51746-150">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="51746-151">андроидонбоардед</span><span class="sxs-lookup"><span data-stu-id="51746-151">androidOnboarded</span></span>|<span data-ttu-id="51746-152">Логический</span><span class="sxs-lookup"><span data-stu-id="51746-152">Boolean</span></span>|<span data-ttu-id="51746-153">Партнер, направленный на устройства с Android.</span><span class="sxs-lookup"><span data-stu-id="51746-153">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="51746-154">иосонбоардед</span><span class="sxs-lookup"><span data-stu-id="51746-154">iosOnboarded</span></span>|<span data-ttu-id="51746-155">Логический</span><span class="sxs-lookup"><span data-stu-id="51746-155">Boolean</span></span>|<span data-ttu-id="51746-156">Партнер, подключенный к устройствам iOS.</span><span class="sxs-lookup"><span data-stu-id="51746-156">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="51746-157">макосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="51746-157">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="51746-158">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="51746-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="51746-159">Группы пользователей, которые регистрируют устройства Mac через партнера.</span><span class="sxs-lookup"><span data-stu-id="51746-159">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="51746-160">виндовсенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="51746-160">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="51746-161">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="51746-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="51746-162">Группы пользователей, которые регистрируют устройства Windows с помощью партнера.</span><span class="sxs-lookup"><span data-stu-id="51746-162">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="51746-163">андроиденроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="51746-163">androidEnrollmentAssignments</span></span>|<span data-ttu-id="51746-164">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="51746-164">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="51746-165">Группы пользователей, которые регистрируют устройства с Android через партнера.</span><span class="sxs-lookup"><span data-stu-id="51746-165">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="51746-166">иосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="51746-166">iosEnrollmentAssignments</span></span>|<span data-ttu-id="51746-167">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="51746-167">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="51746-168">Группы пользователей, которые регистрируют устройства с iOS через партнера.</span><span class="sxs-lookup"><span data-stu-id="51746-168">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="51746-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="51746-169">Response</span></span>
<span data-ttu-id="51746-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51746-170">If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51746-171">Пример</span><span class="sxs-lookup"><span data-stu-id="51746-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="51746-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="51746-172">Request</span></span>
<span data-ttu-id="51746-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51746-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="51746-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="51746-174">Response</span></span>
<span data-ttu-id="51746-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51746-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





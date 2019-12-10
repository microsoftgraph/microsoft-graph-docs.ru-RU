---
title: Создание Комплианцеманажементпартнер
description: Создание нового объекта Комплианцеманажементпартнер.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cbdc27b37794627aaf444138e92bb751c41c2780
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941920"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="3b33b-103">Создание Комплианцеманажементпартнер</span><span class="sxs-lookup"><span data-stu-id="3b33b-103">Create complianceManagementPartner</span></span>

> <span data-ttu-id="3b33b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b33b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b33b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b33b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b33b-106">Создание нового объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="3b33b-106">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b33b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3b33b-107">Prerequisites</span></span>
<span data-ttu-id="3b33b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b33b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b33b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b33b-110">Permission type</span></span>|<span data-ttu-id="3b33b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b33b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b33b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b33b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b33b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b33b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3b33b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b33b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b33b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b33b-115">Not supported.</span></span>|
|<span data-ttu-id="3b33b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b33b-116">Application</span></span>|<span data-ttu-id="3b33b-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b33b-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b33b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b33b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="3b33b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3b33b-119">Request headers</span></span>
|<span data-ttu-id="3b33b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b33b-120">Header</span></span>|<span data-ttu-id="3b33b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3b33b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b33b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b33b-122">Authorization</span></span>|<span data-ttu-id="3b33b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b33b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b33b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3b33b-124">Accept</span></span>|<span data-ttu-id="3b33b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b33b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b33b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3b33b-126">Request body</span></span>
<span data-ttu-id="3b33b-127">В тексте запроса добавьте представление объекта Комплианцеманажементпартнер в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b33b-127">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="3b33b-128">В следующей таблице приведены свойства, необходимые при создании Комплианцеманажементпартнер.</span><span class="sxs-lookup"><span data-stu-id="3b33b-128">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="3b33b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b33b-129">Property</span></span>|<span data-ttu-id="3b33b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3b33b-130">Type</span></span>|<span data-ttu-id="3b33b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3b33b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b33b-132">id</span><span class="sxs-lookup"><span data-stu-id="3b33b-132">id</span></span>|<span data-ttu-id="3b33b-133">String</span><span class="sxs-lookup"><span data-stu-id="3b33b-133">String</span></span>|<span data-ttu-id="3b33b-134">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="3b33b-134">Id of the entity</span></span>|
|<span data-ttu-id="3b33b-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="3b33b-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="3b33b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b33b-136">DateTimeOffset</span></span>|<span data-ttu-id="3b33b-137">Метка времени последнего пакета пульса после того, как администратор направил соответствие партнеру управления соответствием</span><span class="sxs-lookup"><span data-stu-id="3b33b-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="3b33b-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="3b33b-138">partnerState</span></span>|[<span data-ttu-id="3b33b-139">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="3b33b-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="3b33b-140">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="3b33b-140">Partner state of this tenant.</span></span> <span data-ttu-id="3b33b-141">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="3b33b-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="3b33b-142">displayName</span><span class="sxs-lookup"><span data-stu-id="3b33b-142">displayName</span></span>|<span data-ttu-id="3b33b-143">Строка</span><span class="sxs-lookup"><span data-stu-id="3b33b-143">String</span></span>|<span data-ttu-id="3b33b-144">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="3b33b-144">Partner display name</span></span>|
|<span data-ttu-id="3b33b-145">макосонбоардед</span><span class="sxs-lookup"><span data-stu-id="3b33b-145">macOsOnboarded</span></span>|<span data-ttu-id="3b33b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b33b-146">Boolean</span></span>|<span data-ttu-id="3b33b-147">Партнер, подключенный к устройствам Mac.</span><span class="sxs-lookup"><span data-stu-id="3b33b-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="3b33b-148">виндовсонбоардед</span><span class="sxs-lookup"><span data-stu-id="3b33b-148">windowsOnboarded</span></span>|<span data-ttu-id="3b33b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b33b-149">Boolean</span></span>|<span data-ttu-id="3b33b-150">Партнер, направленный на устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="3b33b-150">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="3b33b-151">андроидонбоардед</span><span class="sxs-lookup"><span data-stu-id="3b33b-151">androidOnboarded</span></span>|<span data-ttu-id="3b33b-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b33b-152">Boolean</span></span>|<span data-ttu-id="3b33b-153">Партнер, направленный на устройства с Android.</span><span class="sxs-lookup"><span data-stu-id="3b33b-153">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="3b33b-154">иосонбоардед</span><span class="sxs-lookup"><span data-stu-id="3b33b-154">iosOnboarded</span></span>|<span data-ttu-id="3b33b-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b33b-155">Boolean</span></span>|<span data-ttu-id="3b33b-156">Партнер, подключенный к устройствам iOS.</span><span class="sxs-lookup"><span data-stu-id="3b33b-156">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="3b33b-157">макосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="3b33b-157">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="3b33b-158">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3b33b-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="3b33b-159">Группы пользователей, которые регистрируют устройства Mac через партнера.</span><span class="sxs-lookup"><span data-stu-id="3b33b-159">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="3b33b-160">виндовсенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="3b33b-160">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="3b33b-161">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3b33b-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="3b33b-162">Группы пользователей, которые регистрируют устройства Windows с помощью партнера.</span><span class="sxs-lookup"><span data-stu-id="3b33b-162">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="3b33b-163">андроиденроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="3b33b-163">androidEnrollmentAssignments</span></span>|<span data-ttu-id="3b33b-164">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3b33b-164">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="3b33b-165">Группы пользователей, которые регистрируют устройства с Android через партнера.</span><span class="sxs-lookup"><span data-stu-id="3b33b-165">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="3b33b-166">иосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="3b33b-166">iosEnrollmentAssignments</span></span>|<span data-ttu-id="3b33b-167">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3b33b-167">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="3b33b-168">Группы пользователей, которые регистрируют устройства с iOS через партнера.</span><span class="sxs-lookup"><span data-stu-id="3b33b-168">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="3b33b-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b33b-169">Response</span></span>
<span data-ttu-id="3b33b-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b33b-170">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b33b-171">Пример</span><span class="sxs-lookup"><span data-stu-id="3b33b-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b33b-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b33b-172">Request</span></span>
<span data-ttu-id="3b33b-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b33b-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
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

### <a name="response"></a><span data-ttu-id="3b33b-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b33b-174">Response</span></span>
<span data-ttu-id="3b33b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b33b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






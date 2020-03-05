---
title: Создание Комплианцеманажементпартнер
description: Создание нового объекта Комплианцеманажементпартнер.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f449556df216643ff8d3e72797d105d39934e37
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462532"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="d836a-103">Создание Комплианцеманажементпартнер</span><span class="sxs-lookup"><span data-stu-id="d836a-103">Create complianceManagementPartner</span></span>

<span data-ttu-id="d836a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d836a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d836a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d836a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d836a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d836a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d836a-107">Создание нового объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="d836a-107">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d836a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d836a-108">Prerequisites</span></span>
<span data-ttu-id="d836a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d836a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d836a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d836a-111">Permission type</span></span>|<span data-ttu-id="d836a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d836a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d836a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d836a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d836a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d836a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d836a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d836a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d836a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d836a-116">Not supported.</span></span>|
|<span data-ttu-id="d836a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d836a-117">Application</span></span>|<span data-ttu-id="d836a-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d836a-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d836a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d836a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="d836a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d836a-120">Request headers</span></span>
|<span data-ttu-id="d836a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d836a-121">Header</span></span>|<span data-ttu-id="d836a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d836a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d836a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d836a-123">Authorization</span></span>|<span data-ttu-id="d836a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d836a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d836a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d836a-125">Accept</span></span>|<span data-ttu-id="d836a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d836a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d836a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d836a-127">Request body</span></span>
<span data-ttu-id="d836a-128">В тексте запроса добавьте представление объекта Комплианцеманажементпартнер в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d836a-128">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="d836a-129">В следующей таблице приведены свойства, необходимые при создании Комплианцеманажементпартнер.</span><span class="sxs-lookup"><span data-stu-id="d836a-129">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="d836a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d836a-130">Property</span></span>|<span data-ttu-id="d836a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d836a-131">Type</span></span>|<span data-ttu-id="d836a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d836a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d836a-133">id</span><span class="sxs-lookup"><span data-stu-id="d836a-133">id</span></span>|<span data-ttu-id="d836a-134">String</span><span class="sxs-lookup"><span data-stu-id="d836a-134">String</span></span>|<span data-ttu-id="d836a-135">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="d836a-135">Id of the entity</span></span>|
|<span data-ttu-id="d836a-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="d836a-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="d836a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d836a-137">DateTimeOffset</span></span>|<span data-ttu-id="d836a-138">Метка времени последнего пакета пульса после того, как администратор направил соответствие партнеру управления соответствием</span><span class="sxs-lookup"><span data-stu-id="d836a-138">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="d836a-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="d836a-139">partnerState</span></span>|[<span data-ttu-id="d836a-140">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="d836a-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="d836a-141">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="d836a-141">Partner state of this tenant.</span></span> <span data-ttu-id="d836a-142">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="d836a-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="d836a-143">displayName</span><span class="sxs-lookup"><span data-stu-id="d836a-143">displayName</span></span>|<span data-ttu-id="d836a-144">Строка</span><span class="sxs-lookup"><span data-stu-id="d836a-144">String</span></span>|<span data-ttu-id="d836a-145">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="d836a-145">Partner display name</span></span>|
|<span data-ttu-id="d836a-146">макосонбоардед</span><span class="sxs-lookup"><span data-stu-id="d836a-146">macOsOnboarded</span></span>|<span data-ttu-id="d836a-147">Логический</span><span class="sxs-lookup"><span data-stu-id="d836a-147">Boolean</span></span>|<span data-ttu-id="d836a-148">Партнер, подключенный к устройствам Mac.</span><span class="sxs-lookup"><span data-stu-id="d836a-148">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="d836a-149">виндовсонбоардед</span><span class="sxs-lookup"><span data-stu-id="d836a-149">windowsOnboarded</span></span>|<span data-ttu-id="d836a-150">Логический</span><span class="sxs-lookup"><span data-stu-id="d836a-150">Boolean</span></span>|<span data-ttu-id="d836a-151">Партнер, направленный на устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="d836a-151">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="d836a-152">андроидонбоардед</span><span class="sxs-lookup"><span data-stu-id="d836a-152">androidOnboarded</span></span>|<span data-ttu-id="d836a-153">Логический</span><span class="sxs-lookup"><span data-stu-id="d836a-153">Boolean</span></span>|<span data-ttu-id="d836a-154">Партнер, направленный на устройства с Android.</span><span class="sxs-lookup"><span data-stu-id="d836a-154">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="d836a-155">иосонбоардед</span><span class="sxs-lookup"><span data-stu-id="d836a-155">iosOnboarded</span></span>|<span data-ttu-id="d836a-156">Логический</span><span class="sxs-lookup"><span data-stu-id="d836a-156">Boolean</span></span>|<span data-ttu-id="d836a-157">Партнер, подключенный к устройствам iOS.</span><span class="sxs-lookup"><span data-stu-id="d836a-157">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="d836a-158">макосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="d836a-158">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="d836a-159">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d836a-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="d836a-160">Группы пользователей, которые регистрируют устройства Mac через партнера.</span><span class="sxs-lookup"><span data-stu-id="d836a-160">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="d836a-161">виндовсенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="d836a-161">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="d836a-162">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d836a-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="d836a-163">Группы пользователей, которые регистрируют устройства Windows с помощью партнера.</span><span class="sxs-lookup"><span data-stu-id="d836a-163">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="d836a-164">андроиденроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="d836a-164">androidEnrollmentAssignments</span></span>|<span data-ttu-id="d836a-165">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d836a-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="d836a-166">Группы пользователей, которые регистрируют устройства с Android через партнера.</span><span class="sxs-lookup"><span data-stu-id="d836a-166">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="d836a-167">иосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="d836a-167">iosEnrollmentAssignments</span></span>|<span data-ttu-id="d836a-168">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d836a-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="d836a-169">Группы пользователей, которые регистрируют устройства с iOS через партнера.</span><span class="sxs-lookup"><span data-stu-id="d836a-169">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="d836a-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="d836a-170">Response</span></span>
<span data-ttu-id="d836a-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d836a-171">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d836a-172">Пример</span><span class="sxs-lookup"><span data-stu-id="d836a-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="d836a-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="d836a-173">Request</span></span>
<span data-ttu-id="d836a-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d836a-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d836a-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="d836a-175">Response</span></span>
<span data-ttu-id="d836a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d836a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






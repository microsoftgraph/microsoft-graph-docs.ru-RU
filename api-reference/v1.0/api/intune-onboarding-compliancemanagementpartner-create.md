---
title: Создание Комплианцеманажементпартнер
description: Создание нового объекта Комплианцеманажементпартнер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 09aefccda257cd4e49fa02df72554618a32d8962
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967907"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="c344e-103">Создание Комплианцеманажементпартнер</span><span class="sxs-lookup"><span data-stu-id="c344e-103">Create complianceManagementPartner</span></span>

<span data-ttu-id="c344e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c344e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c344e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c344e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c344e-106">Создание нового объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="c344e-106">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c344e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c344e-107">Prerequisites</span></span>
<span data-ttu-id="c344e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c344e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c344e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c344e-110">Permission type</span></span>|<span data-ttu-id="c344e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c344e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c344e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c344e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c344e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c344e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c344e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c344e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c344e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c344e-115">Not supported.</span></span>|
|<span data-ttu-id="c344e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c344e-116">Application</span></span>|<span data-ttu-id="c344e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c344e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c344e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c344e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="c344e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c344e-119">Request headers</span></span>
|<span data-ttu-id="c344e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c344e-120">Header</span></span>|<span data-ttu-id="c344e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c344e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c344e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c344e-122">Authorization</span></span>|<span data-ttu-id="c344e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c344e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c344e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c344e-124">Accept</span></span>|<span data-ttu-id="c344e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c344e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c344e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c344e-126">Request body</span></span>
<span data-ttu-id="c344e-127">В тексте запроса добавьте представление объекта Комплианцеманажементпартнер в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c344e-127">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="c344e-128">В следующей таблице приведены свойства, необходимые при создании Комплианцеманажементпартнер.</span><span class="sxs-lookup"><span data-stu-id="c344e-128">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="c344e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c344e-129">Property</span></span>|<span data-ttu-id="c344e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c344e-130">Type</span></span>|<span data-ttu-id="c344e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c344e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c344e-132">id</span><span class="sxs-lookup"><span data-stu-id="c344e-132">id</span></span>|<span data-ttu-id="c344e-133">String</span><span class="sxs-lookup"><span data-stu-id="c344e-133">String</span></span>|<span data-ttu-id="c344e-134">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="c344e-134">Id of the entity</span></span>|
|<span data-ttu-id="c344e-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="c344e-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="c344e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c344e-136">DateTimeOffset</span></span>|<span data-ttu-id="c344e-137">Метка времени последнего пакета пульса после того, как администратор направил соответствие партнеру управления соответствием</span><span class="sxs-lookup"><span data-stu-id="c344e-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="c344e-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="c344e-138">partnerState</span></span>|[<span data-ttu-id="c344e-139">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="c344e-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="c344e-140">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="c344e-140">Partner state of this tenant.</span></span> <span data-ttu-id="c344e-141">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="c344e-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="c344e-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c344e-142">displayName</span></span>|<span data-ttu-id="c344e-143">String</span><span class="sxs-lookup"><span data-stu-id="c344e-143">String</span></span>|<span data-ttu-id="c344e-144">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="c344e-144">Partner display name</span></span>|
|<span data-ttu-id="c344e-145">макосонбоардед</span><span class="sxs-lookup"><span data-stu-id="c344e-145">macOsOnboarded</span></span>|<span data-ttu-id="c344e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c344e-146">Boolean</span></span>|<span data-ttu-id="c344e-147">Партнер, подключенный к устройствам Mac.</span><span class="sxs-lookup"><span data-stu-id="c344e-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="c344e-148">андроидонбоардед</span><span class="sxs-lookup"><span data-stu-id="c344e-148">androidOnboarded</span></span>|<span data-ttu-id="c344e-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="c344e-149">Boolean</span></span>|<span data-ttu-id="c344e-150">Партнер, направленный на устройства с Android.</span><span class="sxs-lookup"><span data-stu-id="c344e-150">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="c344e-151">иосонбоардед</span><span class="sxs-lookup"><span data-stu-id="c344e-151">iosOnboarded</span></span>|<span data-ttu-id="c344e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="c344e-152">Boolean</span></span>|<span data-ttu-id="c344e-153">Партнер, подключенный к устройствам iOS.</span><span class="sxs-lookup"><span data-stu-id="c344e-153">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="c344e-154">макосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="c344e-154">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="c344e-155">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c344e-155">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c344e-156">Группы пользователей, которые регистрируют устройства Mac через партнера.</span><span class="sxs-lookup"><span data-stu-id="c344e-156">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="c344e-157">андроиденроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="c344e-157">androidEnrollmentAssignments</span></span>|<span data-ttu-id="c344e-158">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c344e-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c344e-159">Группы пользователей, которые регистрируют устройства с Android через партнера.</span><span class="sxs-lookup"><span data-stu-id="c344e-159">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="c344e-160">иосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="c344e-160">iosEnrollmentAssignments</span></span>|<span data-ttu-id="c344e-161">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c344e-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c344e-162">Группы пользователей, которые регистрируют устройства с iOS через партнера.</span><span class="sxs-lookup"><span data-stu-id="c344e-162">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="c344e-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c344e-163">Response</span></span>
<span data-ttu-id="c344e-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c344e-164">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c344e-165">Пример</span><span class="sxs-lookup"><span data-stu-id="c344e-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="c344e-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="c344e-166">Request</span></span>
<span data-ttu-id="c344e-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c344e-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners
Content-type: application/json
Content-length: 982

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
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

### <a name="response"></a><span data-ttu-id="c344e-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c344e-168">Response</span></span>
<span data-ttu-id="c344e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c344e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1031

{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "displayName": "Display Name value",
  "macOsOnboarded": true,
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







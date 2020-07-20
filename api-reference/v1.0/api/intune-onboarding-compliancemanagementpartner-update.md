---
title: Обновление Комплианцеманажементпартнер
description: Обновление свойств объекта Комплианцеманажементпартнер.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9574c2ddaacb60f9c41ea73608445de93365cb6e
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744171"
---
# <a name="update-compliancemanagementpartner"></a><span data-ttu-id="8d16d-103">Обновление Комплианцеманажементпартнер</span><span class="sxs-lookup"><span data-stu-id="8d16d-103">Update complianceManagementPartner</span></span>

<span data-ttu-id="8d16d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d16d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d16d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d16d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d16d-106">Обновление свойств объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="8d16d-106">Update the properties of a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d16d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d16d-107">Prerequisites</span></span>
<span data-ttu-id="8d16d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d16d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d16d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d16d-110">Permission type</span></span>|<span data-ttu-id="8d16d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d16d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d16d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d16d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d16d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d16d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8d16d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d16d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d16d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d16d-115">Not supported.</span></span>|
|<span data-ttu-id="8d16d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d16d-116">Application</span></span>|<span data-ttu-id="8d16d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d16d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d16d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d16d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="8d16d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8d16d-119">Request headers</span></span>
|<span data-ttu-id="8d16d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d16d-120">Header</span></span>|<span data-ttu-id="8d16d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8d16d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d16d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d16d-122">Authorization</span></span>|<span data-ttu-id="8d16d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d16d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d16d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8d16d-124">Accept</span></span>|<span data-ttu-id="8d16d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d16d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d16d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d16d-126">Request body</span></span>
<span data-ttu-id="8d16d-127">В тексте запроса добавьте представление объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d16d-127">In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

<span data-ttu-id="8d16d-128">В следующей таблице приведены свойства, необходимые при создании [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="8d16d-128">The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

|<span data-ttu-id="8d16d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d16d-129">Property</span></span>|<span data-ttu-id="8d16d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8d16d-130">Type</span></span>|<span data-ttu-id="8d16d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8d16d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d16d-132">id</span><span class="sxs-lookup"><span data-stu-id="8d16d-132">id</span></span>|<span data-ttu-id="8d16d-133">String</span><span class="sxs-lookup"><span data-stu-id="8d16d-133">String</span></span>|<span data-ttu-id="8d16d-134">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="8d16d-134">Id of the entity</span></span>|
|<span data-ttu-id="8d16d-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="8d16d-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="8d16d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d16d-136">DateTimeOffset</span></span>|<span data-ttu-id="8d16d-137">Метка времени последнего пакета пульса после того, как администратор направил соответствие партнеру управления соответствием</span><span class="sxs-lookup"><span data-stu-id="8d16d-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="8d16d-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="8d16d-138">partnerState</span></span>|[<span data-ttu-id="8d16d-139">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="8d16d-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="8d16d-140">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="8d16d-140">Partner state of this tenant.</span></span> <span data-ttu-id="8d16d-141">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="8d16d-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="8d16d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="8d16d-142">displayName</span></span>|<span data-ttu-id="8d16d-143">Строка</span><span class="sxs-lookup"><span data-stu-id="8d16d-143">String</span></span>|<span data-ttu-id="8d16d-144">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="8d16d-144">Partner display name</span></span>|
|<span data-ttu-id="8d16d-145">макосонбоардед</span><span class="sxs-lookup"><span data-stu-id="8d16d-145">macOsOnboarded</span></span>|<span data-ttu-id="8d16d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d16d-146">Boolean</span></span>|<span data-ttu-id="8d16d-147">Партнер, подключенный к устройствам Mac.</span><span class="sxs-lookup"><span data-stu-id="8d16d-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="8d16d-148">андроидонбоардед</span><span class="sxs-lookup"><span data-stu-id="8d16d-148">androidOnboarded</span></span>|<span data-ttu-id="8d16d-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d16d-149">Boolean</span></span>|<span data-ttu-id="8d16d-150">Партнер, направленный на устройства с Android.</span><span class="sxs-lookup"><span data-stu-id="8d16d-150">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="8d16d-151">иосонбоардед</span><span class="sxs-lookup"><span data-stu-id="8d16d-151">iosOnboarded</span></span>|<span data-ttu-id="8d16d-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d16d-152">Boolean</span></span>|<span data-ttu-id="8d16d-153">Партнер, подключенный к устройствам iOS.</span><span class="sxs-lookup"><span data-stu-id="8d16d-153">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="8d16d-154">макосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="8d16d-154">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="8d16d-155">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8d16d-155">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="8d16d-156">Группы пользователей, которые регистрируют устройства Mac через партнера.</span><span class="sxs-lookup"><span data-stu-id="8d16d-156">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="8d16d-157">андроиденроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="8d16d-157">androidEnrollmentAssignments</span></span>|<span data-ttu-id="8d16d-158">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8d16d-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="8d16d-159">Группы пользователей, которые регистрируют устройства с Android через партнера.</span><span class="sxs-lookup"><span data-stu-id="8d16d-159">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="8d16d-160">иосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="8d16d-160">iosEnrollmentAssignments</span></span>|<span data-ttu-id="8d16d-161">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8d16d-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="8d16d-162">Группы пользователей, которые регистрируют устройства с iOS через партнера.</span><span class="sxs-lookup"><span data-stu-id="8d16d-162">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="8d16d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d16d-163">Response</span></span>
<span data-ttu-id="8d16d-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d16d-164">If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d16d-165">Пример</span><span class="sxs-lookup"><span data-stu-id="8d16d-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d16d-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d16d-166">Request</span></span>
<span data-ttu-id="8d16d-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d16d-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
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

### <a name="response"></a><span data-ttu-id="8d16d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d16d-168">Response</span></span>
<span data-ttu-id="8d16d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d16d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




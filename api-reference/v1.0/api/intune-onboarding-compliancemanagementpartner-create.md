---
title: Создание Комплианцеманажементпартнер
description: Создание нового объекта Комплианцеманажементпартнер.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c606f0fdf4fbf9f589c2aab2423373225f1bdf7c
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744180"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="c3cfc-103">Создание Комплианцеманажементпартнер</span><span class="sxs-lookup"><span data-stu-id="c3cfc-103">Create complianceManagementPartner</span></span>

<span data-ttu-id="c3cfc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3cfc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3cfc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3cfc-106">Создание нового объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="c3cfc-106">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3cfc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c3cfc-107">Prerequisites</span></span>
<span data-ttu-id="c3cfc-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c3cfc-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3cfc-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3cfc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3cfc-110">Permission type</span></span>|<span data-ttu-id="c3cfc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3cfc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3cfc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3cfc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3cfc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3cfc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c3cfc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3cfc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3cfc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-115">Not supported.</span></span>|
|<span data-ttu-id="c3cfc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3cfc-116">Application</span></span>|<span data-ttu-id="c3cfc-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3cfc-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3cfc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3cfc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="c3cfc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c3cfc-119">Request headers</span></span>
|<span data-ttu-id="c3cfc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3cfc-120">Header</span></span>|<span data-ttu-id="c3cfc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c3cfc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3cfc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3cfc-122">Authorization</span></span>|<span data-ttu-id="c3cfc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3cfc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c3cfc-124">Accept</span></span>|<span data-ttu-id="c3cfc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3cfc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3cfc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3cfc-126">Request body</span></span>
<span data-ttu-id="c3cfc-127">В тексте запроса добавьте представление объекта Комплианцеманажементпартнер в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-127">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="c3cfc-128">В следующей таблице приведены свойства, необходимые при создании Комплианцеманажементпартнер.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-128">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="c3cfc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3cfc-129">Property</span></span>|<span data-ttu-id="c3cfc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c3cfc-130">Type</span></span>|<span data-ttu-id="c3cfc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c3cfc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3cfc-132">id</span><span class="sxs-lookup"><span data-stu-id="c3cfc-132">id</span></span>|<span data-ttu-id="c3cfc-133">String</span><span class="sxs-lookup"><span data-stu-id="c3cfc-133">String</span></span>|<span data-ttu-id="c3cfc-134">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="c3cfc-134">Id of the entity</span></span>|
|<span data-ttu-id="c3cfc-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="c3cfc-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="c3cfc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3cfc-136">DateTimeOffset</span></span>|<span data-ttu-id="c3cfc-137">Метка времени последнего пакета пульса после того, как администратор направил соответствие партнеру управления соответствием</span><span class="sxs-lookup"><span data-stu-id="c3cfc-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="c3cfc-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="c3cfc-138">partnerState</span></span>|[<span data-ttu-id="c3cfc-139">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="c3cfc-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="c3cfc-140">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-140">Partner state of this tenant.</span></span> <span data-ttu-id="c3cfc-141">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="c3cfc-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c3cfc-142">displayName</span></span>|<span data-ttu-id="c3cfc-143">Строка</span><span class="sxs-lookup"><span data-stu-id="c3cfc-143">String</span></span>|<span data-ttu-id="c3cfc-144">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="c3cfc-144">Partner display name</span></span>|
|<span data-ttu-id="c3cfc-145">макосонбоардед</span><span class="sxs-lookup"><span data-stu-id="c3cfc-145">macOsOnboarded</span></span>|<span data-ttu-id="c3cfc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3cfc-146">Boolean</span></span>|<span data-ttu-id="c3cfc-147">Партнер, подключенный к устройствам Mac.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="c3cfc-148">андроидонбоардед</span><span class="sxs-lookup"><span data-stu-id="c3cfc-148">androidOnboarded</span></span>|<span data-ttu-id="c3cfc-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3cfc-149">Boolean</span></span>|<span data-ttu-id="c3cfc-150">Партнер, направленный на устройства с Android.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-150">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="c3cfc-151">иосонбоардед</span><span class="sxs-lookup"><span data-stu-id="c3cfc-151">iosOnboarded</span></span>|<span data-ttu-id="c3cfc-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3cfc-152">Boolean</span></span>|<span data-ttu-id="c3cfc-153">Партнер, подключенный к устройствам iOS.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-153">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="c3cfc-154">макосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="c3cfc-154">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="c3cfc-155">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c3cfc-155">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c3cfc-156">Группы пользователей, которые регистрируют устройства Mac через партнера.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-156">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="c3cfc-157">андроиденроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="c3cfc-157">androidEnrollmentAssignments</span></span>|<span data-ttu-id="c3cfc-158">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c3cfc-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c3cfc-159">Группы пользователей, которые регистрируют устройства с Android через партнера.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-159">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="c3cfc-160">иосенроллментассигнментс</span><span class="sxs-lookup"><span data-stu-id="c3cfc-160">iosEnrollmentAssignments</span></span>|<span data-ttu-id="c3cfc-161">Коллекция [комплианцеманажементпартнерассигнмент](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c3cfc-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="c3cfc-162">Группы пользователей, которые регистрируют устройства с iOS через партнера.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-162">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="c3cfc-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3cfc-163">Response</span></span>
<span data-ttu-id="c3cfc-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-164">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3cfc-165">Пример</span><span class="sxs-lookup"><span data-stu-id="c3cfc-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3cfc-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3cfc-166">Request</span></span>
<span data-ttu-id="c3cfc-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3cfc-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3cfc-168">Response</span></span>
<span data-ttu-id="c3cfc-169">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-169">Here is an example of the response.</span></span> <span data-ttu-id="c3cfc-170">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-170">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c3cfc-171">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c3cfc-171">All of the properties will be returned from an actual call.</span></span>
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




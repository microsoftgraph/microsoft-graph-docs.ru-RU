---
title: Обновление complianceManagementPartner
description: Обновление свойств объекта complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b8ca2caf205599881aae0957d988b700d790d4d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153839"
---
# <a name="update-compliancemanagementpartner"></a><span data-ttu-id="1269d-103">Обновление complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="1269d-103">Update complianceManagementPartner</span></span>

<span data-ttu-id="1269d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1269d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1269d-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1269d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1269d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1269d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1269d-107">Обновление свойств объекта [complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="1269d-107">Update the properties of a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1269d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1269d-108">Prerequisites</span></span>
<span data-ttu-id="1269d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1269d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1269d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1269d-111">Permission type</span></span>|<span data-ttu-id="1269d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1269d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1269d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1269d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1269d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1269d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1269d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1269d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1269d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1269d-116">Not supported.</span></span>|
|<span data-ttu-id="1269d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1269d-117">Application</span></span>|<span data-ttu-id="1269d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1269d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1269d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1269d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="1269d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1269d-120">Request headers</span></span>
|<span data-ttu-id="1269d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1269d-121">Header</span></span>|<span data-ttu-id="1269d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1269d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1269d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1269d-123">Authorization</span></span>|<span data-ttu-id="1269d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1269d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1269d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1269d-125">Accept</span></span>|<span data-ttu-id="1269d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1269d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1269d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1269d-127">Request body</span></span>
<span data-ttu-id="1269d-128">В теле запроса укажу представление объекта [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="1269d-128">In the request body, supply a JSON representation for the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

<span data-ttu-id="1269d-129">В следующей таблице показаны свойства, необходимые при создании [объекта complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="1269d-129">The following table shows the properties that are required when you create the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

|<span data-ttu-id="1269d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1269d-130">Property</span></span>|<span data-ttu-id="1269d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1269d-131">Type</span></span>|<span data-ttu-id="1269d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1269d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1269d-133">id</span><span class="sxs-lookup"><span data-stu-id="1269d-133">id</span></span>|<span data-ttu-id="1269d-134">String</span><span class="sxs-lookup"><span data-stu-id="1269d-134">String</span></span>|<span data-ttu-id="1269d-135">ИД сущности</span><span class="sxs-lookup"><span data-stu-id="1269d-135">Id of the entity</span></span>|
|<span data-ttu-id="1269d-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="1269d-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="1269d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1269d-137">DateTimeOffset</span></span>|<span data-ttu-id="1269d-138">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span><span class="sxs-lookup"><span data-stu-id="1269d-138">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="1269d-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="1269d-139">partnerState</span></span>|[<span data-ttu-id="1269d-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="1269d-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="1269d-141">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="1269d-141">Partner state of this tenant.</span></span> <span data-ttu-id="1269d-142">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="1269d-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="1269d-143">displayName</span><span class="sxs-lookup"><span data-stu-id="1269d-143">displayName</span></span>|<span data-ttu-id="1269d-144">String</span><span class="sxs-lookup"><span data-stu-id="1269d-144">String</span></span>|<span data-ttu-id="1269d-145">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="1269d-145">Partner display name</span></span>|
|<span data-ttu-id="1269d-146">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="1269d-146">macOsOnboarded</span></span>|<span data-ttu-id="1269d-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="1269d-147">Boolean</span></span>|<span data-ttu-id="1269d-148">Партнер для устройств Mac.</span><span class="sxs-lookup"><span data-stu-id="1269d-148">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="1269d-149">windowsOnboarded</span><span class="sxs-lookup"><span data-stu-id="1269d-149">windowsOnboarded</span></span>|<span data-ttu-id="1269d-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="1269d-150">Boolean</span></span>|<span data-ttu-id="1269d-151">Партнер, в который вошел для устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="1269d-151">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="1269d-152">androidOnboarded</span><span class="sxs-lookup"><span data-stu-id="1269d-152">androidOnboarded</span></span>|<span data-ttu-id="1269d-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="1269d-153">Boolean</span></span>|<span data-ttu-id="1269d-154">Партнер, вошел в платформу для устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="1269d-154">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="1269d-155">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="1269d-155">iosOnboarded</span></span>|<span data-ttu-id="1269d-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="1269d-156">Boolean</span></span>|<span data-ttu-id="1269d-157">Партнер, в который вошел для устройств с ios.</span><span class="sxs-lookup"><span data-stu-id="1269d-157">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="1269d-158">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="1269d-158">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="1269d-159">[Коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1269d-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="1269d-160">Группы пользователей, которые регистрют устройства Mac через партнера.</span><span class="sxs-lookup"><span data-stu-id="1269d-160">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="1269d-161">windowsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="1269d-161">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="1269d-162">[Коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1269d-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="1269d-163">Группы пользователей, которые регистрют устройства с Windows через партнера.</span><span class="sxs-lookup"><span data-stu-id="1269d-163">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="1269d-164">androidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="1269d-164">androidEnrollmentAssignments</span></span>|<span data-ttu-id="1269d-165">[Коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1269d-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="1269d-166">Группы пользователей, которые регистрют устройства Android через партнера.</span><span class="sxs-lookup"><span data-stu-id="1269d-166">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="1269d-167">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="1269d-167">iosEnrollmentAssignments</span></span>|<span data-ttu-id="1269d-168">[Коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1269d-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="1269d-169">Группы пользователей, которые регистрют устройства ios через партнера.</span><span class="sxs-lookup"><span data-stu-id="1269d-169">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="1269d-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="1269d-170">Response</span></span>
<span data-ttu-id="1269d-171">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1269d-171">If successful, this method returns a `200 OK` response code and an updated [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1269d-172">Пример</span><span class="sxs-lookup"><span data-stu-id="1269d-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="1269d-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="1269d-173">Request</span></span>
<span data-ttu-id="1269d-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1269d-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
Content-type: application/json
Content-length: 2216

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1269d-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="1269d-175">Response</span></span>
<span data-ttu-id="1269d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1269d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2265

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```





---
title: Создание complianceManagementPartner
description: Создание нового объекта complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd800d6ae8d1e2f1de3ba6ccec82c7a333180ddb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152735"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="12589-103">Создание complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="12589-103">Create complianceManagementPartner</span></span>

<span data-ttu-id="12589-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12589-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12589-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12589-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12589-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12589-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12589-107">Создание нового [объекта complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="12589-107">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12589-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="12589-108">Prerequisites</span></span>
<span data-ttu-id="12589-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12589-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12589-111">Permission type</span></span>|<span data-ttu-id="12589-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12589-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12589-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12589-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12589-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12589-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="12589-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12589-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12589-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12589-116">Not supported.</span></span>|
|<span data-ttu-id="12589-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="12589-117">Application</span></span>|<span data-ttu-id="12589-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12589-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12589-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12589-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="12589-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="12589-120">Request headers</span></span>
|<span data-ttu-id="12589-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12589-121">Header</span></span>|<span data-ttu-id="12589-122">Значение</span><span class="sxs-lookup"><span data-stu-id="12589-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12589-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12589-123">Authorization</span></span>|<span data-ttu-id="12589-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12589-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12589-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12589-125">Accept</span></span>|<span data-ttu-id="12589-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12589-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12589-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12589-127">Request body</span></span>
<span data-ttu-id="12589-128">В теле запроса поставляем представление JSON для объекта complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="12589-128">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="12589-129">В следующей таблице показаны свойства, необходимые при создании complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="12589-129">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="12589-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="12589-130">Property</span></span>|<span data-ttu-id="12589-131">Тип</span><span class="sxs-lookup"><span data-stu-id="12589-131">Type</span></span>|<span data-ttu-id="12589-132">Описание</span><span class="sxs-lookup"><span data-stu-id="12589-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12589-133">id</span><span class="sxs-lookup"><span data-stu-id="12589-133">id</span></span>|<span data-ttu-id="12589-134">Строка</span><span class="sxs-lookup"><span data-stu-id="12589-134">String</span></span>|<span data-ttu-id="12589-135">Id объекта</span><span class="sxs-lookup"><span data-stu-id="12589-135">Id of the entity</span></span>|
|<span data-ttu-id="12589-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="12589-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="12589-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12589-137">DateTimeOffset</span></span>|<span data-ttu-id="12589-138">Timestamp последнего сердцебиения после администратора, направленного партнеру по управлению соответствием</span><span class="sxs-lookup"><span data-stu-id="12589-138">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="12589-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="12589-139">partnerState</span></span>|[<span data-ttu-id="12589-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="12589-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="12589-141">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="12589-141">Partner state of this tenant.</span></span> <span data-ttu-id="12589-142">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="12589-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="12589-143">displayName</span><span class="sxs-lookup"><span data-stu-id="12589-143">displayName</span></span>|<span data-ttu-id="12589-144">Строка</span><span class="sxs-lookup"><span data-stu-id="12589-144">String</span></span>|<span data-ttu-id="12589-145">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="12589-145">Partner display name</span></span>|
|<span data-ttu-id="12589-146">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="12589-146">macOsOnboarded</span></span>|<span data-ttu-id="12589-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="12589-147">Boolean</span></span>|<span data-ttu-id="12589-148">Партнер, на борту для устройств Mac.</span><span class="sxs-lookup"><span data-stu-id="12589-148">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="12589-149">WindowsOnboarded</span><span class="sxs-lookup"><span data-stu-id="12589-149">windowsOnboarded</span></span>|<span data-ttu-id="12589-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="12589-150">Boolean</span></span>|<span data-ttu-id="12589-151">Партнер, на борту для устройств Windows.</span><span class="sxs-lookup"><span data-stu-id="12589-151">Partner onboarded for Windows devices.</span></span>|
|<span data-ttu-id="12589-152">AndroidOnboarded</span><span class="sxs-lookup"><span data-stu-id="12589-152">androidOnboarded</span></span>|<span data-ttu-id="12589-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="12589-153">Boolean</span></span>|<span data-ttu-id="12589-154">Партнер, на борту для android-устройств.</span><span class="sxs-lookup"><span data-stu-id="12589-154">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="12589-155">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="12589-155">iosOnboarded</span></span>|<span data-ttu-id="12589-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="12589-156">Boolean</span></span>|<span data-ttu-id="12589-157">Партнер, на борту для устройств ios.</span><span class="sxs-lookup"><span data-stu-id="12589-157">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="12589-158">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="12589-158">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="12589-159">[коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="12589-159">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="12589-160">Группы пользователей, которые регистрют устройства Mac через партнера.</span><span class="sxs-lookup"><span data-stu-id="12589-160">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="12589-161">windowsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="12589-161">windowsEnrollmentAssignments</span></span>|<span data-ttu-id="12589-162">[коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="12589-162">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="12589-163">Группы пользователей, которые регистрют устройства Windows через партнера.</span><span class="sxs-lookup"><span data-stu-id="12589-163">User groups which enroll Windows devices through partner.</span></span>|
|<span data-ttu-id="12589-164">AndroidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="12589-164">androidEnrollmentAssignments</span></span>|<span data-ttu-id="12589-165">[коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="12589-165">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="12589-166">Группы пользователей, которые регистрют устройства Android через партнера.</span><span class="sxs-lookup"><span data-stu-id="12589-166">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="12589-167">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="12589-167">iosEnrollmentAssignments</span></span>|<span data-ttu-id="12589-168">[коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="12589-168">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="12589-169">Группы пользователей, которые регистрют устройства ios через партнера.</span><span class="sxs-lookup"><span data-stu-id="12589-169">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="12589-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="12589-170">Response</span></span>
<span data-ttu-id="12589-171">В случае успешного выполнения этот метод возвращает код ответа и объект `201 Created` [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="12589-171">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12589-172">Пример</span><span class="sxs-lookup"><span data-stu-id="12589-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="12589-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="12589-173">Request</span></span>
<span data-ttu-id="12589-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12589-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
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

### <a name="response"></a><span data-ttu-id="12589-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="12589-175">Response</span></span>
<span data-ttu-id="12589-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12589-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





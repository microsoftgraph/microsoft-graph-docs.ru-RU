---
title: Создание complianceManagementPartner
description: Создание нового объекта complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0779afeef4d9b3944c5bd4c40b9222bf59b4fe09
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758047"
---
# <a name="create-compliancemanagementpartner"></a><span data-ttu-id="5ee83-103">Создание complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="5ee83-103">Create complianceManagementPartner</span></span>

<span data-ttu-id="5ee83-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ee83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ee83-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ee83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ee83-106">Создание нового [объекта complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="5ee83-106">Create a new [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ee83-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5ee83-107">Prerequisites</span></span>
<span data-ttu-id="5ee83-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ee83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ee83-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ee83-110">Permission type</span></span>|<span data-ttu-id="5ee83-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ee83-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ee83-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ee83-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ee83-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee83-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5ee83-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ee83-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ee83-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ee83-115">Not supported.</span></span>|
|<span data-ttu-id="5ee83-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5ee83-116">Application</span></span>|<span data-ttu-id="5ee83-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee83-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ee83-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ee83-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="5ee83-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5ee83-119">Request headers</span></span>
|<span data-ttu-id="5ee83-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ee83-120">Header</span></span>|<span data-ttu-id="5ee83-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5ee83-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ee83-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ee83-122">Authorization</span></span>|<span data-ttu-id="5ee83-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ee83-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ee83-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5ee83-124">Accept</span></span>|<span data-ttu-id="5ee83-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ee83-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ee83-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ee83-126">Request body</span></span>
<span data-ttu-id="5ee83-127">В теле запроса поставляем представление JSON для объекта complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="5ee83-127">In the request body, supply a JSON representation for the complianceManagementPartner object.</span></span>

<span data-ttu-id="5ee83-128">В следующей таблице показаны свойства, необходимые при создании complianceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="5ee83-128">The following table shows the properties that are required when you create the complianceManagementPartner.</span></span>

|<span data-ttu-id="5ee83-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ee83-129">Property</span></span>|<span data-ttu-id="5ee83-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5ee83-130">Type</span></span>|<span data-ttu-id="5ee83-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5ee83-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ee83-132">id</span><span class="sxs-lookup"><span data-stu-id="5ee83-132">id</span></span>|<span data-ttu-id="5ee83-133">String</span><span class="sxs-lookup"><span data-stu-id="5ee83-133">String</span></span>|<span data-ttu-id="5ee83-134">Id объекта</span><span class="sxs-lookup"><span data-stu-id="5ee83-134">Id of the entity</span></span>|
|<span data-ttu-id="5ee83-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee83-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="5ee83-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee83-136">DateTimeOffset</span></span>|<span data-ttu-id="5ee83-137">Timestamp последнего сердцебиения после администратора, направленного партнеру по управлению соответствием</span><span class="sxs-lookup"><span data-stu-id="5ee83-137">Timestamp of last heartbeat after admin onboarded to the compliance management partner</span></span>|
|<span data-ttu-id="5ee83-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="5ee83-138">partnerState</span></span>|[<span data-ttu-id="5ee83-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="5ee83-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="5ee83-140">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="5ee83-140">Partner state of this tenant.</span></span> <span data-ttu-id="5ee83-141">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="5ee83-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="5ee83-142">displayName</span><span class="sxs-lookup"><span data-stu-id="5ee83-142">displayName</span></span>|<span data-ttu-id="5ee83-143">String</span><span class="sxs-lookup"><span data-stu-id="5ee83-143">String</span></span>|<span data-ttu-id="5ee83-144">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="5ee83-144">Partner display name</span></span>|
|<span data-ttu-id="5ee83-145">macOsOnboarded</span><span class="sxs-lookup"><span data-stu-id="5ee83-145">macOsOnboarded</span></span>|<span data-ttu-id="5ee83-146">Логический</span><span class="sxs-lookup"><span data-stu-id="5ee83-146">Boolean</span></span>|<span data-ttu-id="5ee83-147">Партнер, на борту для устройств Mac.</span><span class="sxs-lookup"><span data-stu-id="5ee83-147">Partner onboarded for Mac devices.</span></span>|
|<span data-ttu-id="5ee83-148">AndroidOnboarded</span><span class="sxs-lookup"><span data-stu-id="5ee83-148">androidOnboarded</span></span>|<span data-ttu-id="5ee83-149">Логический</span><span class="sxs-lookup"><span data-stu-id="5ee83-149">Boolean</span></span>|<span data-ttu-id="5ee83-150">Партнер, на борту для android-устройств.</span><span class="sxs-lookup"><span data-stu-id="5ee83-150">Partner onboarded for Android devices.</span></span>|
|<span data-ttu-id="5ee83-151">iosOnboarded</span><span class="sxs-lookup"><span data-stu-id="5ee83-151">iosOnboarded</span></span>|<span data-ttu-id="5ee83-152">Логический</span><span class="sxs-lookup"><span data-stu-id="5ee83-152">Boolean</span></span>|<span data-ttu-id="5ee83-153">Партнер, на борту для устройств ios.</span><span class="sxs-lookup"><span data-stu-id="5ee83-153">Partner onboarded for ios devices.</span></span>|
|<span data-ttu-id="5ee83-154">macOsEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="5ee83-154">macOsEnrollmentAssignments</span></span>|<span data-ttu-id="5ee83-155">[коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5ee83-155">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="5ee83-156">Группы пользователей, которые регистрют устройства Mac через партнера.</span><span class="sxs-lookup"><span data-stu-id="5ee83-156">User groups which enroll Mac devices through partner.</span></span>|
|<span data-ttu-id="5ee83-157">AndroidEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="5ee83-157">androidEnrollmentAssignments</span></span>|<span data-ttu-id="5ee83-158">[коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5ee83-158">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="5ee83-159">Группы пользователей, которые регистрют устройства Android через партнера.</span><span class="sxs-lookup"><span data-stu-id="5ee83-159">User groups which enroll Android devices through partner.</span></span>|
|<span data-ttu-id="5ee83-160">iosEnrollmentAssignments</span><span class="sxs-lookup"><span data-stu-id="5ee83-160">iosEnrollmentAssignments</span></span>|<span data-ttu-id="5ee83-161">[коллекция complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5ee83-161">[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="5ee83-162">Группы пользователей, которые регистрют устройства ios через партнера.</span><span class="sxs-lookup"><span data-stu-id="5ee83-162">User groups which enroll ios devices through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="5ee83-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ee83-163">Response</span></span>
<span data-ttu-id="5ee83-164">В случае успешного выполнения этот метод возвращает код ответа и объект `201 Created` [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5ee83-164">If successful, this method returns a `201 Created` response code and a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ee83-165">Пример</span><span class="sxs-lookup"><span data-stu-id="5ee83-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ee83-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ee83-166">Request</span></span>
<span data-ttu-id="5ee83-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ee83-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners
Content-type: application/json
Content-length: 1186

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5ee83-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ee83-168">Response</span></span>
<span data-ttu-id="5ee83-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ee83-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1235

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```





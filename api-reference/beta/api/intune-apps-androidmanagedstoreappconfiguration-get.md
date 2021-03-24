---
title: Get AndroidManagedStoreAppConfiguration
description: Чтение свойств и связей объекта AndroidManagedStoreAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 159b1b286fd379a1333e4e949cad628963b42f84
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140968"
---
# <a name="get-androidmanagedstoreappconfiguration"></a><span data-ttu-id="e4432-103">Get AndroidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e4432-103">Get androidManagedStoreAppConfiguration</span></span>

<span data-ttu-id="e4432-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4432-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4432-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4432-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4432-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4432-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4432-107">Чтение свойств и связей [объекта AndroidManagedStoreAppConfiguration.](../resources/intune-apps-androidmanagedstoreappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4432-107">Read properties and relationships of the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4432-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e4432-108">Prerequisites</span></span>
<span data-ttu-id="e4432-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4432-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4432-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4432-111">Permission type</span></span>|<span data-ttu-id="e4432-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4432-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4432-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4432-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4432-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4432-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e4432-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4432-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4432-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4432-116">Not supported.</span></span>|
|<span data-ttu-id="e4432-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e4432-117">Application</span></span>|<span data-ttu-id="e4432-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4432-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4432-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4432-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4432-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e4432-120">Optional query parameters</span></span>
<span data-ttu-id="e4432-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e4432-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4432-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4432-122">Request headers</span></span>
|<span data-ttu-id="e4432-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4432-123">Header</span></span>|<span data-ttu-id="e4432-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e4432-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4432-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4432-125">Authorization</span></span>|<span data-ttu-id="e4432-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4432-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4432-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e4432-127">Accept</span></span>|<span data-ttu-id="e4432-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e4432-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4432-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4432-129">Request body</span></span>
<span data-ttu-id="e4432-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4432-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4432-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4432-131">Response</span></span>
<span data-ttu-id="e4432-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4432-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4432-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e4432-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4432-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4432-134">Request</span></span>
<span data-ttu-id="e4432-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4432-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e4432-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4432-136">Response</span></span>
<span data-ttu-id="e4432-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4432-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 880

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
    "id": "919a9335-9335-919a-3593-9a9135939a91",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "packageId": "Package Id value",
    "payloadJson": "Payload Json value",
    "permissionActions": [
      {
        "@odata.type": "microsoft.graph.androidPermissionAction",
        "permission": "Permission value",
        "action": "autoGrant"
      }
    ],
    "appSupportsOemConfig": true,
    "profileApplicability": "androidWorkProfile"
  }
}
```





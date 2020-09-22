---
title: Get windowsUniversalAppX
description: Чтение свойств и связей объекта windowsUniversalAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dccc2bf59ff509a5ca937488474684a212695219
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976076"
---
# <a name="get-windowsuniversalappx"></a><span data-ttu-id="f91ad-103">Get windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="f91ad-103">Get windowsUniversalAppX</span></span>

<span data-ttu-id="f91ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f91ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f91ad-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f91ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f91ad-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f91ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f91ad-107">Чтение свойств и связей объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="f91ad-107">Read properties and relationships of the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f91ad-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f91ad-108">Prerequisites</span></span>
<span data-ttu-id="f91ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f91ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f91ad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f91ad-111">Permission type</span></span>|<span data-ttu-id="f91ad-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f91ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f91ad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f91ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f91ad-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f91ad-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f91ad-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f91ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f91ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f91ad-116">Not supported.</span></span>|
|<span data-ttu-id="f91ad-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f91ad-117">Application</span></span>|<span data-ttu-id="f91ad-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f91ad-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f91ad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f91ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f91ad-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="f91ad-120">Optional query parameters</span></span>
<span data-ttu-id="f91ad-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f91ad-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f91ad-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f91ad-122">Request headers</span></span>
|<span data-ttu-id="f91ad-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f91ad-123">Header</span></span>|<span data-ttu-id="f91ad-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f91ad-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f91ad-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f91ad-125">Authorization</span></span>|<span data-ttu-id="f91ad-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f91ad-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f91ad-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f91ad-127">Accept</span></span>|<span data-ttu-id="f91ad-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f91ad-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f91ad-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f91ad-129">Request body</span></span>
<span data-ttu-id="f91ad-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f91ad-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f91ad-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f91ad-131">Response</span></span>
<span data-ttu-id="f91ad-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f91ad-132">If successful, this method returns a `200 OK` response code and [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f91ad-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f91ad-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f91ad-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f91ad-134">Request</span></span>
<span data-ttu-id="f91ad-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f91ad-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f91ad-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f91ad-136">Response</span></span>
<span data-ttu-id="f91ad-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f91ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1807

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUniversalAppX",
    "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "uploadState": 11,
    "publishingState": "processing",
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "dependentAppCount": 1,
    "supersedingAppCount": 3,
    "supersededAppCount": 2,
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "applicableArchitectures": "x86",
    "applicableDeviceTypes": "desktop",
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
    "isBundle": true,
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
      "v8_0": true,
      "v8_1": true,
      "v10_0": true,
      "v10_1607": true,
      "v10_1703": true,
      "v10_1709": true,
      "v10_1803": true,
      "v10_1809": true,
      "v10_1903": true
    },
    "identityVersion": "Identity Version value"
  }
}
```







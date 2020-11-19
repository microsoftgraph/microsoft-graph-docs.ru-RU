---
title: Получение windowsPhone81AppX
description: Чтение свойств и связей объекта windowsPhone81AppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e7459fa91e386215a76d6ac08a004f9908eb59c7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49246719"
---
# <a name="get-windowsphone81appx"></a><span data-ttu-id="c2cc0-103">Получение windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="c2cc0-103">Get windowsPhone81AppX</span></span>

<span data-ttu-id="c2cc0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2cc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2cc0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2cc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2cc0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2cc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2cc0-107">Чтение свойств и связей объекта [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="c2cc0-107">Read properties and relationships of the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2cc0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2cc0-108">Prerequisites</span></span>
<span data-ttu-id="c2cc0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2cc0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2cc0-111">Permission type</span></span>|<span data-ttu-id="c2cc0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2cc0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2cc0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2cc0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2cc0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2cc0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c2cc0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2cc0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2cc0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2cc0-116">Not supported.</span></span>|
|<span data-ttu-id="c2cc0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c2cc0-117">Application</span></span>|<span data-ttu-id="c2cc0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2cc0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2cc0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2cc0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2cc0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2cc0-120">Optional query parameters</span></span>
<span data-ttu-id="c2cc0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2cc0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2cc0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2cc0-122">Request headers</span></span>
|<span data-ttu-id="c2cc0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2cc0-123">Header</span></span>|<span data-ttu-id="c2cc0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c2cc0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2cc0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2cc0-125">Authorization</span></span>|<span data-ttu-id="c2cc0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2cc0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2cc0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c2cc0-127">Accept</span></span>|<span data-ttu-id="c2cc0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c2cc0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2cc0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2cc0-129">Request body</span></span>
<span data-ttu-id="c2cc0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2cc0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2cc0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2cc0-131">Response</span></span>
<span data-ttu-id="c2cc0-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2cc0-132">If successful, this method returns a `200 OK` response code and [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2cc0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c2cc0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2cc0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2cc0-134">Request</span></span>
<span data-ttu-id="c2cc0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2cc0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="c2cc0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2cc0-136">Response</span></span>
<span data-ttu-id="c2cc0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2cc0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1859

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81AppX",
    "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
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
    "phoneProductIdentifier": "Phone Product Identifier value",
    "phonePublisherId": "Phone Publisher Id value",
    "identityVersion": "Identity Version value"
  }
}
```





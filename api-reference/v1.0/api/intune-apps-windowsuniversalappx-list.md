---
title: Перечисление объектов windowsUniversalAppX
description: Список свойств и связей объектов windowsUniversalAppX.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 128df90dade0e4e1782f519e2439576da11e3525
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464456"
---
# <a name="list-windowsuniversalappxs"></a><span data-ttu-id="72c48-103">Перечисление объектов windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="72c48-103">List windowsUniversalAppXs</span></span>

<span data-ttu-id="72c48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72c48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72c48-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72c48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72c48-106">Список свойств и связей объектов [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="72c48-106">List properties and relationships of the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72c48-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="72c48-107">Prerequisites</span></span>
<span data-ttu-id="72c48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72c48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72c48-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72c48-110">Permission type</span></span>|<span data-ttu-id="72c48-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72c48-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72c48-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72c48-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72c48-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c48-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="72c48-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72c48-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72c48-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72c48-115">Not supported.</span></span>|
|<span data-ttu-id="72c48-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72c48-116">Application</span></span>|<span data-ttu-id="72c48-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72c48-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72c48-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72c48-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="72c48-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="72c48-119">Request headers</span></span>
|<span data-ttu-id="72c48-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72c48-120">Header</span></span>|<span data-ttu-id="72c48-121">Значение</span><span class="sxs-lookup"><span data-stu-id="72c48-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72c48-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72c48-122">Authorization</span></span>|<span data-ttu-id="72c48-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72c48-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72c48-124">Accept</span><span class="sxs-lookup"><span data-stu-id="72c48-124">Accept</span></span>|<span data-ttu-id="72c48-125">application/json</span><span class="sxs-lookup"><span data-stu-id="72c48-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72c48-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="72c48-126">Request body</span></span>
<span data-ttu-id="72c48-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72c48-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72c48-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="72c48-128">Response</span></span>
<span data-ttu-id="72c48-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72c48-129">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72c48-130">Пример</span><span class="sxs-lookup"><span data-stu-id="72c48-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="72c48-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="72c48-131">Request</span></span>
<span data-ttu-id="72c48-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72c48-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="72c48-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="72c48-133">Response</span></span>
<span data-ttu-id="72c48-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72c48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1534

{
  "value": [
    {
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
      "publishingState": "processing",
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
        "v10_0": true
      },
      "identityVersion": "Identity Version value"
    }
  ]
}
```







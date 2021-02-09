---
title: Список windowsPhone81AppX
description: Список свойств и связей объектов windowsPhone81AppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8e448744053bb36182294673a1c23ded6d6dc5fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156191"
---
# <a name="list-windowsphone81appxs"></a><span data-ttu-id="73bc9-103">Список windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="73bc9-103">List windowsPhone81AppXs</span></span>

<span data-ttu-id="73bc9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73bc9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73bc9-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73bc9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73bc9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73bc9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73bc9-107">Список свойств и связей объектов [windowsPhone81AppX.](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="73bc9-107">List properties and relationships of the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73bc9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="73bc9-108">Prerequisites</span></span>
<span data-ttu-id="73bc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73bc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73bc9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73bc9-111">Permission type</span></span>|<span data-ttu-id="73bc9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73bc9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73bc9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73bc9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73bc9-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="73bc9-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="73bc9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73bc9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73bc9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73bc9-116">Not supported.</span></span>|
|<span data-ttu-id="73bc9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73bc9-117">Application</span></span>|<span data-ttu-id="73bc9-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="73bc9-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73bc9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73bc9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="73bc9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="73bc9-120">Request headers</span></span>
|<span data-ttu-id="73bc9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73bc9-121">Header</span></span>|<span data-ttu-id="73bc9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="73bc9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73bc9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73bc9-123">Authorization</span></span>|<span data-ttu-id="73bc9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73bc9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73bc9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="73bc9-125">Accept</span></span>|<span data-ttu-id="73bc9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73bc9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73bc9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73bc9-127">Request body</span></span>
<span data-ttu-id="73bc9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73bc9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73bc9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="73bc9-129">Response</span></span>
<span data-ttu-id="73bc9-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73bc9-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73bc9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="73bc9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="73bc9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="73bc9-132">Request</span></span>
<span data-ttu-id="73bc9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73bc9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="73bc9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="73bc9-134">Response</span></span>
<span data-ttu-id="73bc9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73bc9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2025

{
  "value": [
    {
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
        "v10_1903": true,
        "v10_1909": true,
        "v10_2004": true
      },
      "phoneProductIdentifier": "Phone Product Identifier value",
      "phonePublisherId": "Phone Publisher Id value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```





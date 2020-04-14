---
title: Список windowsPhone81AppXBundles
description: Список свойств и связей объектов windowsPhone81AppXBundle.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4345a930e816361a09d25a0fcf89c6bf4f42e421
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43393571"
---
# <a name="list-windowsphone81appxbundles"></a><span data-ttu-id="7ce0a-103">Список windowsPhone81AppXBundles</span><span class="sxs-lookup"><span data-stu-id="7ce0a-103">List windowsPhone81AppXBundles</span></span>

<span data-ttu-id="7ce0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ce0a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ce0a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ce0a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ce0a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ce0a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ce0a-107">Список свойств и связей объектов [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="7ce0a-107">List properties and relationships of the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ce0a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7ce0a-108">Prerequisites</span></span>
<span data-ttu-id="7ce0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ce0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ce0a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ce0a-111">Permission type</span></span>|<span data-ttu-id="7ce0a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ce0a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ce0a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ce0a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ce0a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ce0a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7ce0a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ce0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ce0a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ce0a-116">Not supported.</span></span>|
|<span data-ttu-id="7ce0a-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="7ce0a-117">Application</span></span>|<span data-ttu-id="7ce0a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ce0a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ce0a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ce0a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7ce0a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7ce0a-120">Request headers</span></span>
|<span data-ttu-id="7ce0a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ce0a-121">Header</span></span>|<span data-ttu-id="7ce0a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7ce0a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ce0a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ce0a-123">Authorization</span></span>|<span data-ttu-id="7ce0a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ce0a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ce0a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7ce0a-125">Accept</span></span>|<span data-ttu-id="7ce0a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ce0a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ce0a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ce0a-127">Request body</span></span>
<span data-ttu-id="7ce0a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ce0a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ce0a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ce0a-129">Response</span></span>
<span data-ttu-id="7ce0a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7ce0a-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ce0a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7ce0a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ce0a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ce0a-132">Request</span></span>
<span data-ttu-id="7ce0a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ce0a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="7ce0a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ce0a-134">Response</span></span>
<span data-ttu-id="7ce0a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ce0a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2796

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
      "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
      "identityVersion": "Identity Version value",
      "appXPackageInformationList": [
        {
          "@odata.type": "microsoft.graph.windowsPackageInformation",
          "applicableArchitecture": "x86",
          "displayName": "Display Name value",
          "identityName": "Identity Name value",
          "identityPublisher": "Identity Publisher value",
          "identityResourceIdentifier": "Identity Resource Identifier value",
          "identityVersion": "Identity Version value",
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
          }
        }
      ]
    }
  ]
}
```




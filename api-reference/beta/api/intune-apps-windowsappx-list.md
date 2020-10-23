---
title: Список Виндовсаппксс
description: Список свойств и связей объектов windowsAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc68115ea945f15aa48f37040728b9761277bcbd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727945"
---
# <a name="list-windowsappxs"></a><span data-ttu-id="0cd59-103">Список Виндовсаппксс</span><span class="sxs-lookup"><span data-stu-id="0cd59-103">List windowsAppXs</span></span>

<span data-ttu-id="0cd59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cd59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cd59-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cd59-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cd59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cd59-107">Список свойств и связей объектов [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="0cd59-107">List properties and relationships of the [windowsAppX](../resources/intune-apps-windowsappx.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cd59-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0cd59-108">Prerequisites</span></span>
<span data-ttu-id="0cd59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cd59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd59-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cd59-111">Permission type</span></span>|<span data-ttu-id="0cd59-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cd59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cd59-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cd59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0cd59-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cd59-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0cd59-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cd59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cd59-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd59-116">Not supported.</span></span>|
|<span data-ttu-id="0cd59-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0cd59-117">Application</span></span>|<span data-ttu-id="0cd59-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cd59-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cd59-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cd59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0cd59-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0cd59-120">Request headers</span></span>
|<span data-ttu-id="0cd59-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0cd59-121">Header</span></span>|<span data-ttu-id="0cd59-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0cd59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cd59-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0cd59-123">Authorization</span></span>|<span data-ttu-id="0cd59-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cd59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cd59-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0cd59-125">Accept</span></span>|<span data-ttu-id="0cd59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0cd59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cd59-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0cd59-127">Request body</span></span>
<span data-ttu-id="0cd59-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0cd59-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cd59-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0cd59-129">Response</span></span>
<span data-ttu-id="0cd59-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windowsAppX](../resources/intune-apps-windowsappx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0cd59-130">If successful, this method returns a `200 OK` response code and a collection of [windowsAppX](../resources/intune-apps-windowsappx.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd59-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0cd59-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cd59-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cd59-132">Request</span></span>
<span data-ttu-id="0cd59-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cd59-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="0cd59-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cd59-134">Response</span></span>
<span data-ttu-id="0cd59-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0cd59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1867

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAppX",
      "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  ]
}
```






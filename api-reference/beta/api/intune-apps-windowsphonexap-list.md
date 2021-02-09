---
title: Список windowsPhoneXAP
description: Список свойств и связей объектов windowsPhoneXAP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e3ac1e2e7dac62a23a0efe42f2b8204165780c4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155302"
---
# <a name="list-windowsphonexaps"></a><span data-ttu-id="fba5e-103">Список windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="fba5e-103">List windowsPhoneXAPs</span></span>

<span data-ttu-id="fba5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fba5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fba5e-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fba5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fba5e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fba5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fba5e-107">Список свойств и связей объектов [windowsPhoneXAP.](../resources/intune-apps-windowsphonexap.md)</span><span class="sxs-lookup"><span data-stu-id="fba5e-107">List properties and relationships of the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fba5e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fba5e-108">Prerequisites</span></span>
<span data-ttu-id="fba5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fba5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fba5e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fba5e-111">Permission type</span></span>|<span data-ttu-id="fba5e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fba5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fba5e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fba5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fba5e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fba5e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fba5e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fba5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fba5e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fba5e-116">Not supported.</span></span>|
|<span data-ttu-id="fba5e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fba5e-117">Application</span></span>|<span data-ttu-id="fba5e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fba5e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fba5e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fba5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fba5e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fba5e-120">Request headers</span></span>
|<span data-ttu-id="fba5e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fba5e-121">Header</span></span>|<span data-ttu-id="fba5e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fba5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fba5e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fba5e-123">Authorization</span></span>|<span data-ttu-id="fba5e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fba5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fba5e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fba5e-125">Accept</span></span>|<span data-ttu-id="fba5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fba5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fba5e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fba5e-127">Request body</span></span>
<span data-ttu-id="fba5e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fba5e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fba5e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fba5e-129">Response</span></span>
<span data-ttu-id="fba5e-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fba5e-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fba5e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fba5e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fba5e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fba5e-132">Request</span></span>
<span data-ttu-id="fba5e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fba5e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="fba5e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fba5e-134">Response</span></span>
<span data-ttu-id="fba5e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fba5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1729

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhoneXAP",
      "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
      "productIdentifier": "Product Identifier value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```





---
title: Перечисление объектов mobileLobApp
description: Список свойств и связей объектов mobileLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40089b498bd72993b9417bd34d38eb097941386e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976958"
---
# <a name="list-mobilelobapps"></a><span data-ttu-id="2e278-103">Перечисление объектов mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="2e278-103">List mobileLobApps</span></span>

<span data-ttu-id="2e278-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e278-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e278-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e278-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e278-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e278-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e278-107">Список свойств и связей объектов [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e278-107">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e278-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2e278-108">Prerequisites</span></span>
<span data-ttu-id="2e278-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e278-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e278-111">Permission type</span></span>|<span data-ttu-id="2e278-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e278-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e278-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e278-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e278-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e278-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2e278-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e278-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e278-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e278-116">Not supported.</span></span>|
|<span data-ttu-id="2e278-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e278-117">Application</span></span>|<span data-ttu-id="2e278-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e278-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e278-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e278-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2e278-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2e278-120">Request headers</span></span>
|<span data-ttu-id="2e278-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e278-121">Header</span></span>|<span data-ttu-id="2e278-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2e278-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e278-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e278-123">Authorization</span></span>|<span data-ttu-id="2e278-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e278-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e278-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2e278-125">Accept</span></span>|<span data-ttu-id="2e278-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e278-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e278-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2e278-127">Request body</span></span>
<span data-ttu-id="2e278-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e278-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e278-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e278-129">Response</span></span>
<span data-ttu-id="2e278-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileLobApp](../resources/intune-apps-mobilelobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e278-130">If successful, this method returns a `200 OK` response code and a collection of [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e278-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2e278-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e278-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e278-132">Request</span></span>
<span data-ttu-id="2e278-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e278-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="2e278-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e278-134">Response</span></span>
<span data-ttu-id="2e278-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e278-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1206

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileLobApp",
      "id": "2fc11935-1935-2fc1-3519-c12f3519c12f",
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
      "size": 4
    }
  ]
}
```







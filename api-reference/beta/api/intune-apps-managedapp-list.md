---
title: Перечисление объектов managedApp
description: Список свойств и связей объектов managedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 61a60fdb70e88b9f99e410bda91057a23dff8340
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451051"
---
# <a name="list-managedapps"></a><span data-ttu-id="4a6c0-103">Перечисление объектов managedApp</span><span class="sxs-lookup"><span data-stu-id="4a6c0-103">List managedApps</span></span>

<span data-ttu-id="4a6c0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4a6c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a6c0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a6c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a6c0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a6c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a6c0-107">Список свойств и связей объектов [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="4a6c0-107">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a6c0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4a6c0-108">Prerequisites</span></span>
<span data-ttu-id="4a6c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a6c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a6c0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a6c0-111">Permission type</span></span>|<span data-ttu-id="4a6c0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a6c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a6c0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a6c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a6c0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a6c0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4a6c0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a6c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a6c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a6c0-116">Not supported.</span></span>|
|<span data-ttu-id="4a6c0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a6c0-117">Application</span></span>|<span data-ttu-id="4a6c0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a6c0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a6c0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a6c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4a6c0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4a6c0-120">Request headers</span></span>
|<span data-ttu-id="4a6c0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a6c0-121">Header</span></span>|<span data-ttu-id="4a6c0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4a6c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a6c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a6c0-123">Authorization</span></span>|<span data-ttu-id="4a6c0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a6c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a6c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4a6c0-125">Accept</span></span>|<span data-ttu-id="4a6c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a6c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a6c0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a6c0-127">Request body</span></span>
<span data-ttu-id="4a6c0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a6c0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a6c0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a6c0-129">Response</span></span>
<span data-ttu-id="4a6c0-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedApp](../resources/intune-apps-managedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a6c0-130">If successful, this method returns a `200 OK` response code and a collection of [managedApp](../resources/intune-apps-managedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a6c0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4a6c0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a6c0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a6c0-132">Request</span></span>
<span data-ttu-id="4a6c0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a6c0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="4a6c0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a6c0-134">Response</span></span>
<span data-ttu-id="4a6c0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a6c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1093

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedApp",
      "id": "f687dd85-dd85-f687-85dd-87f685dd87f6",
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
      "appAvailability": "lineOfBusiness",
      "version": "Version value"
    }
  ]
}
```






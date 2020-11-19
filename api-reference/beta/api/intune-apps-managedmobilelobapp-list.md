---
title: Перечисление объектов managedMobileLobApp
description: Список свойств и связей объектов managedMobileLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a63cb12a1ad62b3ab104a7b30018dadbf1647419
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49249478"
---
# <a name="list-managedmobilelobapps"></a><span data-ttu-id="0bf17-103">Перечисление объектов managedMobileLobApp</span><span class="sxs-lookup"><span data-stu-id="0bf17-103">List managedMobileLobApps</span></span>

<span data-ttu-id="0bf17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bf17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bf17-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bf17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bf17-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bf17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bf17-107">Список свойств и связей объектов [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0bf17-107">List properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bf17-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0bf17-108">Prerequisites</span></span>
<span data-ttu-id="0bf17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bf17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bf17-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bf17-111">Permission type</span></span>|<span data-ttu-id="0bf17-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bf17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bf17-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bf17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bf17-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bf17-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0bf17-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bf17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bf17-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bf17-116">Not supported.</span></span>|
|<span data-ttu-id="0bf17-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0bf17-117">Application</span></span>|<span data-ttu-id="0bf17-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bf17-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bf17-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bf17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0bf17-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0bf17-120">Request headers</span></span>
|<span data-ttu-id="0bf17-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0bf17-121">Header</span></span>|<span data-ttu-id="0bf17-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0bf17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bf17-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0bf17-123">Authorization</span></span>|<span data-ttu-id="0bf17-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bf17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bf17-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0bf17-125">Accept</span></span>|<span data-ttu-id="0bf17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bf17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bf17-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0bf17-127">Request body</span></span>
<span data-ttu-id="0bf17-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0bf17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bf17-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bf17-129">Response</span></span>
<span data-ttu-id="0bf17-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0bf17-130">If successful, this method returns a `200 OK` response code and a collection of [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bf17-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0bf17-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bf17-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bf17-132">Request</span></span>
<span data-ttu-id="0bf17-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0bf17-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="0bf17-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bf17-134">Response</span></span>
<span data-ttu-id="0bf17-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0bf17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1292

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedMobileLobApp",
      "id": "cded7cc4-7cc4-cded-c47c-edcdc47cedcd",
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
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4
    }
  ]
}
```





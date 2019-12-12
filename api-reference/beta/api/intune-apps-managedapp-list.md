---
title: Перечисление объектов managedApp
description: Список свойств и связей объектов managedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0fbd02d45d47f748b7354f3a6ae23d6e99a71dc8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39951742"
---
# <a name="list-managedapps"></a><span data-ttu-id="6dc4c-103">Перечисление объектов managedApp</span><span class="sxs-lookup"><span data-stu-id="6dc4c-103">List managedApps</span></span>

> <span data-ttu-id="6dc4c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dc4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dc4c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6dc4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dc4c-106">Список свойств и связей объектов [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="6dc4c-106">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dc4c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6dc4c-107">Prerequisites</span></span>
<span data-ttu-id="6dc4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dc4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dc4c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dc4c-110">Permission type</span></span>|<span data-ttu-id="6dc4c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dc4c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dc4c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dc4c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6dc4c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dc4c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6dc4c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dc4c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dc4c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dc4c-115">Not supported.</span></span>|
|<span data-ttu-id="6dc4c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6dc4c-116">Application</span></span>|<span data-ttu-id="6dc4c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dc4c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dc4c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dc4c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6dc4c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6dc4c-119">Request headers</span></span>
|<span data-ttu-id="6dc4c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6dc4c-120">Header</span></span>|<span data-ttu-id="6dc4c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6dc4c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dc4c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dc4c-122">Authorization</span></span>|<span data-ttu-id="6dc4c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dc4c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dc4c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6dc4c-124">Accept</span></span>|<span data-ttu-id="6dc4c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6dc4c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dc4c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6dc4c-126">Request body</span></span>
<span data-ttu-id="6dc4c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6dc4c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dc4c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="6dc4c-128">Response</span></span>
<span data-ttu-id="6dc4c-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedApp](../resources/intune-apps-managedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6dc4c-129">If successful, this method returns a `200 OK` response code and a collection of [managedApp](../resources/intune-apps-managedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dc4c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6dc4c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dc4c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dc4c-131">Request</span></span>
<span data-ttu-id="6dc4c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dc4c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="6dc4c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dc4c-133">Response</span></span>
<span data-ttu-id="6dc4c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6dc4c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






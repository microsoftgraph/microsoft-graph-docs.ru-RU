---
title: Список officeSuiteApps
description: Свойства списка и связей объектов officeSuiteApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 173503a4ecef31b75ae0d2a4a1dc29b4f5de2d48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417422"
---
# <a name="list-officesuiteapps"></a><span data-ttu-id="81280-103">Список officeSuiteApps</span><span class="sxs-lookup"><span data-stu-id="81280-103">List officeSuiteApps</span></span>

> <span data-ttu-id="81280-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="81280-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="81280-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81280-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81280-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81280-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81280-107">Свойства списка и связей объектов [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="81280-107">List properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81280-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="81280-108">Prerequisites</span></span>
<span data-ttu-id="81280-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="81280-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="81280-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81280-111">Permission type</span></span>|<span data-ttu-id="81280-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81280-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81280-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81280-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81280-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="81280-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="81280-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81280-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81280-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81280-116">Not supported.</span></span>|
|<span data-ttu-id="81280-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81280-117">Application</span></span>|<span data-ttu-id="81280-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81280-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81280-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81280-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="81280-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81280-120">Request headers</span></span>
|<span data-ttu-id="81280-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81280-121">Header</span></span>|<span data-ttu-id="81280-122">Значение</span><span class="sxs-lookup"><span data-stu-id="81280-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81280-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="81280-123">Authorization</span></span>|<span data-ttu-id="81280-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="81280-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81280-125">Accept</span><span class="sxs-lookup"><span data-stu-id="81280-125">Accept</span></span>|<span data-ttu-id="81280-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81280-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81280-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81280-127">Request body</span></span>
<span data-ttu-id="81280-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81280-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81280-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="81280-129">Response</span></span>
<span data-ttu-id="81280-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="81280-130">If successful, this method returns a `200 OK` response code and a collection of [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81280-131">Пример</span><span class="sxs-lookup"><span data-stu-id="81280-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="81280-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="81280-132">Request</span></span>
<span data-ttu-id="81280-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81280-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="81280-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="81280-134">Response</span></span>
<span data-ttu-id="81280-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="81280-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1977

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeSuiteApp",
      "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
      "autoAcceptEula": true,
      "productIds": [
        "o365BusinessRetail"
      ],
      "excludedApps": {
        "@odata.type": "microsoft.graph.excludedApps",
        "access": true,
        "excel": true,
        "groove": true,
        "infoPath": true,
        "lync": true,
        "oneDrive": true,
        "oneNote": true,
        "outlook": true,
        "powerPoint": true,
        "publisher": true,
        "sharePointDesigner": true,
        "visio": true,
        "word": true
      },
      "useSharedComputerActivation": true,
      "updateChannel": "current",
      "officePlatformArchitecture": "x86",
      "localesToInstall": [
        "Locales To Install value"
      ],
      "installProgressDisplayLevel": "full",
      "shouldUninstallOlderVersionsOfOffice": true,
      "targetVersion": "Target Version value",
      "updateVersion": "Update Version value",
      "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
    }
  ]
}
```





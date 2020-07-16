---
title: Получение officeSuiteApp
description: Чтение свойств и связей объекта officeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ceabdbab0d69b45d800c8292c9fb1528f834a2b7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793292"
---
# <a name="get-officesuiteapp"></a><span data-ttu-id="3da4c-103">Получение officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="3da4c-103">Get officeSuiteApp</span></span>

<span data-ttu-id="3da4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3da4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3da4c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3da4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3da4c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3da4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3da4c-107">Чтение свойств и связей объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3da4c-107">Read properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3da4c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3da4c-108">Prerequisites</span></span>
<span data-ttu-id="3da4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3da4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3da4c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3da4c-111">Permission type</span></span>|<span data-ttu-id="3da4c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3da4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3da4c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3da4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3da4c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3da4c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3da4c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3da4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3da4c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3da4c-116">Not supported.</span></span>|
|<span data-ttu-id="3da4c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3da4c-117">Application</span></span>|<span data-ttu-id="3da4c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3da4c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3da4c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3da4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3da4c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3da4c-120">Optional query parameters</span></span>
<span data-ttu-id="3da4c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3da4c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3da4c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3da4c-122">Request headers</span></span>
|<span data-ttu-id="3da4c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3da4c-123">Header</span></span>|<span data-ttu-id="3da4c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="3da4c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3da4c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3da4c-125">Authorization</span></span>|<span data-ttu-id="3da4c-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3da4c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3da4c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="3da4c-127">Accept</span></span>|<span data-ttu-id="3da4c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3da4c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3da4c-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3da4c-129">Request body</span></span>
<span data-ttu-id="3da4c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3da4c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3da4c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3da4c-131">Response</span></span>
<span data-ttu-id="3da4c-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3da4c-132">If successful, this method returns a `200 OK` response code and [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3da4c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3da4c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3da4c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3da4c-134">Request</span></span>
<span data-ttu-id="3da4c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3da4c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="3da4c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3da4c-136">Response</span></span>
<span data-ttu-id="3da4c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3da4c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1925

{
  "value": {
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
    "dependentAppCount": 1,
    "autoAcceptEula": true,
    "productIds": [
      "o365BusinessRetail"
    ],
    "excludedApps": {
      "@odata.type": "microsoft.graph.excludedApps",
      "access": true,
      "bing": true,
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
      "teams": true,
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
}
```




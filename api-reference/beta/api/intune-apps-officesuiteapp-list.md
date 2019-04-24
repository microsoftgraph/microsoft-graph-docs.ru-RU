---
title: Список Оффицесуитеаппс
description: Список свойств и связей объектов officeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfcd54d0f7bf00a7db291046a754361b9d9ee0e3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32488480"
---
# <a name="list-officesuiteapps"></a><span data-ttu-id="2f2a8-103">Список Оффицесуитеаппс</span><span class="sxs-lookup"><span data-stu-id="2f2a8-103">List officeSuiteApps</span></span>

> <span data-ttu-id="2f2a8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f2a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f2a8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f2a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f2a8-106">Список свойств и связей объектов [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="2f2a8-106">List properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f2a8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2f2a8-107">Prerequisites</span></span>
<span data-ttu-id="2f2a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f2a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f2a8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f2a8-110">Permission type</span></span>|<span data-ttu-id="2f2a8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f2a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f2a8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f2a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f2a8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f2a8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2f2a8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f2a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f2a8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f2a8-115">Not supported.</span></span>|
|<span data-ttu-id="2f2a8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f2a8-116">Application</span></span>|<span data-ttu-id="2f2a8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f2a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f2a8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f2a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2f2a8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f2a8-119">Request headers</span></span>
|<span data-ttu-id="2f2a8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f2a8-120">Header</span></span>|<span data-ttu-id="2f2a8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2f2a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f2a8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f2a8-122">Authorization</span></span>|<span data-ttu-id="2f2a8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f2a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f2a8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2f2a8-124">Accept</span></span>|<span data-ttu-id="2f2a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f2a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f2a8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f2a8-126">Request body</span></span>
<span data-ttu-id="2f2a8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f2a8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f2a8-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f2a8-128">Response</span></span>
<span data-ttu-id="2f2a8-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f2a8-129">If successful, this method returns a `200 OK` response code and a collection of [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f2a8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2f2a8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f2a8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f2a8-131">Request</span></span>
<span data-ttu-id="2f2a8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f2a8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="2f2a8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f2a8-133">Response</span></span>
<span data-ttu-id="2f2a8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f2a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2032

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
      "dependentAppCount": 1,
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
  ]
}
```






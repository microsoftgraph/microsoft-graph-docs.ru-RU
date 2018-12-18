---
title: Получение officeSuiteApp
description: Чтение свойства и связи объекта officeSuiteApp.
author: tfitzmac
ms.openlocfilehash: e90833113bdb626d5d61d9c52027efdd6cc6b073
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348729"
---
# <a name="get-officesuiteapp"></a><span data-ttu-id="92bff-103">Получение officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="92bff-103">Get officeSuiteApp</span></span>

> <span data-ttu-id="92bff-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="92bff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92bff-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92bff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92bff-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="92bff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92bff-107">Чтение свойства и связи объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="92bff-107">Read properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92bff-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="92bff-108">Prerequisites</span></span>
<span data-ttu-id="92bff-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92bff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92bff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92bff-111">Permission type</span></span>|<span data-ttu-id="92bff-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92bff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92bff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92bff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92bff-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="92bff-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="92bff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92bff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92bff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92bff-116">Not supported.</span></span>|
|<span data-ttu-id="92bff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92bff-117">Application</span></span>|<span data-ttu-id="92bff-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92bff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92bff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92bff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92bff-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="92bff-120">Optional query parameters</span></span>
<span data-ttu-id="92bff-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="92bff-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="92bff-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92bff-122">Request headers</span></span>
|<span data-ttu-id="92bff-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92bff-123">Header</span></span>|<span data-ttu-id="92bff-124">Значение</span><span class="sxs-lookup"><span data-stu-id="92bff-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92bff-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92bff-125">Authorization</span></span>|<span data-ttu-id="92bff-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="92bff-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92bff-127">Accept</span><span class="sxs-lookup"><span data-stu-id="92bff-127">Accept</span></span>|<span data-ttu-id="92bff-128">application/json</span><span class="sxs-lookup"><span data-stu-id="92bff-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92bff-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92bff-129">Request body</span></span>
<span data-ttu-id="92bff-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92bff-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92bff-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="92bff-131">Response</span></span>
<span data-ttu-id="92bff-132">Успешно завершена, этот метод возвращает `200 OK` объект [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="92bff-132">If successful, this method returns a `200 OK` response code and [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92bff-133">Пример</span><span class="sxs-lookup"><span data-stu-id="92bff-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="92bff-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="92bff-134">Request</span></span>
<span data-ttu-id="92bff-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92bff-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="92bff-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="92bff-136">Response</span></span>
<span data-ttu-id="92bff-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="92bff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1693

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
    "updateVersion": "Update Version value"
  }
}
```






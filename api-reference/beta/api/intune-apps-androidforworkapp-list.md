---
title: Список Андроидфорворкаппс
description: Список свойств и связей объектов Андроидфорворкапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d3b190662b4e5af4f0575a16f562c44b2d3a507
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173936"
---
# <a name="list-androidforworkapps"></a><span data-ttu-id="97a1e-103">Список Андроидфорворкаппс</span><span class="sxs-lookup"><span data-stu-id="97a1e-103">List androidForWorkApps</span></span>

> <span data-ttu-id="97a1e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97a1e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97a1e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97a1e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97a1e-106">Список свойств и связей объектов [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="97a1e-106">List properties and relationships of the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97a1e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="97a1e-107">Prerequisites</span></span>
<span data-ttu-id="97a1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97a1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97a1e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97a1e-110">Permission type</span></span>|<span data-ttu-id="97a1e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97a1e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97a1e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97a1e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97a1e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a1e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="97a1e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97a1e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97a1e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97a1e-115">Not supported.</span></span>|
|<span data-ttu-id="97a1e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97a1e-116">Application</span></span>|<span data-ttu-id="97a1e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a1e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97a1e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97a1e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="97a1e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97a1e-119">Request headers</span></span>
|<span data-ttu-id="97a1e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97a1e-120">Header</span></span>|<span data-ttu-id="97a1e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="97a1e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97a1e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97a1e-122">Authorization</span></span>|<span data-ttu-id="97a1e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97a1e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97a1e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="97a1e-124">Accept</span></span>|<span data-ttu-id="97a1e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97a1e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97a1e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="97a1e-126">Request body</span></span>
<span data-ttu-id="97a1e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97a1e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97a1e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="97a1e-128">Response</span></span>
<span data-ttu-id="97a1e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97a1e-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97a1e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="97a1e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="97a1e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="97a1e-131">Request</span></span>
<span data-ttu-id="97a1e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97a1e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="97a1e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="97a1e-133">Response</span></span>
<span data-ttu-id="97a1e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97a1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1228

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkApp",
      "id": "c5010785-0785-c501-8507-01c5850701c5",
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
      "packageId": "Package Id value",
      "appIdentifier": "App Identifier value",
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "appStoreUrl": "https://example.com/appStoreUrl/"
    }
  ]
}
```





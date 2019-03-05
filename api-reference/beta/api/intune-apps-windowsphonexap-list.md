---
title: Список Виндовсфонексапс
description: Список свойств и связей объектов Виндовсфонексап.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1cb87e6cbd34b63091cb7e5398b252c732486c71
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145698"
---
# <a name="list-windowsphonexaps"></a><span data-ttu-id="0d253-103">Список Виндовсфонексапс</span><span class="sxs-lookup"><span data-stu-id="0d253-103">List windowsPhoneXAPs</span></span>

> <span data-ttu-id="0d253-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d253-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d253-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d253-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d253-106">Список свойств и связей объектов [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="0d253-106">List properties and relationships of the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d253-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0d253-107">Prerequisites</span></span>
<span data-ttu-id="0d253-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0d253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0d253-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d253-110">Permission type</span></span>|<span data-ttu-id="0d253-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d253-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d253-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d253-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d253-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d253-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0d253-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d253-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d253-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d253-115">Not supported.</span></span>|
|<span data-ttu-id="0d253-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d253-116">Application</span></span>|<span data-ttu-id="0d253-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d253-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d253-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d253-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0d253-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d253-119">Request headers</span></span>
|<span data-ttu-id="0d253-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d253-120">Header</span></span>|<span data-ttu-id="0d253-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0d253-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d253-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d253-122">Authorization</span></span>|<span data-ttu-id="0d253-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0d253-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d253-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0d253-124">Accept</span></span>|<span data-ttu-id="0d253-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d253-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d253-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d253-126">Request body</span></span>
<span data-ttu-id="0d253-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d253-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d253-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d253-128">Response</span></span>
<span data-ttu-id="0d253-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d253-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d253-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0d253-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d253-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d253-131">Request</span></span>
<span data-ttu-id="0d253-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d253-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="0d253-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d253-133">Response</span></span>
<span data-ttu-id="0d253-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d253-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1525

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
        "v10_1803": true
      },
      "productIdentifier": "Product Identifier value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```





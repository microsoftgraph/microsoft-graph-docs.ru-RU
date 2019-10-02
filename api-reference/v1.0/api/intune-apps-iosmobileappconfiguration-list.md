---
title: Список iosMobileAppConfigurations
description: Список свойств и связей объектов iosMobileAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 62a1c109265f172eb470d12fe7a765027c4eaeae
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355612"
---
# <a name="list-iosmobileappconfigurations"></a><span data-ttu-id="35210-103">Список iosMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="35210-103">List iosMobileAppConfigurations</span></span>

> <span data-ttu-id="35210-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35210-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35210-105">Список свойств и связей объектов [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35210-105">List properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35210-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="35210-106">Prerequisites</span></span>
<span data-ttu-id="35210-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35210-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35210-109">Permission type</span></span>|<span data-ttu-id="35210-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35210-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35210-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35210-111">Delegated (work or school account)</span></span>|<span data-ttu-id="35210-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="35210-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="35210-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35210-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35210-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35210-114">Not supported.</span></span>|
|<span data-ttu-id="35210-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35210-115">Application</span></span>|<span data-ttu-id="35210-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35210-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35210-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35210-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="35210-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35210-118">Request headers</span></span>
|<span data-ttu-id="35210-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35210-119">Header</span></span>|<span data-ttu-id="35210-120">Значение</span><span class="sxs-lookup"><span data-stu-id="35210-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35210-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35210-121">Authorization</span></span>|<span data-ttu-id="35210-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35210-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35210-123">Accept</span><span class="sxs-lookup"><span data-stu-id="35210-123">Accept</span></span>|<span data-ttu-id="35210-124">application/json</span><span class="sxs-lookup"><span data-stu-id="35210-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35210-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35210-125">Request body</span></span>
<span data-ttu-id="35210-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35210-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35210-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="35210-127">Response</span></span>
<span data-ttu-id="35210-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="35210-128">If successful, this method returns a `200 OK` response code and a collection of [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35210-129">Пример</span><span class="sxs-lookup"><span data-stu-id="35210-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="35210-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="35210-130">Request</span></span>
<span data-ttu-id="35210-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35210-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="35210-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="35210-132">Response</span></span>
<span data-ttu-id="35210-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35210-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 815

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
      "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
      "settings": [
        {
          "@odata.type": "microsoft.graph.appConfigurationSettingItem",
          "appConfigKey": "App Config Key value",
          "appConfigKeyType": "integerType",
          "appConfigKeyValue": "App Config Key Value value"
        }
      ]
    }
  ]
}
```





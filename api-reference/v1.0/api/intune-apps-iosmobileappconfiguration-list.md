---
title: Список iosMobileAppConfigurations
description: Список свойств и связей объектов iosMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2698bb368ddb00a6c78a9c0ffdda25461e8109a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469046"
---
# <a name="list-iosmobileappconfigurations"></a><span data-ttu-id="a0074-103">Список iosMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="a0074-103">List iosMobileAppConfigurations</span></span>

<span data-ttu-id="a0074-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0074-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0074-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0074-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0074-106">Список свойств и связей объектов [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0074-106">List properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0074-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a0074-107">Prerequisites</span></span>
<span data-ttu-id="a0074-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0074-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0074-110">Permission type</span></span>|<span data-ttu-id="a0074-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0074-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0074-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0074-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0074-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0074-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a0074-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0074-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0074-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0074-115">Not supported.</span></span>|
|<span data-ttu-id="a0074-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0074-116">Application</span></span>|<span data-ttu-id="a0074-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0074-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0074-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0074-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0074-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a0074-119">Request headers</span></span>
|<span data-ttu-id="a0074-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0074-120">Header</span></span>|<span data-ttu-id="a0074-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a0074-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0074-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0074-122">Authorization</span></span>|<span data-ttu-id="a0074-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0074-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0074-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a0074-124">Accept</span></span>|<span data-ttu-id="a0074-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0074-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0074-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a0074-126">Request body</span></span>
<span data-ttu-id="a0074-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0074-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0074-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0074-128">Response</span></span>
<span data-ttu-id="a0074-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a0074-129">If successful, this method returns a `200 OK` response code and a collection of [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0074-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a0074-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0074-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0074-131">Request</span></span>
<span data-ttu-id="a0074-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0074-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="a0074-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0074-133">Response</span></span>
<span data-ttu-id="a0074-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0074-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







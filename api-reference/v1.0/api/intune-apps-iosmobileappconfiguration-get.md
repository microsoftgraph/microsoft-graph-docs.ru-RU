---
title: Получить iosMobileAppConfiguration
description: Чтение списка свойств и связей объекта iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 67dfbd4e16116fa7ad0af0d26e0e6303cf14df15
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002596"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="b71a6-103">Получить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b71a6-103">Get iosMobileAppConfiguration</span></span>

> <span data-ttu-id="b71a6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b71a6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b71a6-105">Чтение списка свойств и связей объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b71a6-105">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b71a6-106">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="b71a6-106">Prerequisites</span></span>
<span data-ttu-id="b71a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b71a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b71a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b71a6-109">Permission type</span></span>|<span data-ttu-id="b71a6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b71a6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b71a6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b71a6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b71a6-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b71a6-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b71a6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b71a6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b71a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b71a6-114">Not supported.</span></span>|
|<span data-ttu-id="b71a6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b71a6-115">Application</span></span>|<span data-ttu-id="b71a6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b71a6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b71a6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b71a6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b71a6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b71a6-118">Optional query parameters</span></span>
<span data-ttu-id="b71a6-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b71a6-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b71a6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b71a6-120">Request headers</span></span>
|<span data-ttu-id="b71a6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b71a6-121">Header</span></span>|<span data-ttu-id="b71a6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b71a6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b71a6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b71a6-123">Authorization</span></span>|<span data-ttu-id="b71a6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b71a6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b71a6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b71a6-125">Accept</span></span>|<span data-ttu-id="b71a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b71a6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b71a6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b71a6-127">Request body</span></span>
<span data-ttu-id="b71a6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b71a6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b71a6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b71a6-129">Response</span></span>
<span data-ttu-id="b71a6-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b71a6-130">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b71a6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b71a6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b71a6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b71a6-132">Request</span></span>
<span data-ttu-id="b71a6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b71a6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b71a6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b71a6-134">Response</span></span>
<span data-ttu-id="b71a6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b71a6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "value": {
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
}
```




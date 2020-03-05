---
title: Получить iosMobileAppConfiguration
description: Чтение списка свойств и связей объекта iosMobileAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cd412cc0fb49789ba4b2dda5a957f6293e302cf6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445675"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="0befd-103">Получить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0befd-103">Get iosMobileAppConfiguration</span></span>

<span data-ttu-id="0befd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0befd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0befd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0befd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0befd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0befd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0befd-107">Чтение списка свойств и связей объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0befd-107">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0befd-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="0befd-108">Prerequisites</span></span>
<span data-ttu-id="0befd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0befd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0befd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0befd-111">Permission type</span></span>|<span data-ttu-id="0befd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0befd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0befd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0befd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0befd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0befd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0befd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0befd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0befd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0befd-116">Not supported.</span></span>|
|<span data-ttu-id="0befd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0befd-117">Application</span></span>|<span data-ttu-id="0befd-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0befd-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0befd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0befd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0befd-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0befd-120">Optional query parameters</span></span>
<span data-ttu-id="0befd-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0befd-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0befd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0befd-122">Request headers</span></span>
|<span data-ttu-id="0befd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0befd-123">Header</span></span>|<span data-ttu-id="0befd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0befd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0befd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0befd-125">Authorization</span></span>|<span data-ttu-id="0befd-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0befd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0befd-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0befd-127">Accept</span></span>|<span data-ttu-id="0befd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0befd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0befd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0befd-129">Request body</span></span>
<span data-ttu-id="0befd-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0befd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0befd-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="0befd-131">Response</span></span>
<span data-ttu-id="0befd-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0befd-132">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0befd-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0befd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0befd-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0befd-134">Request</span></span>
<span data-ttu-id="0befd-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0befd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0befd-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0befd-136">Response</span></span>
<span data-ttu-id="0befd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0befd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 831

{
  "value": {
    "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
    "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
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






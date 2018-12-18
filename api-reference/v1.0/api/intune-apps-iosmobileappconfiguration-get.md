---
title: Получить iosMobileAppConfiguration
description: Считывание свойств и связей объекта iosMobileAppConfiguration.
author: tfitzmac
ms.openlocfilehash: 7566b74e9a0277d0bd5e67b2e76e59faed28cf73
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348022"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="443fe-103">Получить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="443fe-103">Get iosMobileAppConfiguration</span></span>

> <span data-ttu-id="443fe-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="443fe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="443fe-105">Чтение списка свойств и связей объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="443fe-105">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="443fe-106">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="443fe-106">Prerequisites</span></span>
<span data-ttu-id="443fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="443fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="443fe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="443fe-109">Permission type</span></span>|<span data-ttu-id="443fe-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="443fe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="443fe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="443fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="443fe-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="443fe-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="443fe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="443fe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="443fe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="443fe-114">Not supported.</span></span>|
|<span data-ttu-id="443fe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="443fe-115">Application</span></span>|<span data-ttu-id="443fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="443fe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="443fe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="443fe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="443fe-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="443fe-118">Optional query parameters</span></span>
<span data-ttu-id="443fe-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="443fe-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="443fe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="443fe-120">Request headers</span></span>
|<span data-ttu-id="443fe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="443fe-121">Header</span></span>|<span data-ttu-id="443fe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="443fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="443fe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="443fe-123">Authorization</span></span>|<span data-ttu-id="443fe-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="443fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="443fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="443fe-125">Accept</span></span>|<span data-ttu-id="443fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="443fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="443fe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="443fe-127">Request body</span></span>
<span data-ttu-id="443fe-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="443fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="443fe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="443fe-129">Response</span></span>
<span data-ttu-id="443fe-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="443fe-130">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="443fe-131">Пример</span><span class="sxs-lookup"><span data-stu-id="443fe-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="443fe-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="443fe-132">Request</span></span>
<span data-ttu-id="443fe-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="443fe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="443fe-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="443fe-134">Response</span></span>
<span data-ttu-id="443fe-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="443fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




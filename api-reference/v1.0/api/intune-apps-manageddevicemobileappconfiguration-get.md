---
title: Получение объекта managedDeviceMobileAppConfiguration
description: Чтение свойств и связей объекта managedDeviceMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 78b3552052f875bce3aee94969a51aecf5f49393
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867328"
---
# <a name="get-manageddevicemobileappconfiguration"></a><span data-ttu-id="43159-103">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="43159-103">Get managedDeviceMobileAppConfiguration</span></span>

> <span data-ttu-id="43159-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="43159-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43159-105">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43159-105">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43159-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="43159-106">Prerequisites</span></span>
<span data-ttu-id="43159-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43159-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43159-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43159-109">Permission type</span></span>|<span data-ttu-id="43159-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43159-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43159-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43159-111">Delegated (work or school account)</span></span>|<span data-ttu-id="43159-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="43159-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="43159-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43159-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43159-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43159-114">Not supported.</span></span>|
|<span data-ttu-id="43159-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43159-115">Application</span></span>|<span data-ttu-id="43159-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43159-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43159-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43159-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43159-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="43159-118">Optional query parameters</span></span>
<span data-ttu-id="43159-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="43159-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="43159-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43159-120">Request headers</span></span>
|<span data-ttu-id="43159-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43159-121">Header</span></span>|<span data-ttu-id="43159-122">Значение</span><span class="sxs-lookup"><span data-stu-id="43159-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43159-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43159-123">Authorization</span></span>|<span data-ttu-id="43159-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="43159-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43159-125">Accept</span><span class="sxs-lookup"><span data-stu-id="43159-125">Accept</span></span>|<span data-ttu-id="43159-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43159-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43159-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43159-127">Request body</span></span>
<span data-ttu-id="43159-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43159-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43159-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="43159-129">Response</span></span>
<span data-ttu-id="43159-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43159-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43159-131">Пример</span><span class="sxs-lookup"><span data-stu-id="43159-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="43159-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="43159-132">Request</span></span>
<span data-ttu-id="43159-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43159-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="43159-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="43159-134">Response</span></span>
<span data-ttu-id="43159-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="43159-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
    "id": "c60e7591-7591-c60e-9175-0ec691750ec6",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```




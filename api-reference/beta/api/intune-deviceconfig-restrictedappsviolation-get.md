---
title: Получение Рестриктедаппсвиолатион
description: Чтение свойств и связей объекта Рестриктедаппсвиолатион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58f1b2676a9270ebe1421e09d1ac88f77b9635ef
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49270920"
---
# <a name="get-restrictedappsviolation"></a><span data-ttu-id="70017-103">Получение Рестриктедаппсвиолатион</span><span class="sxs-lookup"><span data-stu-id="70017-103">Get restrictedAppsViolation</span></span>

<span data-ttu-id="70017-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70017-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70017-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70017-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70017-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70017-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70017-107">Чтение свойств и связей объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="70017-107">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70017-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="70017-108">Prerequisites</span></span>
<span data-ttu-id="70017-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70017-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70017-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70017-111">Permission type</span></span>|<span data-ttu-id="70017-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70017-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70017-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70017-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70017-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="70017-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="70017-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70017-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70017-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70017-116">Not supported.</span></span>|
|<span data-ttu-id="70017-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="70017-117">Application</span></span>|<span data-ttu-id="70017-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="70017-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70017-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70017-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70017-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70017-120">Optional query parameters</span></span>
<span data-ttu-id="70017-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="70017-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70017-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70017-122">Request headers</span></span>
|<span data-ttu-id="70017-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70017-123">Header</span></span>|<span data-ttu-id="70017-124">Значение</span><span class="sxs-lookup"><span data-stu-id="70017-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70017-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70017-125">Authorization</span></span>|<span data-ttu-id="70017-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70017-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70017-127">Accept</span><span class="sxs-lookup"><span data-stu-id="70017-127">Accept</span></span>|<span data-ttu-id="70017-128">application/json</span><span class="sxs-lookup"><span data-stu-id="70017-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70017-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70017-129">Request body</span></span>
<span data-ttu-id="70017-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70017-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70017-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="70017-131">Response</span></span>
<span data-ttu-id="70017-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70017-132">If successful, this method returns a `200 OK` response code and [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70017-133">Пример</span><span class="sxs-lookup"><span data-stu-id="70017-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="70017-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="70017-134">Request</span></span>
<span data-ttu-id="70017-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70017-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

### <a name="response"></a><span data-ttu-id="70017-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="70017-136">Response</span></span>
<span data-ttu-id="70017-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70017-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 664

{
  "value": {
    "@odata.type": "#microsoft.graph.restrictedAppsViolation",
    "id": "53f99903-9903-53f9-0399-f9530399f953",
    "userId": "User Id value",
    "userName": "User Name value",
    "managedDeviceId": "Managed Device Id value",
    "deviceName": "Device Name value",
    "deviceConfigurationId": "Device Configuration Id value",
    "deviceConfigurationName": "Device Configuration Name value",
    "platformType": "androidForWork",
    "restrictedAppsState": "notApprovedApps",
    "restrictedApps": [
      {
        "@odata.type": "microsoft.graph.managedDeviceReportedApp",
        "appId": "App Id value"
      }
    ]
  }
}
```





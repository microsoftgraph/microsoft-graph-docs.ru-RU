---
title: Получение Рестриктедаппсвиолатион
description: Чтение свойств и связей объекта Рестриктедаппсвиолатион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 87c0ff4faf0bb12de5ee905f508f8b8107f9c8fd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947843"
---
# <a name="get-restrictedappsviolation"></a><span data-ttu-id="c471f-103">Получение Рестриктедаппсвиолатион</span><span class="sxs-lookup"><span data-stu-id="c471f-103">Get restrictedAppsViolation</span></span>

> <span data-ttu-id="c471f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c471f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c471f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c471f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c471f-106">Чтение свойств и связей объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="c471f-106">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c471f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c471f-107">Prerequisites</span></span>
<span data-ttu-id="c471f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c471f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c471f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c471f-110">Permission type</span></span>|<span data-ttu-id="c471f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c471f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c471f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c471f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c471f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c471f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c471f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c471f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c471f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c471f-115">Not supported.</span></span>|
|<span data-ttu-id="c471f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c471f-116">Application</span></span>|<span data-ttu-id="c471f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c471f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c471f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c471f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c471f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c471f-119">Optional query parameters</span></span>
<span data-ttu-id="c471f-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c471f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c471f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c471f-121">Request headers</span></span>
|<span data-ttu-id="c471f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c471f-122">Header</span></span>|<span data-ttu-id="c471f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c471f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c471f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c471f-124">Authorization</span></span>|<span data-ttu-id="c471f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c471f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c471f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c471f-126">Accept</span></span>|<span data-ttu-id="c471f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c471f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c471f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c471f-128">Request body</span></span>
<span data-ttu-id="c471f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c471f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c471f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c471f-130">Response</span></span>
<span data-ttu-id="c471f-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c471f-131">If successful, this method returns a `200 OK` response code and [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c471f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c471f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c471f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c471f-133">Request</span></span>
<span data-ttu-id="c471f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c471f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

### <a name="response"></a><span data-ttu-id="c471f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c471f-135">Response</span></span>
<span data-ttu-id="c471f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c471f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






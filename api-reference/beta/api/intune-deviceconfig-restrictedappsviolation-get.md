---
title: Получение Рестриктедаппсвиолатион
description: Чтение свойств и связей объекта Рестриктедаппсвиолатион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb1c4160a963a91e957a0cc9615d8b90a7236eaa
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971320"
---
# <a name="get-restrictedappsviolation"></a><span data-ttu-id="f870e-103">Получение Рестриктедаппсвиолатион</span><span class="sxs-lookup"><span data-stu-id="f870e-103">Get restrictedAppsViolation</span></span>

> <span data-ttu-id="f870e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f870e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f870e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f870e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f870e-106">Чтение свойств и связей объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="f870e-106">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f870e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f870e-107">Prerequisites</span></span>
<span data-ttu-id="f870e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f870e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f870e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f870e-110">Permission type</span></span>|<span data-ttu-id="f870e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f870e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f870e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f870e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f870e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f870e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f870e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f870e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f870e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f870e-115">Not supported.</span></span>|
|<span data-ttu-id="f870e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f870e-116">Application</span></span>|<span data-ttu-id="f870e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f870e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f870e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f870e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f870e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f870e-119">Optional query parameters</span></span>
<span data-ttu-id="f870e-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f870e-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f870e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f870e-121">Request headers</span></span>
|<span data-ttu-id="f870e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f870e-122">Header</span></span>|<span data-ttu-id="f870e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f870e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f870e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f870e-124">Authorization</span></span>|<span data-ttu-id="f870e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f870e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f870e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f870e-126">Accept</span></span>|<span data-ttu-id="f870e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f870e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f870e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f870e-128">Request body</span></span>
<span data-ttu-id="f870e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f870e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f870e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f870e-130">Response</span></span>
<span data-ttu-id="f870e-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f870e-131">If successful, this method returns a `200 OK` response code and [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f870e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f870e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f870e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f870e-133">Request</span></span>
<span data-ttu-id="f870e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f870e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

### <a name="response"></a><span data-ttu-id="f870e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f870e-135">Response</span></span>
<span data-ttu-id="f870e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f870e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





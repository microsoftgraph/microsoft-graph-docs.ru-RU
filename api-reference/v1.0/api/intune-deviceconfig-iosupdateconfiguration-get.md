---
title: Get iosUpdateConfiguration
description: Чтение свойств и связей объекта iosUpdateConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 89434eef6007a6930ce828b59974f156557ac2c6
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366246"
---
# <a name="get-iosupdateconfiguration"></a><span data-ttu-id="8f1c7-103">Get iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="8f1c7-103">Get iosUpdateConfiguration</span></span>

> <span data-ttu-id="8f1c7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f1c7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f1c7-105">Чтение свойств и связей объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f1c7-105">Read properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f1c7-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8f1c7-106">Prerequisites</span></span>
<span data-ttu-id="8f1c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f1c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f1c7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f1c7-109">Permission type</span></span>|<span data-ttu-id="8f1c7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f1c7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f1c7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f1c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f1c7-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f1c7-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8f1c7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f1c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f1c7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f1c7-114">Not supported.</span></span>|
|<span data-ttu-id="8f1c7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f1c7-115">Application</span></span>|<span data-ttu-id="8f1c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f1c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f1c7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f1c7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f1c7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8f1c7-118">Optional query parameters</span></span>
<span data-ttu-id="8f1c7-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8f1c7-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f1c7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f1c7-120">Request headers</span></span>
|<span data-ttu-id="8f1c7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f1c7-121">Header</span></span>|<span data-ttu-id="8f1c7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8f1c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f1c7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f1c7-123">Authorization</span></span>|<span data-ttu-id="8f1c7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f1c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f1c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8f1c7-125">Accept</span></span>|<span data-ttu-id="8f1c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f1c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f1c7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f1c7-127">Request body</span></span>
<span data-ttu-id="8f1c7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f1c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f1c7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f1c7-129">Response</span></span>
<span data-ttu-id="8f1c7-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8f1c7-130">If successful, this method returns a `200 OK` response code and [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f1c7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8f1c7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f1c7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f1c7-132">Request</span></span>
<span data-ttu-id="8f1c7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f1c7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8f1c7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f1c7-134">Response</span></span>
<span data-ttu-id="8f1c7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f1c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 542

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
    "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "activeHoursStart": "12:00:05.5020000",
    "activeHoursEnd": "11:59:00.8990000",
    "scheduledInstallDays": [
      "monday"
    ],
    "utcTimeOffsetInMinutes": 6
  }
}
```





---
title: Получение targetedManagedAppConfiguration
description: Чтение свойств и связей объекта targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c2d348884d053e694d06856810424f64995bf460
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43398152"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="b7cf7-103">Получение targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7cf7-103">Get targetedManagedAppConfiguration</span></span>

<span data-ttu-id="b7cf7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7cf7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7cf7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7cf7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7cf7-106">Чтение свойств и связей объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7cf7-106">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7cf7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b7cf7-107">Prerequisites</span></span>
<span data-ttu-id="b7cf7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7cf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7cf7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7cf7-110">Permission type</span></span>|<span data-ttu-id="b7cf7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7cf7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7cf7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7cf7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7cf7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7cf7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b7cf7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7cf7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7cf7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7cf7-115">Not supported.</span></span>|
|<span data-ttu-id="b7cf7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7cf7-116">Application</span></span>|<span data-ttu-id="b7cf7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7cf7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7cf7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7cf7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7cf7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7cf7-119">Optional query parameters</span></span>
<span data-ttu-id="b7cf7-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b7cf7-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7cf7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7cf7-121">Request headers</span></span>
|<span data-ttu-id="b7cf7-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7cf7-122">Header</span></span>|<span data-ttu-id="b7cf7-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b7cf7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7cf7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7cf7-124">Authorization</span></span>|<span data-ttu-id="b7cf7-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7cf7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7cf7-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b7cf7-126">Accept</span></span>|<span data-ttu-id="b7cf7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b7cf7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7cf7-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7cf7-128">Request body</span></span>
<span data-ttu-id="b7cf7-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7cf7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7cf7-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7cf7-130">Response</span></span>
<span data-ttu-id="b7cf7-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b7cf7-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7cf7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b7cf7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7cf7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7cf7-133">Request</span></span>
<span data-ttu-id="b7cf7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7cf7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b7cf7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7cf7-135">Response</span></span>
<span data-ttu-id="b7cf7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7cf7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "2444e029-e029-2444-29e0-442429e04424",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "deployedAppCount": 0,
    "isAssigned": true
  }
}
```







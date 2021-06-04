---
title: Получение targetedManagedAppConfiguration
description: Чтение свойств и связей объекта targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83b1fd32604a7342cbc9a17de115cc595bf8d46e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52745431"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="ced90-103">Получение targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ced90-103">Get targetedManagedAppConfiguration</span></span>

<span data-ttu-id="ced90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ced90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ced90-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ced90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ced90-106">Чтение свойств и связей объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ced90-106">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ced90-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ced90-107">Prerequisites</span></span>
<span data-ttu-id="ced90-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ced90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ced90-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ced90-110">Permission type</span></span>|<span data-ttu-id="ced90-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ced90-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ced90-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ced90-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ced90-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ced90-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ced90-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ced90-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ced90-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ced90-115">Not supported.</span></span>|
|<span data-ttu-id="ced90-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ced90-116">Application</span></span>|<span data-ttu-id="ced90-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ced90-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ced90-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ced90-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ced90-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ced90-119">Optional query parameters</span></span>
<span data-ttu-id="ced90-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ced90-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ced90-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ced90-121">Request headers</span></span>
|<span data-ttu-id="ced90-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ced90-122">Header</span></span>|<span data-ttu-id="ced90-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ced90-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ced90-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ced90-124">Authorization</span></span>|<span data-ttu-id="ced90-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ced90-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ced90-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ced90-126">Accept</span></span>|<span data-ttu-id="ced90-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ced90-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ced90-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ced90-128">Request body</span></span>
<span data-ttu-id="ced90-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ced90-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ced90-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ced90-130">Response</span></span>
<span data-ttu-id="ced90-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ced90-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ced90-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ced90-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ced90-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ced90-133">Request</span></span>
<span data-ttu-id="ced90-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ced90-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ced90-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ced90-135">Response</span></span>
<span data-ttu-id="ced90-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ced90-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





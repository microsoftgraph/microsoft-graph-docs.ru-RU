---
title: Перечисление объектов deviceEnrollmentConfiguration
description: Список свойств и связей объектов deviceEnrollmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5fbe05ecb7203875d245f907caf4da3bddbf6393
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52745095"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="9230c-103">Перечисление объектов deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="9230c-103">List deviceEnrollmentConfigurations</span></span>

<span data-ttu-id="9230c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9230c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9230c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9230c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9230c-106">Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9230c-106">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9230c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9230c-107">Prerequisites</span></span>
<span data-ttu-id="9230c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9230c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9230c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9230c-110">Permission type</span></span>|<span data-ttu-id="9230c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9230c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9230c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9230c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9230c-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9230c-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9230c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9230c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9230c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9230c-115">Not supported.</span></span>|
|<span data-ttu-id="9230c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9230c-116">Application</span></span>|<span data-ttu-id="9230c-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9230c-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9230c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9230c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9230c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9230c-119">Request headers</span></span>
|<span data-ttu-id="9230c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9230c-120">Header</span></span>|<span data-ttu-id="9230c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9230c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9230c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9230c-122">Authorization</span></span>|<span data-ttu-id="9230c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9230c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9230c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9230c-124">Accept</span></span>|<span data-ttu-id="9230c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9230c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9230c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9230c-126">Request body</span></span>
<span data-ttu-id="9230c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9230c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9230c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9230c-128">Response</span></span>
<span data-ttu-id="9230c-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9230c-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9230c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9230c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9230c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9230c-131">Request</span></span>
<span data-ttu-id="9230c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9230c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="9230c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9230c-133">Response</span></span>
<span data-ttu-id="9230c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9230c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```





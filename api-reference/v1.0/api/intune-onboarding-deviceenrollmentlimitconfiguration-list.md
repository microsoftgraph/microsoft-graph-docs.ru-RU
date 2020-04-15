---
title: Перечисление объектов deviceEnrollmentLimitConfiguration
description: Список свойств и связей объектов deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2fbbfb18654dbcb6777af21750831a79ef418f3a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452919"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="4e026-103">Перечисление объектов deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="4e026-103">List deviceEnrollmentLimitConfigurations</span></span>

<span data-ttu-id="4e026-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e026-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e026-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e026-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e026-106">Список свойств и связей объектов [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e026-106">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e026-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e026-107">Prerequisites</span></span>
<span data-ttu-id="4e026-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e026-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e026-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e026-110">Permission type</span></span>|<span data-ttu-id="4e026-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e026-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e026-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e026-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e026-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e026-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4e026-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e026-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e026-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e026-115">Not supported.</span></span>|
|<span data-ttu-id="4e026-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e026-116">Application</span></span>|<span data-ttu-id="4e026-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e026-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e026-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e026-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4e026-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e026-119">Request headers</span></span>
|<span data-ttu-id="4e026-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e026-120">Header</span></span>|<span data-ttu-id="4e026-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4e026-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e026-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e026-122">Authorization</span></span>|<span data-ttu-id="4e026-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e026-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e026-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4e026-124">Accept</span></span>|<span data-ttu-id="4e026-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e026-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e026-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e026-126">Request body</span></span>
<span data-ttu-id="4e026-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e026-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e026-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e026-128">Response</span></span>
<span data-ttu-id="4e026-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4e026-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e026-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4e026-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e026-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e026-131">Request</span></span>
<span data-ttu-id="4e026-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e026-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="4e026-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e026-133">Response</span></span>
<span data-ttu-id="4e026-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e026-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
      "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "limit": 5
    }
  ]
}
```







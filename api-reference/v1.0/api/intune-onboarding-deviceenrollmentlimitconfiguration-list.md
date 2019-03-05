---
title: Перечисление объектов deviceEnrollmentLimitConfiguration
description: Список свойств и связей объектов deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1816ec8358f29f8a638199346f0216ed883b7fb
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258970"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="2f1e0-103">Перечисление объектов deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f1e0-103">List deviceEnrollmentLimitConfigurations</span></span>

> <span data-ttu-id="2f1e0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f1e0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f1e0-105">Список свойств и связей объектов [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f1e0-105">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f1e0-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f1e0-106">Prerequisites</span></span>
<span data-ttu-id="2f1e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f1e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f1e0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f1e0-109">Permission type</span></span>|<span data-ttu-id="2f1e0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f1e0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f1e0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f1e0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f1e0-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f1e0-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2f1e0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f1e0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f1e0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f1e0-114">Not supported.</span></span>|
|<span data-ttu-id="2f1e0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f1e0-115">Application</span></span>|<span data-ttu-id="2f1e0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f1e0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f1e0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f1e0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f1e0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f1e0-118">Request headers</span></span>
|<span data-ttu-id="2f1e0-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f1e0-119">Header</span></span>|<span data-ttu-id="2f1e0-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2f1e0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f1e0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f1e0-121">Authorization</span></span>|<span data-ttu-id="2f1e0-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2f1e0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f1e0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2f1e0-123">Accept</span></span>|<span data-ttu-id="2f1e0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f1e0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f1e0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f1e0-125">Request body</span></span>
<span data-ttu-id="2f1e0-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f1e0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f1e0-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f1e0-127">Response</span></span>
<span data-ttu-id="2f1e0-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f1e0-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f1e0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2f1e0-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f1e0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f1e0-130">Request</span></span>
<span data-ttu-id="2f1e0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f1e0-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="2f1e0-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f1e0-132">Response</span></span>
<span data-ttu-id="2f1e0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f1e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




---
title: Перечисление объектов deviceEnrollmentLimitConfiguration
description: Список свойств и связей объектов deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7739dba8fc1a793513823cf030d08ddd5f9b56ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972035"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="27db0-103">Перечисление объектов deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="27db0-103">List deviceEnrollmentLimitConfigurations</span></span>

> <span data-ttu-id="27db0-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="27db0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27db0-105">Список свойств и связей объектов [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27db0-105">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27db0-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="27db0-106">Prerequisites</span></span>
<span data-ttu-id="27db0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27db0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27db0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27db0-109">Permission type</span></span>|<span data-ttu-id="27db0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27db0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27db0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27db0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="27db0-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="27db0-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="27db0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27db0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27db0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27db0-114">Not supported.</span></span>|
|<span data-ttu-id="27db0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27db0-115">Application</span></span>|<span data-ttu-id="27db0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27db0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27db0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27db0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="27db0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27db0-118">Request headers</span></span>
|<span data-ttu-id="27db0-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27db0-119">Header</span></span>|<span data-ttu-id="27db0-120">Значение</span><span class="sxs-lookup"><span data-stu-id="27db0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27db0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="27db0-121">Authorization</span></span>|<span data-ttu-id="27db0-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="27db0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27db0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="27db0-123">Accept</span></span>|<span data-ttu-id="27db0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="27db0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27db0-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="27db0-125">Request body</span></span>
<span data-ttu-id="27db0-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27db0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27db0-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="27db0-127">Response</span></span>
<span data-ttu-id="27db0-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="27db0-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27db0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="27db0-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="27db0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="27db0-130">Request</span></span>
<span data-ttu-id="27db0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27db0-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="27db0-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="27db0-132">Response</span></span>
<span data-ttu-id="27db0-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="27db0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




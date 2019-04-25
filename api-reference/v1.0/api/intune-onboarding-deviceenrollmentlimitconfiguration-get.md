---
title: Получение deviceEnrollmentLimitConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6806cdc0fc02a1edcec712a4a39e0dc4b50578b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582838"
---
# <a name="get-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="d6703-103">Получение deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6703-103">Get deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="d6703-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6703-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6703-105">Чтение свойств и связей объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6703-105">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6703-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d6703-106">Prerequisites</span></span>
<span data-ttu-id="d6703-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6703-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6703-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6703-109">Permission type</span></span>|<span data-ttu-id="d6703-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6703-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6703-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6703-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6703-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6703-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d6703-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6703-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6703-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6703-114">Not supported.</span></span>|
|<span data-ttu-id="d6703-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6703-115">Application</span></span>|<span data-ttu-id="d6703-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6703-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6703-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6703-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6703-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d6703-118">Optional query parameters</span></span>
<span data-ttu-id="d6703-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d6703-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6703-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6703-120">Request headers</span></span>
|<span data-ttu-id="d6703-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6703-121">Header</span></span>|<span data-ttu-id="d6703-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d6703-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6703-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6703-123">Authorization</span></span>|<span data-ttu-id="d6703-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6703-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6703-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6703-125">Accept</span></span>|<span data-ttu-id="d6703-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6703-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6703-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6703-127">Request body</span></span>
<span data-ttu-id="d6703-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6703-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6703-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6703-129">Response</span></span>
<span data-ttu-id="d6703-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d6703-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6703-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d6703-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6703-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6703-132">Request</span></span>
<span data-ttu-id="d6703-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6703-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d6703-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6703-134">Response</span></span>
<span data-ttu-id="d6703-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6703-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 414

{
  "value": {
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
}
```




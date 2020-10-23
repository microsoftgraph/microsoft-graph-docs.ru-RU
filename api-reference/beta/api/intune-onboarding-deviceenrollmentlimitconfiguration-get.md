---
title: Получение deviceEnrollmentLimitConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1741cae31b1aed982bf2b80abde7b73ba98b94e4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709266"
---
# <a name="get-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="ee078-103">Получение deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee078-103">Get deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="ee078-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee078-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee078-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee078-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee078-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee078-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee078-107">Чтение свойств и связей объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee078-107">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee078-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ee078-108">Prerequisites</span></span>
<span data-ttu-id="ee078-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee078-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee078-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee078-111">Permission type</span></span>|<span data-ttu-id="ee078-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee078-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee078-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee078-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee078-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee078-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ee078-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee078-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee078-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee078-116">Not supported.</span></span>|
|<span data-ttu-id="ee078-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee078-117">Application</span></span>|<span data-ttu-id="ee078-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee078-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee078-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee078-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee078-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee078-120">Optional query parameters</span></span>
<span data-ttu-id="ee078-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ee078-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee078-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee078-122">Request headers</span></span>
|<span data-ttu-id="ee078-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee078-123">Header</span></span>|<span data-ttu-id="ee078-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ee078-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee078-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee078-125">Authorization</span></span>|<span data-ttu-id="ee078-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee078-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee078-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ee078-127">Accept</span></span>|<span data-ttu-id="ee078-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ee078-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee078-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee078-129">Request body</span></span>
<span data-ttu-id="ee078-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee078-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee078-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee078-131">Response</span></span>
<span data-ttu-id="ee078-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ee078-132">If successful, this method returns a `200 OK` response code and [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee078-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ee078-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee078-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee078-134">Request</span></span>
<span data-ttu-id="ee078-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee078-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ee078-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee078-136">Response</span></span>
<span data-ttu-id="ee078-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee078-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 482

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
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "limit": 5
  }
}
```






---
title: Получение объекта deviceEnrollmentConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0e90822aed702f7fa515846891f26d29f57fe46
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801112"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="2b3d6-103">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b3d6-103">Get deviceEnrollmentConfiguration</span></span>

> <span data-ttu-id="2b3d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b3d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b3d6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b3d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b3d6-106">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b3d6-106">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b3d6-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2b3d6-107">Prerequisites</span></span>
<span data-ttu-id="2b3d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b3d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b3d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b3d6-110">Permission type</span></span>|<span data-ttu-id="2b3d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b3d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b3d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b3d6-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2b3d6-113">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="2b3d6-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2b3d6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b3d6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="2b3d6-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2b3d6-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2b3d6-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b3d6-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2b3d6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b3d6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b3d6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b3d6-118">Not supported.</span></span>|
|<span data-ttu-id="2b3d6-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="2b3d6-119">Application</span></span>||
| <span data-ttu-id="2b3d6-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="2b3d6-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2b3d6-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b3d6-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="2b3d6-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2b3d6-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2b3d6-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b3d6-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b3d6-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b3d6-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b3d6-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b3d6-125">Optional query parameters</span></span>
<span data-ttu-id="2b3d6-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2b3d6-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b3d6-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b3d6-127">Request headers</span></span>
|<span data-ttu-id="2b3d6-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b3d6-128">Header</span></span>|<span data-ttu-id="2b3d6-129">Значение</span><span class="sxs-lookup"><span data-stu-id="2b3d6-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b3d6-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b3d6-130">Authorization</span></span>|<span data-ttu-id="2b3d6-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b3d6-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b3d6-132">Accept</span><span class="sxs-lookup"><span data-stu-id="2b3d6-132">Accept</span></span>|<span data-ttu-id="2b3d6-133">application/json</span><span class="sxs-lookup"><span data-stu-id="2b3d6-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b3d6-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b3d6-134">Request body</span></span>
<span data-ttu-id="2b3d6-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b3d6-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b3d6-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b3d6-136">Response</span></span>
<span data-ttu-id="2b3d6-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b3d6-137">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b3d6-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2b3d6-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b3d6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b3d6-139">Request</span></span>
<span data-ttu-id="2b3d6-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b3d6-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2b3d6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b3d6-141">Response</span></span>
<span data-ttu-id="2b3d6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b3d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
    "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7
  }
}
```








---
title: Получение объекта deviceEnrollmentConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0af22a9c351242dba83f397cbcaa36aafe68c0e4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201060"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="6f06a-103">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f06a-103">Get deviceEnrollmentConfiguration</span></span>

> <span data-ttu-id="6f06a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f06a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f06a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f06a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f06a-106">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f06a-106">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f06a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6f06a-107">Prerequisites</span></span>
<span data-ttu-id="6f06a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f06a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f06a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f06a-110">Permission type</span></span>|<span data-ttu-id="6f06a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f06a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f06a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f06a-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6f06a-113">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="6f06a-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="6f06a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f06a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="6f06a-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="6f06a-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6f06a-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f06a-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6f06a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f06a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f06a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f06a-118">Not supported.</span></span>|
|<span data-ttu-id="6f06a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f06a-119">Application</span></span>||
| <span data-ttu-id="6f06a-120">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="6f06a-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="6f06a-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f06a-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="6f06a-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="6f06a-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6f06a-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f06a-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f06a-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f06a-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f06a-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6f06a-125">Optional query parameters</span></span>
<span data-ttu-id="6f06a-126">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6f06a-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f06a-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f06a-127">Request headers</span></span>
|<span data-ttu-id="6f06a-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f06a-128">Header</span></span>|<span data-ttu-id="6f06a-129">Значение</span><span class="sxs-lookup"><span data-stu-id="6f06a-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f06a-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f06a-130">Authorization</span></span>|<span data-ttu-id="6f06a-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f06a-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f06a-132">Accept</span><span class="sxs-lookup"><span data-stu-id="6f06a-132">Accept</span></span>|<span data-ttu-id="6f06a-133">application/json</span><span class="sxs-lookup"><span data-stu-id="6f06a-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f06a-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f06a-134">Request body</span></span>
<span data-ttu-id="6f06a-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f06a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f06a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f06a-136">Response</span></span>
<span data-ttu-id="6f06a-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6f06a-137">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f06a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6f06a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f06a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f06a-139">Request</span></span>
<span data-ttu-id="6f06a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f06a-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6f06a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f06a-141">Response</span></span>
<span data-ttu-id="6f06a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f06a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





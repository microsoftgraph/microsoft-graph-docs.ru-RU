---
title: Получение объекта deviceEnrollmentConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 687f2e50be80d3d8d7ed2bf30b173c630285a70c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074449"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="9436b-103">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="9436b-103">Get deviceEnrollmentConfiguration</span></span>

<span data-ttu-id="9436b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9436b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9436b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9436b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9436b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9436b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9436b-107">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9436b-107">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9436b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9436b-108">Prerequisites</span></span>
<span data-ttu-id="9436b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9436b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9436b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9436b-111">Permission type</span></span>|<span data-ttu-id="9436b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9436b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9436b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9436b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9436b-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="9436b-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9436b-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9436b-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="9436b-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="9436b-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="9436b-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9436b-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9436b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9436b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9436b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9436b-119">Not supported.</span></span>|
|<span data-ttu-id="9436b-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9436b-120">Application</span></span>||
| <span data-ttu-id="9436b-121">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="9436b-121">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9436b-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9436b-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="9436b-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="9436b-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="9436b-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9436b-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9436b-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9436b-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9436b-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9436b-126">Optional query parameters</span></span>
<span data-ttu-id="9436b-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9436b-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9436b-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9436b-128">Request headers</span></span>
|<span data-ttu-id="9436b-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9436b-129">Header</span></span>|<span data-ttu-id="9436b-130">Значение</span><span class="sxs-lookup"><span data-stu-id="9436b-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9436b-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9436b-131">Authorization</span></span>|<span data-ttu-id="9436b-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9436b-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9436b-133">Accept</span><span class="sxs-lookup"><span data-stu-id="9436b-133">Accept</span></span>|<span data-ttu-id="9436b-134">application/json</span><span class="sxs-lookup"><span data-stu-id="9436b-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9436b-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9436b-135">Request body</span></span>
<span data-ttu-id="9436b-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9436b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9436b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9436b-137">Response</span></span>
<span data-ttu-id="9436b-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9436b-138">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9436b-139">Пример</span><span class="sxs-lookup"><span data-stu-id="9436b-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="9436b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9436b-140">Request</span></span>
<span data-ttu-id="9436b-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9436b-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9436b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9436b-142">Response</span></span>
<span data-ttu-id="9436b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9436b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










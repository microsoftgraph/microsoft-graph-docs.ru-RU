---
title: Получение объекта deviceEnrollmentConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4db4985a2250160db7124cc22b4e27d431b60e4c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900525"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="cb11d-103">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb11d-103">Get deviceEnrollmentConfiguration</span></span>

> <span data-ttu-id="cb11d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb11d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb11d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb11d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb11d-106">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb11d-106">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb11d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cb11d-107">Prerequisites</span></span>
<span data-ttu-id="cb11d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb11d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb11d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb11d-110">Permission type</span></span>|<span data-ttu-id="cb11d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb11d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb11d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb11d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb11d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb11d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cb11d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb11d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb11d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb11d-115">Not supported.</span></span>|
|<span data-ttu-id="cb11d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb11d-116">Application</span></span>|<span data-ttu-id="cb11d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb11d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb11d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb11d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb11d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cb11d-119">Optional query parameters</span></span>
<span data-ttu-id="cb11d-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cb11d-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb11d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb11d-121">Request headers</span></span>
|<span data-ttu-id="cb11d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb11d-122">Header</span></span>|<span data-ttu-id="cb11d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cb11d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb11d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb11d-124">Authorization</span></span>|<span data-ttu-id="cb11d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb11d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb11d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="cb11d-126">Accept</span></span>|<span data-ttu-id="cb11d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cb11d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb11d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb11d-128">Request body</span></span>
<span data-ttu-id="cb11d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb11d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb11d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb11d-130">Response</span></span>
<span data-ttu-id="cb11d-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cb11d-131">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb11d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cb11d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb11d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb11d-133">Request</span></span>
<span data-ttu-id="cb11d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb11d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="cb11d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb11d-135">Response</span></span>
<span data-ttu-id="cb11d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb11d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





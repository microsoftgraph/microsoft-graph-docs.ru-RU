---
title: Получение объекта deviceEnrollmentConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8d221f37e0fca0cee52bdd6f9d1cdc3a17034324
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974775"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="4a1dd-103">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a1dd-103">Get deviceEnrollmentConfiguration</span></span>

> <span data-ttu-id="4a1dd-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a1dd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a1dd-105">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a1dd-105">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a1dd-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4a1dd-106">Prerequisites</span></span>
<span data-ttu-id="4a1dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a1dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a1dd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a1dd-109">Permission type</span></span>|<span data-ttu-id="4a1dd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a1dd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a1dd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a1dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4a1dd-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a1dd-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4a1dd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a1dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a1dd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a1dd-114">Not supported.</span></span>|
|<span data-ttu-id="4a1dd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a1dd-115">Application</span></span>|<span data-ttu-id="4a1dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a1dd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a1dd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a1dd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a1dd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4a1dd-118">Optional query parameters</span></span>
<span data-ttu-id="4a1dd-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4a1dd-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a1dd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a1dd-120">Request headers</span></span>
|<span data-ttu-id="4a1dd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a1dd-121">Header</span></span>|<span data-ttu-id="4a1dd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4a1dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a1dd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a1dd-123">Authorization</span></span>|<span data-ttu-id="4a1dd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a1dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a1dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4a1dd-125">Accept</span></span>|<span data-ttu-id="4a1dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a1dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a1dd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a1dd-127">Request body</span></span>
<span data-ttu-id="4a1dd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a1dd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a1dd-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a1dd-129">Response</span></span>
<span data-ttu-id="4a1dd-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4a1dd-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a1dd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4a1dd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a1dd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a1dd-132">Request</span></span>
<span data-ttu-id="4a1dd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a1dd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4a1dd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a1dd-134">Response</span></span>
<span data-ttu-id="4a1dd-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a1dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




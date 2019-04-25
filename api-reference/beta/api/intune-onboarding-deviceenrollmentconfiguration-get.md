---
title: Получение объекта deviceEnrollmentConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b137cf4225dae8c85960210bc1f49360eb20d4c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32529067"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="688f4-103">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="688f4-103">Get deviceEnrollmentConfiguration</span></span>

> <span data-ttu-id="688f4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="688f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="688f4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="688f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="688f4-106">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="688f4-106">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="688f4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="688f4-107">Prerequisites</span></span>
<span data-ttu-id="688f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="688f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="688f4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="688f4-110">Permission type</span></span>|<span data-ttu-id="688f4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="688f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="688f4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="688f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="688f4-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="688f4-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="688f4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="688f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="688f4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="688f4-115">Not supported.</span></span>|
|<span data-ttu-id="688f4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="688f4-116">Application</span></span>|<span data-ttu-id="688f4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="688f4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="688f4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="688f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="688f4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="688f4-119">Optional query parameters</span></span>
<span data-ttu-id="688f4-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="688f4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="688f4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="688f4-121">Request headers</span></span>
|<span data-ttu-id="688f4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="688f4-122">Header</span></span>|<span data-ttu-id="688f4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="688f4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="688f4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="688f4-124">Authorization</span></span>|<span data-ttu-id="688f4-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="688f4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="688f4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="688f4-126">Accept</span></span>|<span data-ttu-id="688f4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="688f4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="688f4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="688f4-128">Request body</span></span>
<span data-ttu-id="688f4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="688f4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="688f4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="688f4-130">Response</span></span>
<span data-ttu-id="688f4-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="688f4-131">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="688f4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="688f4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="688f4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="688f4-133">Request</span></span>
<span data-ttu-id="688f4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="688f4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="688f4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="688f4-135">Response</span></span>
<span data-ttu-id="688f4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="688f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






---
title: Получение объекта deviceEnrollmentConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91bf59d48719970f5b8dad91b99ce45d018aa29f
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086111"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="f544f-103">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="f544f-103">Get deviceEnrollmentConfiguration</span></span>

> <span data-ttu-id="f544f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f544f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f544f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f544f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f544f-106">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f544f-106">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f544f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f544f-107">Prerequisites</span></span>
<span data-ttu-id="f544f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f544f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f544f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f544f-110">Permission type</span></span>|<span data-ttu-id="f544f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f544f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f544f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f544f-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f544f-113">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="f544f-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f544f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f544f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="f544f-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="f544f-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f544f-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f544f-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f544f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f544f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f544f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f544f-118">Not supported.</span></span>|
|<span data-ttu-id="f544f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f544f-119">Application</span></span>||
| <span data-ttu-id="f544f-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="f544f-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f544f-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f544f-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="f544f-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="f544f-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f544f-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f544f-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f544f-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f544f-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f544f-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f544f-125">Optional query parameters</span></span>
<span data-ttu-id="f544f-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f544f-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f544f-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f544f-127">Request headers</span></span>
|<span data-ttu-id="f544f-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f544f-128">Header</span></span>|<span data-ttu-id="f544f-129">Значение</span><span class="sxs-lookup"><span data-stu-id="f544f-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f544f-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f544f-130">Authorization</span></span>|<span data-ttu-id="f544f-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f544f-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f544f-132">Accept</span><span class="sxs-lookup"><span data-stu-id="f544f-132">Accept</span></span>|<span data-ttu-id="f544f-133">application/json</span><span class="sxs-lookup"><span data-stu-id="f544f-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f544f-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f544f-134">Request body</span></span>
<span data-ttu-id="f544f-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f544f-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f544f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f544f-136">Response</span></span>
<span data-ttu-id="f544f-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f544f-137">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f544f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f544f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f544f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f544f-139">Request</span></span>
<span data-ttu-id="f544f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f544f-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f544f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f544f-141">Response</span></span>
<span data-ttu-id="f544f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f544f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










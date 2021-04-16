---
title: Получение объекта deviceEnrollmentConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6925e91ff6d1974ea0073de92724020196b98597
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864209"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="2b61e-103">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b61e-103">Get deviceEnrollmentConfiguration</span></span>

<span data-ttu-id="2b61e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b61e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b61e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b61e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b61e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b61e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b61e-107">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b61e-107">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b61e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2b61e-108">Prerequisites</span></span>
<span data-ttu-id="2b61e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b61e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b61e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b61e-111">Permission type</span></span>|<span data-ttu-id="2b61e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b61e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b61e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b61e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2b61e-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="2b61e-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2b61e-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b61e-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="2b61e-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2b61e-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2b61e-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b61e-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2b61e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b61e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b61e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b61e-119">Not supported.</span></span>|
|<span data-ttu-id="2b61e-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2b61e-120">Application</span></span>||
| <span data-ttu-id="2b61e-121">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="2b61e-121">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2b61e-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b61e-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="2b61e-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2b61e-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2b61e-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b61e-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b61e-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b61e-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b61e-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b61e-126">Optional query parameters</span></span>
<span data-ttu-id="2b61e-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2b61e-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b61e-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b61e-128">Request headers</span></span>
|<span data-ttu-id="2b61e-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b61e-129">Header</span></span>|<span data-ttu-id="2b61e-130">Значение</span><span class="sxs-lookup"><span data-stu-id="2b61e-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b61e-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b61e-131">Authorization</span></span>|<span data-ttu-id="2b61e-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b61e-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b61e-133">Accept</span><span class="sxs-lookup"><span data-stu-id="2b61e-133">Accept</span></span>|<span data-ttu-id="2b61e-134">application/json</span><span class="sxs-lookup"><span data-stu-id="2b61e-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b61e-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b61e-135">Request body</span></span>
<span data-ttu-id="2b61e-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b61e-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b61e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b61e-137">Response</span></span>
<span data-ttu-id="2b61e-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b61e-138">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b61e-139">Пример</span><span class="sxs-lookup"><span data-stu-id="2b61e-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b61e-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b61e-140">Request</span></span>
<span data-ttu-id="2b61e-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b61e-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2b61e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b61e-142">Response</span></span>
<span data-ttu-id="2b61e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b61e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








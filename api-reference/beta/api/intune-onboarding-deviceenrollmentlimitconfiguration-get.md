---
title: Получение deviceEnrollmentLimitConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 77891153bf4e85089a48f6ccbd94932baaf4850e
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177753"
---
# <a name="get-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="392aa-103">Получение deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="392aa-103">Get deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="392aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="392aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="392aa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="392aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="392aa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="392aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="392aa-107">Чтение свойств и связей объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="392aa-107">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="392aa-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="392aa-108">Prerequisites</span></span>
<span data-ttu-id="392aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="392aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="392aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="392aa-111">Permission type</span></span>|<span data-ttu-id="392aa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="392aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="392aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="392aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="392aa-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="392aa-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="392aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="392aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="392aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="392aa-116">Not supported.</span></span>|
|<span data-ttu-id="392aa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="392aa-117">Application</span></span>|<span data-ttu-id="392aa-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="392aa-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="392aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="392aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="392aa-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="392aa-120">Optional query parameters</span></span>
<span data-ttu-id="392aa-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="392aa-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="392aa-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="392aa-122">Request headers</span></span>
|<span data-ttu-id="392aa-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="392aa-123">Header</span></span>|<span data-ttu-id="392aa-124">Значение</span><span class="sxs-lookup"><span data-stu-id="392aa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="392aa-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="392aa-125">Authorization</span></span>|<span data-ttu-id="392aa-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="392aa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="392aa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="392aa-127">Accept</span></span>|<span data-ttu-id="392aa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="392aa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="392aa-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="392aa-129">Request body</span></span>
<span data-ttu-id="392aa-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="392aa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="392aa-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="392aa-131">Response</span></span>
<span data-ttu-id="392aa-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="392aa-132">If successful, this method returns a `200 OK` response code and [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="392aa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="392aa-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="392aa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="392aa-134">Request</span></span>
<span data-ttu-id="392aa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="392aa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="392aa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="392aa-136">Response</span></span>
<span data-ttu-id="392aa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="392aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




---
title: Получение windowsDomainJoinConfiguration
description: Чтение свойства и связи объекта windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 64a295ae105a69865e304c45d08e339eadbf7936
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950244"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="be224-103">Получение windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="be224-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="be224-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="be224-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be224-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be224-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be224-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="be224-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be224-107">Чтение свойства и связи объекта [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="be224-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be224-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be224-108">Prerequisites</span></span>

<span data-ttu-id="be224-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be224-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be224-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be224-111">Permission type</span></span>|<span data-ttu-id="be224-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be224-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be224-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be224-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="be224-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="be224-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="be224-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="be224-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="be224-116">&nbsp; &nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="be224-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="be224-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="be224-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="be224-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be224-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be224-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be224-119">Not supported.</span></span>|
|<span data-ttu-id="be224-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be224-120">Application</span></span>|<span data-ttu-id="be224-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be224-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be224-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be224-122">HTTP Request</span></span>
<span data-ttu-id="be224-123">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="be224-123">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="be224-124">**Регистрация**</span><span class="sxs-lookup"><span data-stu-id="be224-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be224-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="be224-125">Optional query parameters</span></span>

<span data-ttu-id="be224-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="be224-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be224-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be224-127">Request headers</span></span>

|<span data-ttu-id="be224-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be224-128">Header</span></span>|<span data-ttu-id="be224-129">Значение</span><span class="sxs-lookup"><span data-stu-id="be224-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be224-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="be224-130">Authorization</span></span>|<span data-ttu-id="be224-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="be224-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be224-132">Accept</span><span class="sxs-lookup"><span data-stu-id="be224-132">Accept</span></span>|<span data-ttu-id="be224-133">application/json</span><span class="sxs-lookup"><span data-stu-id="be224-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be224-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be224-134">Request body</span></span>

<span data-ttu-id="be224-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be224-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be224-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="be224-136">Response</span></span>

<span data-ttu-id="be224-137">Успешно завершена, этот метод возвращает `200 OK` объект [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="be224-137">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be224-138">Пример</span><span class="sxs-lookup"><span data-stu-id="be224-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="be224-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="be224-139">Request</span></span>

<span data-ttu-id="be224-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be224-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="be224-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="be224-141">Response</span></span>

<span data-ttu-id="be224-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="be224-142">Here is an example of the response.</span></span> <span data-ttu-id="be224-143">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="be224-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="be224-144">Свойства, возвращенные фактический вызов зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="be224-144">Properties returned from an actual call depend on the context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
    "id": "40118d08-8d08-4011-088d-1140088d1140",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "computerNameStaticPrefix": "Computer Name Static Prefix value",
    "computerNameSuffixRandomCharCount": 1,
    "activeDirectoryDomainName": "Active Directory Domain Name value"
  }
}
```




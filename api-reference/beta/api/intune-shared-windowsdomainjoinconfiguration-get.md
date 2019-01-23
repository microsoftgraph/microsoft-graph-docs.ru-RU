---
title: Получение windowsDomainJoinConfiguration
description: Чтение свойства и связи объекта windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 64e8db69cc7a3bf158d5ae4d359fde15f1ab7751
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400083"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="f614a-103">Получение windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="f614a-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="f614a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f614a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f614a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f614a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f614a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f614a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f614a-107">Чтение свойства и связи объекта [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f614a-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f614a-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f614a-108">Prerequisites</span></span>

<span data-ttu-id="f614a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f614a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f614a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f614a-111">Permission type</span></span>|<span data-ttu-id="f614a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f614a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f614a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f614a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f614a-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="f614a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f614a-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f614a-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="f614a-116">&nbsp; &nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="f614a-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="f614a-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f614a-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="f614a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f614a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f614a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f614a-119">Not supported.</span></span>|
|<span data-ttu-id="f614a-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f614a-120">Application</span></span>|<span data-ttu-id="f614a-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f614a-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f614a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f614a-122">HTTP Request</span></span>
<span data-ttu-id="f614a-123">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="f614a-123">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="f614a-124">**Регистрация**</span><span class="sxs-lookup"><span data-stu-id="f614a-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f614a-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f614a-125">Optional query parameters</span></span>

<span data-ttu-id="f614a-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f614a-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f614a-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f614a-127">Request headers</span></span>

|<span data-ttu-id="f614a-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f614a-128">Header</span></span>|<span data-ttu-id="f614a-129">Значение</span><span class="sxs-lookup"><span data-stu-id="f614a-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f614a-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="f614a-130">Authorization</span></span>|<span data-ttu-id="f614a-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f614a-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f614a-132">Accept</span><span class="sxs-lookup"><span data-stu-id="f614a-132">Accept</span></span>|<span data-ttu-id="f614a-133">application/json</span><span class="sxs-lookup"><span data-stu-id="f614a-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f614a-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f614a-134">Request body</span></span>

<span data-ttu-id="f614a-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f614a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f614a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f614a-136">Response</span></span>

<span data-ttu-id="f614a-137">Успешно завершена, этот метод возвращает `200 OK` объект [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f614a-137">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f614a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f614a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f614a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f614a-139">Request</span></span>

<span data-ttu-id="f614a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f614a-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f614a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f614a-141">Response</span></span>

<span data-ttu-id="f614a-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f614a-142">Here is an example of the response.</span></span> <span data-ttu-id="f614a-143">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f614a-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f614a-144">Свойства, возвращенные фактический вызов зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="f614a-144">Properties returned from an actual call depend on the context.</span></span>

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




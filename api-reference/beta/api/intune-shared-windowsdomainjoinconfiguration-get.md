---
title: Получение Виндовсдомаинжоинконфигуратион
description: Чтение свойств и связей объекта Виндовсдомаинжоинконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 41d91282e630877ecee3c22adb5acaa1ced4768f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800468"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="f058d-103">Получение Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f058d-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="f058d-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f058d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f058d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f058d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f058d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f058d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f058d-107">Чтение свойств и связей объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f058d-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f058d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f058d-108">Prerequisites</span></span>

<span data-ttu-id="f058d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f058d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f058d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f058d-111">Permission type</span></span>|<span data-ttu-id="f058d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f058d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f058d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f058d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f058d-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="f058d-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f058d-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f058d-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="f058d-116">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="f058d-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="f058d-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f058d-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="f058d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f058d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f058d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f058d-119">Not supported.</span></span>|
|<span data-ttu-id="f058d-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="f058d-120">Application</span></span>||
| <span data-ttu-id="f058d-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="f058d-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f058d-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f058d-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="f058d-123">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="f058d-123">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="f058d-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f058d-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f058d-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f058d-125">HTTP Request</span></span>
<span data-ttu-id="f058d-126">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="f058d-126">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="f058d-127">**Регистрации**</span><span class="sxs-lookup"><span data-stu-id="f058d-127">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f058d-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f058d-128">Optional query parameters</span></span>

<span data-ttu-id="f058d-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f058d-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f058d-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f058d-130">Request headers</span></span>

|<span data-ttu-id="f058d-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f058d-131">Header</span></span>|<span data-ttu-id="f058d-132">Значение</span><span class="sxs-lookup"><span data-stu-id="f058d-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f058d-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="f058d-133">Authorization</span></span>|<span data-ttu-id="f058d-134">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f058d-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f058d-135">Accept</span><span class="sxs-lookup"><span data-stu-id="f058d-135">Accept</span></span>|<span data-ttu-id="f058d-136">application/json</span><span class="sxs-lookup"><span data-stu-id="f058d-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f058d-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f058d-137">Request body</span></span>

<span data-ttu-id="f058d-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f058d-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f058d-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="f058d-139">Response</span></span>

<span data-ttu-id="f058d-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f058d-140">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f058d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="f058d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f058d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f058d-142">Request</span></span>

<span data-ttu-id="f058d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f058d-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f058d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f058d-144">Response</span></span>

<span data-ttu-id="f058d-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f058d-145">Here is an example of the response.</span></span> <span data-ttu-id="f058d-146">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f058d-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f058d-147">Свойства, возвращаемые при фактическом вызове, зависят от контекста.</span><span class="sxs-lookup"><span data-stu-id="f058d-147">Properties returned from an actual call depend on the context.</span></span>

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











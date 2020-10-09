---
title: Получение Виндовсдомаинжоинконфигуратион
description: Чтение свойств и связей объекта Виндовсдомаинжоинконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e25511c308bce1a27e5579e8c61adbc7e7c8e8af
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404009"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="d145c-103">Получение Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d145c-103">Get windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="d145c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d145c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d145c-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d145c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d145c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d145c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d145c-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d145c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d145c-108">Чтение свойств и связей объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d145c-108">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d145c-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d145c-109">Prerequisites</span></span>

<span data-ttu-id="d145c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d145c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d145c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d145c-112">Permission type</span></span>|<span data-ttu-id="d145c-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d145c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d145c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d145c-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d145c-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="d145c-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d145c-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d145c-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d145c-117">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="d145c-117">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d145c-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d145c-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="d145c-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d145c-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d145c-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d145c-120">Not supported.</span></span>|
|<span data-ttu-id="d145c-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d145c-121">Application</span></span>||
| <span data-ttu-id="d145c-122">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="d145c-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d145c-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d145c-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d145c-124">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="d145c-124">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d145c-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d145c-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d145c-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d145c-126">HTTP Request</span></span>
<span data-ttu-id="d145c-127">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="d145c-127">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="d145c-128">**Регистрации**</span><span class="sxs-lookup"><span data-stu-id="d145c-128">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d145c-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d145c-129">Optional query parameters</span></span>

<span data-ttu-id="d145c-130">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d145c-130">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d145c-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d145c-131">Request headers</span></span>

|<span data-ttu-id="d145c-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d145c-132">Header</span></span>|<span data-ttu-id="d145c-133">Значение</span><span class="sxs-lookup"><span data-stu-id="d145c-133">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d145c-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d145c-134">Authorization</span></span>|<span data-ttu-id="d145c-135">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d145c-135">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d145c-136">Accept</span><span class="sxs-lookup"><span data-stu-id="d145c-136">Accept</span></span>|<span data-ttu-id="d145c-137">application/json</span><span class="sxs-lookup"><span data-stu-id="d145c-137">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d145c-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d145c-138">Request body</span></span>

<span data-ttu-id="d145c-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d145c-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d145c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d145c-140">Response</span></span>

<span data-ttu-id="d145c-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d145c-141">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d145c-142">Пример</span><span class="sxs-lookup"><span data-stu-id="d145c-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="d145c-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d145c-143">Request</span></span>

<span data-ttu-id="d145c-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d145c-144">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d145c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d145c-145">Response</span></span>

<span data-ttu-id="d145c-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d145c-146">Here is an example of the response.</span></span> <span data-ttu-id="d145c-147">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="d145c-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d145c-148">Свойства, возвращаемые при фактическом вызове, зависят от контекста.</span><span class="sxs-lookup"><span data-stu-id="d145c-148">Properties returned from an actual call depend on the context.</span></span>

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
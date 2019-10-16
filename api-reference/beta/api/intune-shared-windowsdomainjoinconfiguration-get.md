---
title: Получение Виндовсдомаинжоинконфигуратион
description: Чтение свойств и связей объекта Виндовсдомаинжоинконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b4e9ccc3e45f05537f688b14b5c78fe3af6720d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537848"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="04b75-103">Получение Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="04b75-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="04b75-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="04b75-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04b75-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04b75-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04b75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04b75-107">Чтение свойств и связей объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="04b75-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04b75-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="04b75-108">Prerequisites</span></span>

<span data-ttu-id="04b75-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04b75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04b75-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04b75-111">Permission type</span></span>|<span data-ttu-id="04b75-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04b75-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04b75-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04b75-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="04b75-114">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="04b75-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="04b75-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b75-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="04b75-116">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="04b75-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="04b75-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b75-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="04b75-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04b75-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04b75-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b75-119">Not supported.</span></span>|
|<span data-ttu-id="04b75-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="04b75-120">Application</span></span>||
| <span data-ttu-id="04b75-121">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="04b75-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="04b75-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b75-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="04b75-123">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="04b75-123">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="04b75-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b75-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04b75-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04b75-125">HTTP Request</span></span>
<span data-ttu-id="04b75-126">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="04b75-126">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="04b75-127">**Регистрации**</span><span class="sxs-lookup"><span data-stu-id="04b75-127">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04b75-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="04b75-128">Optional query parameters</span></span>

<span data-ttu-id="04b75-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="04b75-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04b75-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04b75-130">Request headers</span></span>

|<span data-ttu-id="04b75-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04b75-131">Header</span></span>|<span data-ttu-id="04b75-132">Значение</span><span class="sxs-lookup"><span data-stu-id="04b75-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04b75-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04b75-133">Authorization</span></span>|<span data-ttu-id="04b75-134">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04b75-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04b75-135">Accept</span><span class="sxs-lookup"><span data-stu-id="04b75-135">Accept</span></span>|<span data-ttu-id="04b75-136">application/json</span><span class="sxs-lookup"><span data-stu-id="04b75-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04b75-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04b75-137">Request body</span></span>

<span data-ttu-id="04b75-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04b75-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04b75-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="04b75-139">Response</span></span>

<span data-ttu-id="04b75-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04b75-140">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04b75-141">Пример</span><span class="sxs-lookup"><span data-stu-id="04b75-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="04b75-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="04b75-142">Request</span></span>

<span data-ttu-id="04b75-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04b75-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="04b75-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b75-144">Response</span></span>

<span data-ttu-id="04b75-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04b75-145">Here is an example of the response.</span></span> <span data-ttu-id="04b75-146">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="04b75-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="04b75-147">Свойства, возвращаемые при фактическом вызове, зависят от контекста.</span><span class="sxs-lookup"><span data-stu-id="04b75-147">Properties returned from an actual call depend on the context.</span></span>

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










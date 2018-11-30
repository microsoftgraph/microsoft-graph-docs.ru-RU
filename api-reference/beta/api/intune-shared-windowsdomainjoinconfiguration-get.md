---
title: Получение windowsDomainJoinConfiguration
description: Чтение свойства и связи объекта windowsDomainJoinConfiguration.
ms.openlocfilehash: b3b76a902b4a740d142e1027f04d1f98f5fb32aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077363"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="0c421-103">Получение windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c421-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="0c421-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c421-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c421-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c421-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c421-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0c421-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c421-107">Чтение свойства и связи объекта [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0c421-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c421-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0c421-108">Prerequisites</span></span>

<span data-ttu-id="0c421-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c421-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c421-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c421-111">Permission type</span></span>|<span data-ttu-id="0c421-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c421-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c421-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c421-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0c421-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="0c421-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0c421-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c421-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="0c421-116">&nbsp; &nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="0c421-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="0c421-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c421-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="0c421-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c421-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c421-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c421-119">Not supported.</span></span>|
|<span data-ttu-id="0c421-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c421-120">Application</span></span>|<span data-ttu-id="0c421-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c421-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c421-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c421-122">HTTP Request</span></span>
<span data-ttu-id="0c421-123">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="0c421-123">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="0c421-124">**Регистрация**</span><span class="sxs-lookup"><span data-stu-id="0c421-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c421-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0c421-125">Optional query parameters</span></span>

<span data-ttu-id="0c421-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0c421-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c421-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c421-127">Request headers</span></span>

|<span data-ttu-id="0c421-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c421-128">Header</span></span>|<span data-ttu-id="0c421-129">Значение</span><span class="sxs-lookup"><span data-stu-id="0c421-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c421-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c421-130">Authorization</span></span>|<span data-ttu-id="0c421-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0c421-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c421-132">Accept</span><span class="sxs-lookup"><span data-stu-id="0c421-132">Accept</span></span>|<span data-ttu-id="0c421-133">application/json</span><span class="sxs-lookup"><span data-stu-id="0c421-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c421-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c421-134">Request body</span></span>

<span data-ttu-id="0c421-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c421-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c421-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c421-136">Response</span></span>

<span data-ttu-id="0c421-137">Успешно завершена, этот метод возвращает `200 OK` объект [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0c421-137">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c421-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0c421-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c421-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c421-139">Request</span></span>

<span data-ttu-id="0c421-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c421-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0c421-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c421-141">Response</span></span>

<span data-ttu-id="0c421-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0c421-142">Here is an example of the response.</span></span> <span data-ttu-id="0c421-143">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="0c421-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0c421-144">Свойства, возвращенные фактический вызов зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="0c421-144">Properties returned from an actual call depend on the context.</span></span>

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




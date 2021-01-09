---
title: Get deviceManagementDerivedCredentialSettings
description: Чтение свойств и связей объекта deviceManagementDerivedCredentialSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7ca75a572c2ce793594e1e2cce5c8521ed2d9948
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790680"
---
# <a name="get-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="31334-103">Get deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="31334-103">Get deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="31334-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31334-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31334-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31334-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31334-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31334-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31334-107">Чтение свойств и связей объекта [deviceManagementDerivedCredentialSettings.](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)</span><span class="sxs-lookup"><span data-stu-id="31334-107">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31334-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="31334-108">Prerequisites</span></span>
<span data-ttu-id="31334-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31334-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31334-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31334-111">Permission type</span></span>|<span data-ttu-id="31334-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="31334-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31334-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31334-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="31334-114">&nbsp;&nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="31334-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="31334-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="31334-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="31334-116">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="31334-116">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="31334-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="31334-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="31334-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31334-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31334-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31334-119">Not supported.</span></span>|
|<span data-ttu-id="31334-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31334-120">Application</span></span>||
|<span data-ttu-id="31334-121">&nbsp;&nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="31334-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="31334-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="31334-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="31334-123">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="31334-123">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="31334-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="31334-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31334-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31334-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31334-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="31334-126">Optional query parameters</span></span>
<span data-ttu-id="31334-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="31334-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31334-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31334-128">Request headers</span></span>

|<span data-ttu-id="31334-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31334-129">Header</span></span>|<span data-ttu-id="31334-130">Значение</span><span class="sxs-lookup"><span data-stu-id="31334-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31334-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31334-131">Authorization</span></span>|<span data-ttu-id="31334-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31334-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31334-133">Accept</span><span class="sxs-lookup"><span data-stu-id="31334-133">Accept</span></span>|<span data-ttu-id="31334-134">application/json</span><span class="sxs-lookup"><span data-stu-id="31334-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31334-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31334-135">Request body</span></span>
<span data-ttu-id="31334-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31334-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31334-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="31334-137">Response</span></span>
<span data-ttu-id="31334-138">В случае успешного выполнения этот метод возвращает код отклика и объект `200 OK` [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="31334-138">If successful, this method returns a `200 OK` response code and [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31334-139">Пример</span><span class="sxs-lookup"><span data-stu-id="31334-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="31334-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="31334-140">Request</span></span>
<span data-ttu-id="31334-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31334-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
```

### <a name="response"></a><span data-ttu-id="31334-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="31334-142">Response</span></span>
<span data-ttu-id="31334-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31334-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 155

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
    "id": "bc650741-0741-bc65-4107-65bc410765bc"
  }
}
```

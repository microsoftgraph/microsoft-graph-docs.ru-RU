---
title: Получение Девицеманажементдериведкредентиалсеттингс
description: Чтение свойств и связей объекта Девицеманажементдериведкредентиалсеттингс.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f8d9808ea462b33d39560248b9ebebad4727fbda
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43389905"
---
# <a name="get-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="73051-103">Получение Девицеманажементдериведкредентиалсеттингс</span><span class="sxs-lookup"><span data-stu-id="73051-103">Get deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="73051-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73051-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73051-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73051-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73051-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73051-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73051-107">Чтение свойств и связей объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="73051-107">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73051-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="73051-108">Prerequisites</span></span>
<span data-ttu-id="73051-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73051-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73051-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73051-111">Permission type</span></span>|<span data-ttu-id="73051-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73051-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73051-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73051-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="73051-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="73051-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="73051-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73051-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="73051-116">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="73051-116">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="73051-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73051-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="73051-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73051-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73051-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73051-119">Not supported.</span></span>|
|<span data-ttu-id="73051-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="73051-120">Application</span></span>||
|<span data-ttu-id="73051-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="73051-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="73051-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73051-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="73051-123">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="73051-123">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="73051-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73051-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73051-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73051-125">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="73051-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="73051-126">Optional query parameters</span></span>
<span data-ttu-id="73051-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="73051-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73051-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73051-128">Request headers</span></span>
|<span data-ttu-id="73051-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73051-129">Header</span></span>|<span data-ttu-id="73051-130">Значение</span><span class="sxs-lookup"><span data-stu-id="73051-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73051-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="73051-131">Authorization</span></span>|<span data-ttu-id="73051-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73051-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73051-133">Accept</span><span class="sxs-lookup"><span data-stu-id="73051-133">Accept</span></span>|<span data-ttu-id="73051-134">application/json</span><span class="sxs-lookup"><span data-stu-id="73051-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73051-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73051-135">Request body</span></span>
<span data-ttu-id="73051-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73051-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73051-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="73051-137">Response</span></span>
<span data-ttu-id="73051-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73051-138">If successful, this method returns a `200 OK` response code and [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73051-139">Пример</span><span class="sxs-lookup"><span data-stu-id="73051-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="73051-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="73051-140">Request</span></span>
<span data-ttu-id="73051-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73051-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
```

### <a name="response"></a><span data-ttu-id="73051-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="73051-142">Response</span></span>
<span data-ttu-id="73051-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73051-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





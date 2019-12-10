---
title: Получение Девицеманажементдериведкредентиалсеттингс
description: Чтение свойств и связей объекта Девицеманажементдериведкредентиалсеттингс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5519ae01e8091b7f7b55b15b90495d8167ab0c36
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939937"
---
# <a name="get-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="e4df2-103">Получение Девицеманажементдериведкредентиалсеттингс</span><span class="sxs-lookup"><span data-stu-id="e4df2-103">Get deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="e4df2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4df2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4df2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4df2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4df2-106">Чтение свойств и связей объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="e4df2-106">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4df2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e4df2-107">Prerequisites</span></span>
<span data-ttu-id="e4df2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4df2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4df2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4df2-110">Permission type</span></span>|<span data-ttu-id="e4df2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4df2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4df2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4df2-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="e4df2-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="e4df2-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e4df2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4df2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e4df2-115">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="e4df2-115">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="e4df2-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4df2-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e4df2-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4df2-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4df2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4df2-118">Not supported.</span></span>|
|<span data-ttu-id="e4df2-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4df2-119">Application</span></span>||
|<span data-ttu-id="e4df2-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="e4df2-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e4df2-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4df2-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e4df2-122">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="e4df2-122">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="e4df2-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4df2-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4df2-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4df2-124">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="e4df2-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e4df2-125">Optional query parameters</span></span>
<span data-ttu-id="e4df2-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e4df2-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4df2-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4df2-127">Request headers</span></span>
|<span data-ttu-id="e4df2-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4df2-128">Header</span></span>|<span data-ttu-id="e4df2-129">Значение</span><span class="sxs-lookup"><span data-stu-id="e4df2-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4df2-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4df2-130">Authorization</span></span>|<span data-ttu-id="e4df2-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4df2-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4df2-132">Accept</span><span class="sxs-lookup"><span data-stu-id="e4df2-132">Accept</span></span>|<span data-ttu-id="e4df2-133">application/json</span><span class="sxs-lookup"><span data-stu-id="e4df2-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4df2-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4df2-134">Request body</span></span>
<span data-ttu-id="e4df2-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4df2-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4df2-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4df2-136">Response</span></span>
<span data-ttu-id="e4df2-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4df2-137">If successful, this method returns a `200 OK` response code and [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4df2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e4df2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4df2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4df2-139">Request</span></span>
<span data-ttu-id="e4df2-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4df2-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
```

### <a name="response"></a><span data-ttu-id="e4df2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4df2-141">Response</span></span>
<span data-ttu-id="e4df2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4df2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







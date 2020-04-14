---
title: Создание объекта deviceManagementExchangeConnector
description: Создание объекта deviceManagementExchangeConnector.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9613ae194e747657b45baea1e809468feab01b60
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450342"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="ad8d3-103">Создание объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="ad8d3-103">Create deviceManagementExchangeConnector</span></span>

<span data-ttu-id="ad8d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad8d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad8d3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad8d3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad8d3-107">Создание объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="ad8d3-107">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad8d3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ad8d3-108">Prerequisites</span></span>
<span data-ttu-id="ad8d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad8d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad8d3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad8d3-111">Permission type</span></span>|<span data-ttu-id="ad8d3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad8d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad8d3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad8d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad8d3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad8d3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ad8d3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad8d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad8d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-116">Not supported.</span></span>|
|<span data-ttu-id="ad8d3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad8d3-117">Application</span></span>|<span data-ttu-id="ad8d3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad8d3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad8d3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad8d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="ad8d3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ad8d3-120">Request headers</span></span>
|<span data-ttu-id="ad8d3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad8d3-121">Header</span></span>|<span data-ttu-id="ad8d3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad8d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad8d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad8d3-123">Authorization</span></span>|<span data-ttu-id="ad8d3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad8d3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad8d3-125">Accept</span></span>|<span data-ttu-id="ad8d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad8d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad8d3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad8d3-127">Request body</span></span>
<span data-ttu-id="ad8d3-128">В теле запроса добавьте представление объекта deviceManagementExchangeConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-128">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="ad8d3-129">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-129">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="ad8d3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad8d3-130">Property</span></span>|<span data-ttu-id="ad8d3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ad8d3-131">Type</span></span>|<span data-ttu-id="ad8d3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ad8d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad8d3-133">id</span><span class="sxs-lookup"><span data-stu-id="ad8d3-133">id</span></span>|<span data-ttu-id="ad8d3-134">String</span><span class="sxs-lookup"><span data-stu-id="ad8d3-134">String</span></span>|<span data-ttu-id="ad8d3-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ad8d3-135">Not yet documented</span></span>|
|<span data-ttu-id="ad8d3-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ad8d3-136">lastSyncDateTime</span></span>|<span data-ttu-id="ad8d3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad8d3-137">DateTimeOffset</span></span>|<span data-ttu-id="ad8d3-138">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="ad8d3-138">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="ad8d3-139">status</span><span class="sxs-lookup"><span data-stu-id="ad8d3-139">status</span></span>|[<span data-ttu-id="ad8d3-140">девицеманажементексчанжеконнекторстатус</span><span class="sxs-lookup"><span data-stu-id="ad8d3-140">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="ad8d3-141">Состояние соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-141">Exchange Connector Status.</span></span> <span data-ttu-id="ad8d3-142">Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-142">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="ad8d3-143">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="ad8d3-143">primarySmtpAddress</span></span>|<span data-ttu-id="ad8d3-144">String</span><span class="sxs-lookup"><span data-stu-id="ad8d3-144">String</span></span>|<span data-ttu-id="ad8d3-145">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-145">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="ad8d3-146">serverName</span><span class="sxs-lookup"><span data-stu-id="ad8d3-146">serverName</span></span>|<span data-ttu-id="ad8d3-147">String</span><span class="sxs-lookup"><span data-stu-id="ad8d3-147">String</span></span>|<span data-ttu-id="ad8d3-148">Имя сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-148">The name of the Exchange server.</span></span>|
|<span data-ttu-id="ad8d3-149">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="ad8d3-149">connectorServerName</span></span>|<span data-ttu-id="ad8d3-150">String</span><span class="sxs-lookup"><span data-stu-id="ad8d3-150">String</span></span>|<span data-ttu-id="ad8d3-151">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-151">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="ad8d3-152">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="ad8d3-152">exchangeConnectorType</span></span>|[<span data-ttu-id="ad8d3-153">девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="ad8d3-153">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="ad8d3-154">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-154">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="ad8d3-155">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-155">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="ad8d3-156">version</span><span class="sxs-lookup"><span data-stu-id="ad8d3-156">version</span></span>|<span data-ttu-id="ad8d3-157">Строка</span><span class="sxs-lookup"><span data-stu-id="ad8d3-157">String</span></span>|<span data-ttu-id="ad8d3-158">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="ad8d3-158">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="ad8d3-159">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="ad8d3-159">exchangeAlias</span></span>|<span data-ttu-id="ad8d3-160">String</span><span class="sxs-lookup"><span data-stu-id="ad8d3-160">String</span></span>|<span data-ttu-id="ad8d3-161">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="ad8d3-161">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="ad8d3-162">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="ad8d3-162">exchangeOrganization</span></span>|<span data-ttu-id="ad8d3-163">String</span><span class="sxs-lookup"><span data-stu-id="ad8d3-163">String</span></span>|<span data-ttu-id="ad8d3-164">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="ad8d3-164">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="ad8d3-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad8d3-165">Response</span></span>
<span data-ttu-id="ad8d3-166">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-166">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad8d3-167">Пример</span><span class="sxs-lookup"><span data-stu-id="ad8d3-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad8d3-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad8d3-168">Request</span></span>
<span data-ttu-id="ad8d3-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="ad8d3-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad8d3-170">Response</span></span>
<span data-ttu-id="ad8d3-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad8d3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```




---
title: Обновление объекта deviceManagementExchangeConnector
description: Обновление свойств объекта deviceManagementExchangeConnector.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e8d71e8ed9713a4666e4f1ffb695578f7c55b0ed
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512554"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="16b0d-103">Обновление объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="16b0d-103">Update deviceManagementExchangeConnector</span></span>

<span data-ttu-id="16b0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16b0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16b0d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16b0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16b0d-106">Обновление свойств объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="16b0d-106">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16b0d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="16b0d-107">Prerequisites</span></span>
<span data-ttu-id="16b0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16b0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16b0d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16b0d-110">Permission type</span></span>|<span data-ttu-id="16b0d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16b0d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16b0d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16b0d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16b0d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16b0d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="16b0d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16b0d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16b0d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16b0d-115">Not supported.</span></span>|
|<span data-ttu-id="16b0d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16b0d-116">Application</span></span>|<span data-ttu-id="16b0d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16b0d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16b0d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16b0d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="16b0d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="16b0d-119">Request headers</span></span>
|<span data-ttu-id="16b0d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16b0d-120">Header</span></span>|<span data-ttu-id="16b0d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="16b0d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16b0d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16b0d-122">Authorization</span></span>|<span data-ttu-id="16b0d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16b0d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16b0d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="16b0d-124">Accept</span></span>|<span data-ttu-id="16b0d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16b0d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16b0d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16b0d-126">Request body</span></span>
<span data-ttu-id="16b0d-127">В теле запроса добавьте представление объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16b0d-127">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="16b0d-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="16b0d-128">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="16b0d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="16b0d-129">Property</span></span>|<span data-ttu-id="16b0d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="16b0d-130">Type</span></span>|<span data-ttu-id="16b0d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="16b0d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16b0d-132">id</span><span class="sxs-lookup"><span data-stu-id="16b0d-132">id</span></span>|<span data-ttu-id="16b0d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="16b0d-133">String</span></span>|<span data-ttu-id="16b0d-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="16b0d-134">Not yet documented</span></span>|
|<span data-ttu-id="16b0d-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="16b0d-135">lastSyncDateTime</span></span>|<span data-ttu-id="16b0d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16b0d-136">DateTimeOffset</span></span>|<span data-ttu-id="16b0d-137">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="16b0d-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="16b0d-138">status</span><span class="sxs-lookup"><span data-stu-id="16b0d-138">status</span></span>|[<span data-ttu-id="16b0d-139">девицеманажементексчанжеконнекторстатус</span><span class="sxs-lookup"><span data-stu-id="16b0d-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="16b0d-140">Состояние соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="16b0d-140">Exchange Connector Status.</span></span> <span data-ttu-id="16b0d-141">Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="16b0d-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="16b0d-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="16b0d-142">primarySmtpAddress</span></span>|<span data-ttu-id="16b0d-143">Строка</span><span class="sxs-lookup"><span data-stu-id="16b0d-143">String</span></span>|<span data-ttu-id="16b0d-144">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="16b0d-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="16b0d-145">serverName</span><span class="sxs-lookup"><span data-stu-id="16b0d-145">serverName</span></span>|<span data-ttu-id="16b0d-146">Строка</span><span class="sxs-lookup"><span data-stu-id="16b0d-146">String</span></span>|<span data-ttu-id="16b0d-147">Имя сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="16b0d-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="16b0d-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="16b0d-148">connectorServerName</span></span>|<span data-ttu-id="16b0d-149">Строка</span><span class="sxs-lookup"><span data-stu-id="16b0d-149">String</span></span>|<span data-ttu-id="16b0d-150">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="16b0d-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="16b0d-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="16b0d-151">exchangeConnectorType</span></span>|[<span data-ttu-id="16b0d-152">девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="16b0d-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="16b0d-153">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="16b0d-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="16b0d-154">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="16b0d-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="16b0d-155">version</span><span class="sxs-lookup"><span data-stu-id="16b0d-155">version</span></span>|<span data-ttu-id="16b0d-156">Строка</span><span class="sxs-lookup"><span data-stu-id="16b0d-156">String</span></span>|<span data-ttu-id="16b0d-157">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="16b0d-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="16b0d-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="16b0d-158">exchangeAlias</span></span>|<span data-ttu-id="16b0d-159">Строка</span><span class="sxs-lookup"><span data-stu-id="16b0d-159">String</span></span>|<span data-ttu-id="16b0d-160">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="16b0d-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="16b0d-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="16b0d-161">exchangeOrganization</span></span>|<span data-ttu-id="16b0d-162">String</span><span class="sxs-lookup"><span data-stu-id="16b0d-162">String</span></span>|<span data-ttu-id="16b0d-163">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="16b0d-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="16b0d-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="16b0d-164">Response</span></span>
<span data-ttu-id="16b0d-165">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="16b0d-165">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16b0d-166">Пример</span><span class="sxs-lookup"><span data-stu-id="16b0d-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="16b0d-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="16b0d-167">Request</span></span>
<span data-ttu-id="16b0d-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16b0d-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
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

### <a name="response"></a><span data-ttu-id="16b0d-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="16b0d-169">Response</span></span>
<span data-ttu-id="16b0d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16b0d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





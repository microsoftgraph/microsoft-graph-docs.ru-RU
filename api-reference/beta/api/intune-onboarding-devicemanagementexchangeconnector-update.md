---
title: Обновление объекта deviceManagementExchangeConnector
description: Обновление свойств объекта deviceManagementExchangeConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f7caa89b592e6d43e97f3200fad52a52b2e33e4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462147"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="bdd31-103">Обновление объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="bdd31-103">Update deviceManagementExchangeConnector</span></span>

<span data-ttu-id="bdd31-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bdd31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdd31-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdd31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdd31-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdd31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdd31-107">Обновление свойств объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="bdd31-107">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdd31-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bdd31-108">Prerequisites</span></span>
<span data-ttu-id="bdd31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdd31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdd31-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdd31-111">Permission type</span></span>|<span data-ttu-id="bdd31-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdd31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdd31-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdd31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bdd31-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdd31-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bdd31-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdd31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdd31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdd31-116">Not supported.</span></span>|
|<span data-ttu-id="bdd31-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdd31-117">Application</span></span>|<span data-ttu-id="bdd31-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdd31-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdd31-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdd31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="bdd31-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bdd31-120">Request headers</span></span>
|<span data-ttu-id="bdd31-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdd31-121">Header</span></span>|<span data-ttu-id="bdd31-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bdd31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdd31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdd31-123">Authorization</span></span>|<span data-ttu-id="bdd31-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdd31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdd31-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bdd31-125">Accept</span></span>|<span data-ttu-id="bdd31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bdd31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdd31-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdd31-127">Request body</span></span>
<span data-ttu-id="bdd31-128">В теле запроса добавьте представление объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bdd31-128">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="bdd31-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="bdd31-129">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="bdd31-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdd31-130">Property</span></span>|<span data-ttu-id="bdd31-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bdd31-131">Type</span></span>|<span data-ttu-id="bdd31-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bdd31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdd31-133">id</span><span class="sxs-lookup"><span data-stu-id="bdd31-133">id</span></span>|<span data-ttu-id="bdd31-134">String</span><span class="sxs-lookup"><span data-stu-id="bdd31-134">String</span></span>|<span data-ttu-id="bdd31-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bdd31-135">Not yet documented</span></span>|
|<span data-ttu-id="bdd31-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bdd31-136">lastSyncDateTime</span></span>|<span data-ttu-id="bdd31-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdd31-137">DateTimeOffset</span></span>|<span data-ttu-id="bdd31-138">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="bdd31-138">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="bdd31-139">status</span><span class="sxs-lookup"><span data-stu-id="bdd31-139">status</span></span>|[<span data-ttu-id="bdd31-140">девицеманажементексчанжеконнекторстатус</span><span class="sxs-lookup"><span data-stu-id="bdd31-140">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="bdd31-141">Состояние соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="bdd31-141">Exchange Connector Status.</span></span> <span data-ttu-id="bdd31-142">Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="bdd31-142">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="bdd31-143">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="bdd31-143">primarySmtpAddress</span></span>|<span data-ttu-id="bdd31-144">String</span><span class="sxs-lookup"><span data-stu-id="bdd31-144">String</span></span>|<span data-ttu-id="bdd31-145">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="bdd31-145">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="bdd31-146">serverName</span><span class="sxs-lookup"><span data-stu-id="bdd31-146">serverName</span></span>|<span data-ttu-id="bdd31-147">String</span><span class="sxs-lookup"><span data-stu-id="bdd31-147">String</span></span>|<span data-ttu-id="bdd31-148">Имя сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="bdd31-148">The name of the Exchange server.</span></span>|
|<span data-ttu-id="bdd31-149">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="bdd31-149">connectorServerName</span></span>|<span data-ttu-id="bdd31-150">String</span><span class="sxs-lookup"><span data-stu-id="bdd31-150">String</span></span>|<span data-ttu-id="bdd31-151">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="bdd31-151">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="bdd31-152">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="bdd31-152">exchangeConnectorType</span></span>|[<span data-ttu-id="bdd31-153">девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="bdd31-153">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="bdd31-154">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="bdd31-154">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="bdd31-155">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="bdd31-155">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="bdd31-156">version</span><span class="sxs-lookup"><span data-stu-id="bdd31-156">version</span></span>|<span data-ttu-id="bdd31-157">Строка</span><span class="sxs-lookup"><span data-stu-id="bdd31-157">String</span></span>|<span data-ttu-id="bdd31-158">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="bdd31-158">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="bdd31-159">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="bdd31-159">exchangeAlias</span></span>|<span data-ttu-id="bdd31-160">String</span><span class="sxs-lookup"><span data-stu-id="bdd31-160">String</span></span>|<span data-ttu-id="bdd31-161">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="bdd31-161">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="bdd31-162">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="bdd31-162">exchangeOrganization</span></span>|<span data-ttu-id="bdd31-163">String</span><span class="sxs-lookup"><span data-stu-id="bdd31-163">String</span></span>|<span data-ttu-id="bdd31-164">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="bdd31-164">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="bdd31-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdd31-165">Response</span></span>
<span data-ttu-id="bdd31-166">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bdd31-166">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdd31-167">Пример</span><span class="sxs-lookup"><span data-stu-id="bdd31-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdd31-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdd31-168">Request</span></span>
<span data-ttu-id="bdd31-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdd31-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
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

### <a name="response"></a><span data-ttu-id="bdd31-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdd31-170">Response</span></span>
<span data-ttu-id="bdd31-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdd31-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






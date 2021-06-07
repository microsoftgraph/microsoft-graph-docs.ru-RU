---
title: Обновление объекта deviceManagementExchangeConnector
description: Обновление свойств объекта deviceManagementExchangeConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 989e02bd0f5148b04178b34473355c020383bf91
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754799"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="a4ab9-103">Обновление объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="a4ab9-103">Update deviceManagementExchangeConnector</span></span>

<span data-ttu-id="a4ab9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4ab9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4ab9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4ab9-106">Обновление свойств объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="a4ab9-106">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4ab9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a4ab9-107">Prerequisites</span></span>
<span data-ttu-id="a4ab9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4ab9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4ab9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4ab9-110">Permission type</span></span>|<span data-ttu-id="a4ab9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4ab9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4ab9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4ab9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4ab9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4ab9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a4ab9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4ab9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4ab9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-115">Not supported.</span></span>|
|<span data-ttu-id="a4ab9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4ab9-116">Application</span></span>|<span data-ttu-id="a4ab9-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4ab9-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4ab9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4ab9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="a4ab9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a4ab9-119">Request headers</span></span>
|<span data-ttu-id="a4ab9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4ab9-120">Header</span></span>|<span data-ttu-id="a4ab9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a4ab9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4ab9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4ab9-122">Authorization</span></span>|<span data-ttu-id="a4ab9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4ab9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a4ab9-124">Accept</span></span>|<span data-ttu-id="a4ab9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4ab9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4ab9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4ab9-126">Request body</span></span>
<span data-ttu-id="a4ab9-127">В теле запроса добавьте представление объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-127">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="a4ab9-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="a4ab9-128">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="a4ab9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4ab9-129">Property</span></span>|<span data-ttu-id="a4ab9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a4ab9-130">Type</span></span>|<span data-ttu-id="a4ab9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a4ab9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4ab9-132">id</span><span class="sxs-lookup"><span data-stu-id="a4ab9-132">id</span></span>|<span data-ttu-id="a4ab9-133">String</span><span class="sxs-lookup"><span data-stu-id="a4ab9-133">String</span></span>|<span data-ttu-id="a4ab9-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a4ab9-134">Not yet documented</span></span>|
|<span data-ttu-id="a4ab9-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a4ab9-135">lastSyncDateTime</span></span>|<span data-ttu-id="a4ab9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4ab9-136">DateTimeOffset</span></span>|<span data-ttu-id="a4ab9-137">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="a4ab9-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="a4ab9-138">status</span><span class="sxs-lookup"><span data-stu-id="a4ab9-138">status</span></span>|[<span data-ttu-id="a4ab9-139">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="a4ab9-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="a4ab9-140">Exchange Состояние соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-140">Exchange Connector Status.</span></span> <span data-ttu-id="a4ab9-141">Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="a4ab9-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="a4ab9-142">primarySmtpAddress</span></span>|<span data-ttu-id="a4ab9-143">String</span><span class="sxs-lookup"><span data-stu-id="a4ab9-143">String</span></span>|<span data-ttu-id="a4ab9-144">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="a4ab9-145">serverName</span><span class="sxs-lookup"><span data-stu-id="a4ab9-145">serverName</span></span>|<span data-ttu-id="a4ab9-146">String</span><span class="sxs-lookup"><span data-stu-id="a4ab9-146">String</span></span>|<span data-ttu-id="a4ab9-147">Имя сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="a4ab9-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="a4ab9-148">connectorServerName</span></span>|<span data-ttu-id="a4ab9-149">String</span><span class="sxs-lookup"><span data-stu-id="a4ab9-149">String</span></span>|<span data-ttu-id="a4ab9-150">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="a4ab9-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="a4ab9-151">exchangeConnectorType</span></span>|[<span data-ttu-id="a4ab9-152">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="a4ab9-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="a4ab9-153">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="a4ab9-154">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="a4ab9-155">version</span><span class="sxs-lookup"><span data-stu-id="a4ab9-155">version</span></span>|<span data-ttu-id="a4ab9-156">String</span><span class="sxs-lookup"><span data-stu-id="a4ab9-156">String</span></span>|<span data-ttu-id="a4ab9-157">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="a4ab9-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="a4ab9-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="a4ab9-158">exchangeAlias</span></span>|<span data-ttu-id="a4ab9-159">String</span><span class="sxs-lookup"><span data-stu-id="a4ab9-159">String</span></span>|<span data-ttu-id="a4ab9-160">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="a4ab9-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="a4ab9-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="a4ab9-161">exchangeOrganization</span></span>|<span data-ttu-id="a4ab9-162">String</span><span class="sxs-lookup"><span data-stu-id="a4ab9-162">String</span></span>|<span data-ttu-id="a4ab9-163">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="a4ab9-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="a4ab9-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4ab9-164">Response</span></span>
<span data-ttu-id="a4ab9-165">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-165">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4ab9-166">Пример</span><span class="sxs-lookup"><span data-stu-id="a4ab9-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4ab9-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4ab9-167">Request</span></span>
<span data-ttu-id="a4ab9-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a4ab9-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4ab9-169">Response</span></span>
<span data-ttu-id="a4ab9-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





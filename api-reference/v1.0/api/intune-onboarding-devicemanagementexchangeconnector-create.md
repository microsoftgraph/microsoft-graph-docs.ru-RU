---
title: Создание объекта deviceManagementExchangeConnector
description: Создание объекта deviceManagementExchangeConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e28d76266a552470bb5e0ca9b61857c49ccd50c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754834"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="5c0c7-103">Создание объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="5c0c7-103">Create deviceManagementExchangeConnector</span></span>

<span data-ttu-id="5c0c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c0c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c0c7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c0c7-106">Создание объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="5c0c7-106">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c0c7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5c0c7-107">Prerequisites</span></span>
<span data-ttu-id="5c0c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c0c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c0c7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c0c7-110">Permission type</span></span>|<span data-ttu-id="5c0c7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c0c7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c0c7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c0c7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c0c7-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c0c7-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5c0c7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c0c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c0c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-115">Not supported.</span></span>|
|<span data-ttu-id="5c0c7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5c0c7-116">Application</span></span>|<span data-ttu-id="5c0c7-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c0c7-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c0c7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c0c7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="5c0c7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5c0c7-119">Request headers</span></span>
|<span data-ttu-id="5c0c7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c0c7-120">Header</span></span>|<span data-ttu-id="5c0c7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5c0c7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c0c7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c0c7-122">Authorization</span></span>|<span data-ttu-id="5c0c7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c0c7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5c0c7-124">Accept</span></span>|<span data-ttu-id="5c0c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c0c7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c0c7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c0c7-126">Request body</span></span>
<span data-ttu-id="5c0c7-127">В теле запроса добавьте представление объекта deviceManagementExchangeConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-127">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="5c0c7-128">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-128">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="5c0c7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c0c7-129">Property</span></span>|<span data-ttu-id="5c0c7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5c0c7-130">Type</span></span>|<span data-ttu-id="5c0c7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5c0c7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c0c7-132">id</span><span class="sxs-lookup"><span data-stu-id="5c0c7-132">id</span></span>|<span data-ttu-id="5c0c7-133">String</span><span class="sxs-lookup"><span data-stu-id="5c0c7-133">String</span></span>|<span data-ttu-id="5c0c7-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5c0c7-134">Not yet documented</span></span>|
|<span data-ttu-id="5c0c7-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5c0c7-135">lastSyncDateTime</span></span>|<span data-ttu-id="5c0c7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c0c7-136">DateTimeOffset</span></span>|<span data-ttu-id="5c0c7-137">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="5c0c7-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="5c0c7-138">status</span><span class="sxs-lookup"><span data-stu-id="5c0c7-138">status</span></span>|[<span data-ttu-id="5c0c7-139">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="5c0c7-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="5c0c7-140">Exchange Состояние соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-140">Exchange Connector Status.</span></span> <span data-ttu-id="5c0c7-141">Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="5c0c7-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5c0c7-142">primarySmtpAddress</span></span>|<span data-ttu-id="5c0c7-143">String</span><span class="sxs-lookup"><span data-stu-id="5c0c7-143">String</span></span>|<span data-ttu-id="5c0c7-144">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="5c0c7-145">serverName</span><span class="sxs-lookup"><span data-stu-id="5c0c7-145">serverName</span></span>|<span data-ttu-id="5c0c7-146">String</span><span class="sxs-lookup"><span data-stu-id="5c0c7-146">String</span></span>|<span data-ttu-id="5c0c7-147">Имя сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="5c0c7-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="5c0c7-148">connectorServerName</span></span>|<span data-ttu-id="5c0c7-149">String</span><span class="sxs-lookup"><span data-stu-id="5c0c7-149">String</span></span>|<span data-ttu-id="5c0c7-150">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="5c0c7-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="5c0c7-151">exchangeConnectorType</span></span>|[<span data-ttu-id="5c0c7-152">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="5c0c7-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="5c0c7-153">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="5c0c7-154">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="5c0c7-155">version</span><span class="sxs-lookup"><span data-stu-id="5c0c7-155">version</span></span>|<span data-ttu-id="5c0c7-156">String</span><span class="sxs-lookup"><span data-stu-id="5c0c7-156">String</span></span>|<span data-ttu-id="5c0c7-157">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="5c0c7-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="5c0c7-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="5c0c7-158">exchangeAlias</span></span>|<span data-ttu-id="5c0c7-159">String</span><span class="sxs-lookup"><span data-stu-id="5c0c7-159">String</span></span>|<span data-ttu-id="5c0c7-160">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="5c0c7-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="5c0c7-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="5c0c7-161">exchangeOrganization</span></span>|<span data-ttu-id="5c0c7-162">String</span><span class="sxs-lookup"><span data-stu-id="5c0c7-162">String</span></span>|<span data-ttu-id="5c0c7-163">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="5c0c7-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="5c0c7-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c0c7-164">Response</span></span>
<span data-ttu-id="5c0c7-165">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-165">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c0c7-166">Пример</span><span class="sxs-lookup"><span data-stu-id="5c0c7-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c0c7-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c0c7-167">Request</span></span>
<span data-ttu-id="5c0c7-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
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

### <a name="response"></a><span data-ttu-id="5c0c7-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c0c7-169">Response</span></span>
<span data-ttu-id="5c0c7-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c0c7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





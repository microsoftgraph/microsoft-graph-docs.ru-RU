---
title: Создание объекта deviceManagementExchangeConnector
description: Создание объекта deviceManagementExchangeConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2226d76903612062e97ec382bd67be1fc253c6d7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900179"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="8b3e6-103">Создание объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="8b3e6-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="8b3e6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b3e6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b3e6-106">Создание объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="8b3e6-106">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b3e6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8b3e6-107">Prerequisites</span></span>
<span data-ttu-id="8b3e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b3e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b3e6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b3e6-110">Permission type</span></span>|<span data-ttu-id="8b3e6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b3e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b3e6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b3e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b3e6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b3e6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8b3e6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b3e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b3e6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-115">Not supported.</span></span>|
|<span data-ttu-id="8b3e6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b3e6-116">Application</span></span>|<span data-ttu-id="8b3e6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b3e6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b3e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="8b3e6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b3e6-119">Request headers</span></span>
|<span data-ttu-id="8b3e6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b3e6-120">Header</span></span>|<span data-ttu-id="8b3e6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8b3e6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b3e6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b3e6-122">Authorization</span></span>|<span data-ttu-id="8b3e6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b3e6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8b3e6-124">Accept</span></span>|<span data-ttu-id="8b3e6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b3e6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b3e6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b3e6-126">Request body</span></span>
<span data-ttu-id="8b3e6-127">В теле запроса добавьте представление объекта deviceManagementExchangeConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-127">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="8b3e6-128">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-128">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="8b3e6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b3e6-129">Property</span></span>|<span data-ttu-id="8b3e6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8b3e6-130">Type</span></span>|<span data-ttu-id="8b3e6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8b3e6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b3e6-132">id</span><span class="sxs-lookup"><span data-stu-id="8b3e6-132">id</span></span>|<span data-ttu-id="8b3e6-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8b3e6-133">String</span></span>|<span data-ttu-id="8b3e6-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b3e6-134">Not yet documented</span></span>|
|<span data-ttu-id="8b3e6-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8b3e6-135">lastSyncDateTime</span></span>|<span data-ttu-id="8b3e6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b3e6-136">DateTimeOffset</span></span>|<span data-ttu-id="8b3e6-137">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="8b3e6-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="8b3e6-138">status</span><span class="sxs-lookup"><span data-stu-id="8b3e6-138">status</span></span>|[<span data-ttu-id="8b3e6-139">Девицеманажементексчанжеконнекторстатус</span><span class="sxs-lookup"><span data-stu-id="8b3e6-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="8b3e6-140">Состояние соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-140">Exchange Connector Status.</span></span> <span data-ttu-id="8b3e6-141">Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="8b3e6-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="8b3e6-142">primarySmtpAddress</span></span>|<span data-ttu-id="8b3e6-143">Строка</span><span class="sxs-lookup"><span data-stu-id="8b3e6-143">String</span></span>|<span data-ttu-id="8b3e6-144">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="8b3e6-145">serverName</span><span class="sxs-lookup"><span data-stu-id="8b3e6-145">serverName</span></span>|<span data-ttu-id="8b3e6-146">Строка</span><span class="sxs-lookup"><span data-stu-id="8b3e6-146">String</span></span>|<span data-ttu-id="8b3e6-147">Имя сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="8b3e6-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="8b3e6-148">connectorServerName</span></span>|<span data-ttu-id="8b3e6-149">Строка</span><span class="sxs-lookup"><span data-stu-id="8b3e6-149">String</span></span>|<span data-ttu-id="8b3e6-150">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="8b3e6-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="8b3e6-151">exchangeConnectorType</span></span>|[<span data-ttu-id="8b3e6-152">Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="8b3e6-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="8b3e6-153">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="8b3e6-154">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="8b3e6-155">version</span><span class="sxs-lookup"><span data-stu-id="8b3e6-155">version</span></span>|<span data-ttu-id="8b3e6-156">Строка</span><span class="sxs-lookup"><span data-stu-id="8b3e6-156">String</span></span>|<span data-ttu-id="8b3e6-157">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="8b3e6-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="8b3e6-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="8b3e6-158">exchangeAlias</span></span>|<span data-ttu-id="8b3e6-159">Строка</span><span class="sxs-lookup"><span data-stu-id="8b3e6-159">String</span></span>|<span data-ttu-id="8b3e6-160">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="8b3e6-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="8b3e6-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="8b3e6-161">exchangeOrganization</span></span>|<span data-ttu-id="8b3e6-162">String</span><span class="sxs-lookup"><span data-stu-id="8b3e6-162">String</span></span>|<span data-ttu-id="8b3e6-163">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="8b3e6-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="8b3e6-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b3e6-164">Response</span></span>
<span data-ttu-id="8b3e6-165">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-165">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b3e6-166">Пример</span><span class="sxs-lookup"><span data-stu-id="8b3e6-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b3e6-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b3e6-167">Request</span></span>
<span data-ttu-id="8b3e6-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8b3e6-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b3e6-169">Response</span></span>
<span data-ttu-id="8b3e6-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b3e6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





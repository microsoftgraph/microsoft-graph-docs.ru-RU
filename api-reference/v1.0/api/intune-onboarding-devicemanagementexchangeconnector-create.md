---
title: Создание объекта deviceManagementExchangeConnector
description: Создание объекта deviceManagementExchangeConnector.
ms.openlocfilehash: 710f2a1d43f95a8a3ca6f6f154a667b78e8c0795
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024994"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="4d8b1-103">Создание объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="4d8b1-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="4d8b1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d8b1-105">Создание объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="4d8b1-105">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d8b1-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4d8b1-106">Prerequisites</span></span>
<span data-ttu-id="4d8b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d8b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d8b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d8b1-109">Permission type</span></span>|<span data-ttu-id="4d8b1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d8b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d8b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d8b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d8b1-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d8b1-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4d8b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d8b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d8b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-114">Not supported.</span></span>|
|<span data-ttu-id="4d8b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d8b1-115">Application</span></span>|<span data-ttu-id="4d8b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d8b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d8b1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="4d8b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d8b1-118">Request headers</span></span>
|<span data-ttu-id="4d8b1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d8b1-119">Header</span></span>|<span data-ttu-id="4d8b1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4d8b1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d8b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d8b1-121">Authorization</span></span>|<span data-ttu-id="4d8b1-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4d8b1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d8b1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4d8b1-123">Accept</span></span>|<span data-ttu-id="4d8b1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4d8b1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d8b1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d8b1-125">Request body</span></span>
<span data-ttu-id="4d8b1-126">В теле запроса добавьте представление объекта deviceManagementExchangeConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-126">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="4d8b1-127">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-127">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="4d8b1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d8b1-128">Property</span></span>|<span data-ttu-id="4d8b1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4d8b1-129">Type</span></span>|<span data-ttu-id="4d8b1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4d8b1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d8b1-131">id</span><span class="sxs-lookup"><span data-stu-id="4d8b1-131">id</span></span>|<span data-ttu-id="4d8b1-132">String</span><span class="sxs-lookup"><span data-stu-id="4d8b1-132">String</span></span>|<span data-ttu-id="4d8b1-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4d8b1-133">Not yet documented</span></span>|
|<span data-ttu-id="4d8b1-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4d8b1-134">lastSyncDateTime</span></span>|<span data-ttu-id="4d8b1-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d8b1-135">DateTimeOffset</span></span>|<span data-ttu-id="4d8b1-136">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="4d8b1-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="4d8b1-137">status</span><span class="sxs-lookup"><span data-stu-id="4d8b1-137">status</span></span>|[<span data-ttu-id="4d8b1-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="4d8b1-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="4d8b1-139">Состояние соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-139">Exchange Connector Status.</span></span> <span data-ttu-id="4d8b1-140">Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="4d8b1-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="4d8b1-141">primarySmtpAddress</span></span>|<span data-ttu-id="4d8b1-142">String</span><span class="sxs-lookup"><span data-stu-id="4d8b1-142">String</span></span>|<span data-ttu-id="4d8b1-143">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="4d8b1-144">serverName</span><span class="sxs-lookup"><span data-stu-id="4d8b1-144">serverName</span></span>|<span data-ttu-id="4d8b1-145">String</span><span class="sxs-lookup"><span data-stu-id="4d8b1-145">String</span></span>|<span data-ttu-id="4d8b1-146">Имя сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="4d8b1-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="4d8b1-147">connectorServerName</span></span>|<span data-ttu-id="4d8b1-148">String</span><span class="sxs-lookup"><span data-stu-id="4d8b1-148">String</span></span>|<span data-ttu-id="4d8b1-149">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="4d8b1-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="4d8b1-150">exchangeConnectorType</span></span>|[<span data-ttu-id="4d8b1-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="4d8b1-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="4d8b1-152">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="4d8b1-153">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="4d8b1-154">version</span><span class="sxs-lookup"><span data-stu-id="4d8b1-154">version</span></span>|<span data-ttu-id="4d8b1-155">String</span><span class="sxs-lookup"><span data-stu-id="4d8b1-155">String</span></span>|<span data-ttu-id="4d8b1-156">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="4d8b1-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="4d8b1-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="4d8b1-157">exchangeAlias</span></span>|<span data-ttu-id="4d8b1-158">String</span><span class="sxs-lookup"><span data-stu-id="4d8b1-158">String</span></span>|<span data-ttu-id="4d8b1-159">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="4d8b1-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="4d8b1-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="4d8b1-160">exchangeOrganization</span></span>|<span data-ttu-id="4d8b1-161">String</span><span class="sxs-lookup"><span data-stu-id="4d8b1-161">String</span></span>|<span data-ttu-id="4d8b1-162">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="4d8b1-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="4d8b1-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d8b1-163">Response</span></span>
<span data-ttu-id="4d8b1-164">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-164">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d8b1-165">Пример</span><span class="sxs-lookup"><span data-stu-id="4d8b1-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d8b1-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d8b1-166">Request</span></span>
<span data-ttu-id="4d8b1-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d8b1-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d8b1-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d8b1-168">Response</span></span>
<span data-ttu-id="4d8b1-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4d8b1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




---
title: Создание объекта deviceManagementExchangeConnector
description: Создание объекта deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 292562a2a7083e63f083d0ccad5e11071a27ce96
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256443"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="47de7-103">Создание объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="47de7-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="47de7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47de7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47de7-105">Создание объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="47de7-105">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47de7-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="47de7-106">Prerequisites</span></span>
<span data-ttu-id="47de7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="47de7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="47de7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47de7-109">Permission type</span></span>|<span data-ttu-id="47de7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47de7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47de7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47de7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47de7-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47de7-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="47de7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47de7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47de7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47de7-114">Not supported.</span></span>|
|<span data-ttu-id="47de7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47de7-115">Application</span></span>|<span data-ttu-id="47de7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47de7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47de7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47de7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="47de7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47de7-118">Request headers</span></span>
|<span data-ttu-id="47de7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47de7-119">Header</span></span>|<span data-ttu-id="47de7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="47de7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47de7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="47de7-121">Authorization</span></span>|<span data-ttu-id="47de7-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="47de7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47de7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="47de7-123">Accept</span></span>|<span data-ttu-id="47de7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="47de7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47de7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47de7-125">Request body</span></span>
<span data-ttu-id="47de7-126">В теле запроса добавьте представление объекта deviceManagementExchangeConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47de7-126">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="47de7-127">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="47de7-127">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="47de7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="47de7-128">Property</span></span>|<span data-ttu-id="47de7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="47de7-129">Type</span></span>|<span data-ttu-id="47de7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="47de7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47de7-131">id</span><span class="sxs-lookup"><span data-stu-id="47de7-131">id</span></span>|<span data-ttu-id="47de7-132">Строка</span><span class="sxs-lookup"><span data-stu-id="47de7-132">String</span></span>|<span data-ttu-id="47de7-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="47de7-133">Not yet documented</span></span>|
|<span data-ttu-id="47de7-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="47de7-134">lastSyncDateTime</span></span>|<span data-ttu-id="47de7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47de7-135">DateTimeOffset</span></span>|<span data-ttu-id="47de7-136">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="47de7-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="47de7-137">status</span><span class="sxs-lookup"><span data-stu-id="47de7-137">status</span></span>|[<span data-ttu-id="47de7-138">Девицеманажементексчанжеконнекторстатус</span><span class="sxs-lookup"><span data-stu-id="47de7-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="47de7-139">Состояние соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="47de7-139">Exchange Connector Status.</span></span> <span data-ttu-id="47de7-140">Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="47de7-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="47de7-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="47de7-141">primarySmtpAddress</span></span>|<span data-ttu-id="47de7-142">String</span><span class="sxs-lookup"><span data-stu-id="47de7-142">String</span></span>|<span data-ttu-id="47de7-143">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="47de7-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="47de7-144">serverName</span><span class="sxs-lookup"><span data-stu-id="47de7-144">serverName</span></span>|<span data-ttu-id="47de7-145">String</span><span class="sxs-lookup"><span data-stu-id="47de7-145">String</span></span>|<span data-ttu-id="47de7-146">Имя сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="47de7-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="47de7-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="47de7-147">connectorServerName</span></span>|<span data-ttu-id="47de7-148">String</span><span class="sxs-lookup"><span data-stu-id="47de7-148">String</span></span>|<span data-ttu-id="47de7-149">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="47de7-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="47de7-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="47de7-150">exchangeConnectorType</span></span>|[<span data-ttu-id="47de7-151">Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="47de7-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="47de7-152">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="47de7-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="47de7-153">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="47de7-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="47de7-154">version</span><span class="sxs-lookup"><span data-stu-id="47de7-154">version</span></span>|<span data-ttu-id="47de7-155">Строка</span><span class="sxs-lookup"><span data-stu-id="47de7-155">String</span></span>|<span data-ttu-id="47de7-156">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="47de7-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="47de7-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="47de7-157">exchangeAlias</span></span>|<span data-ttu-id="47de7-158">String</span><span class="sxs-lookup"><span data-stu-id="47de7-158">String</span></span>|<span data-ttu-id="47de7-159">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="47de7-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="47de7-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="47de7-160">exchangeOrganization</span></span>|<span data-ttu-id="47de7-161">String</span><span class="sxs-lookup"><span data-stu-id="47de7-161">String</span></span>|<span data-ttu-id="47de7-162">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="47de7-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="47de7-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="47de7-163">Response</span></span>
<span data-ttu-id="47de7-164">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="47de7-164">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47de7-165">Пример</span><span class="sxs-lookup"><span data-stu-id="47de7-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="47de7-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="47de7-166">Request</span></span>
<span data-ttu-id="47de7-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47de7-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47de7-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="47de7-168">Response</span></span>
<span data-ttu-id="47de7-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="47de7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




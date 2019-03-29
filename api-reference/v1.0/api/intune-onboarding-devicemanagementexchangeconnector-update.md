---
title: Обновление объекта deviceManagementExchangeConnector
description: Обновление свойств объекта deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3e8784796577f08bf8c1f30a748513ff5e081c9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957425"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="a7b2c-103">Обновление объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="a7b2c-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="a7b2c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7b2c-105">Обновление свойств объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="a7b2c-105">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7b2c-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a7b2c-106">Prerequisites</span></span>
<span data-ttu-id="a7b2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7b2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7b2c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7b2c-109">Permission type</span></span>|<span data-ttu-id="a7b2c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7b2c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7b2c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7b2c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7b2c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7b2c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a7b2c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7b2c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7b2c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-114">Not supported.</span></span>|
|<span data-ttu-id="a7b2c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7b2c-115">Application</span></span>|<span data-ttu-id="a7b2c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7b2c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7b2c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="a7b2c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7b2c-118">Request headers</span></span>
|<span data-ttu-id="a7b2c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7b2c-119">Header</span></span>|<span data-ttu-id="a7b2c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a7b2c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7b2c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7b2c-121">Authorization</span></span>|<span data-ttu-id="a7b2c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7b2c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a7b2c-123">Accept</span></span>|<span data-ttu-id="a7b2c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a7b2c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7b2c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7b2c-125">Request body</span></span>
<span data-ttu-id="a7b2c-126">В теле запроса добавьте представление объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-126">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="a7b2c-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="a7b2c-127">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="a7b2c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7b2c-128">Property</span></span>|<span data-ttu-id="a7b2c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a7b2c-129">Type</span></span>|<span data-ttu-id="a7b2c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a7b2c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7b2c-131">id</span><span class="sxs-lookup"><span data-stu-id="a7b2c-131">id</span></span>|<span data-ttu-id="a7b2c-132">String</span><span class="sxs-lookup"><span data-stu-id="a7b2c-132">String</span></span>|<span data-ttu-id="a7b2c-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a7b2c-133">Not yet documented</span></span>|
|<span data-ttu-id="a7b2c-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a7b2c-134">lastSyncDateTime</span></span>|<span data-ttu-id="a7b2c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7b2c-135">DateTimeOffset</span></span>|<span data-ttu-id="a7b2c-136">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="a7b2c-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="a7b2c-137">status</span><span class="sxs-lookup"><span data-stu-id="a7b2c-137">status</span></span>|[<span data-ttu-id="a7b2c-138">Девицеманажементексчанжеконнекторстатус</span><span class="sxs-lookup"><span data-stu-id="a7b2c-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="a7b2c-139">Состояние соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-139">Exchange Connector Status.</span></span> <span data-ttu-id="a7b2c-140">Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="a7b2c-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="a7b2c-141">primarySmtpAddress</span></span>|<span data-ttu-id="a7b2c-142">String</span><span class="sxs-lookup"><span data-stu-id="a7b2c-142">String</span></span>|<span data-ttu-id="a7b2c-143">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="a7b2c-144">serverName</span><span class="sxs-lookup"><span data-stu-id="a7b2c-144">serverName</span></span>|<span data-ttu-id="a7b2c-145">String</span><span class="sxs-lookup"><span data-stu-id="a7b2c-145">String</span></span>|<span data-ttu-id="a7b2c-146">Имя сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="a7b2c-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="a7b2c-147">connectorServerName</span></span>|<span data-ttu-id="a7b2c-148">String</span><span class="sxs-lookup"><span data-stu-id="a7b2c-148">String</span></span>|<span data-ttu-id="a7b2c-149">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="a7b2c-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="a7b2c-150">exchangeConnectorType</span></span>|[<span data-ttu-id="a7b2c-151">Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="a7b2c-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="a7b2c-152">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="a7b2c-153">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="a7b2c-154">version</span><span class="sxs-lookup"><span data-stu-id="a7b2c-154">version</span></span>|<span data-ttu-id="a7b2c-155">Строка</span><span class="sxs-lookup"><span data-stu-id="a7b2c-155">String</span></span>|<span data-ttu-id="a7b2c-156">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="a7b2c-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="a7b2c-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="a7b2c-157">exchangeAlias</span></span>|<span data-ttu-id="a7b2c-158">String</span><span class="sxs-lookup"><span data-stu-id="a7b2c-158">String</span></span>|<span data-ttu-id="a7b2c-159">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="a7b2c-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="a7b2c-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="a7b2c-160">exchangeOrganization</span></span>|<span data-ttu-id="a7b2c-161">String</span><span class="sxs-lookup"><span data-stu-id="a7b2c-161">String</span></span>|<span data-ttu-id="a7b2c-162">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="a7b2c-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="a7b2c-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7b2c-163">Response</span></span>
<span data-ttu-id="a7b2c-164">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7b2c-165">Пример</span><span class="sxs-lookup"><span data-stu-id="a7b2c-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7b2c-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7b2c-166">Request</span></span>
<span data-ttu-id="a7b2c-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a7b2c-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7b2c-168">Response</span></span>
<span data-ttu-id="a7b2c-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7b2c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




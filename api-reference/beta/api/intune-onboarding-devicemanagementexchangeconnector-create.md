---
title: Создание объекта deviceManagementExchangeConnector
description: Создание объекта deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e6961c5a4279e69fb264abe7ed0fd4d960226c12
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528822"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="ea009-103">Создание объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="ea009-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="ea009-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea009-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea009-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea009-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea009-106">Создание объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="ea009-106">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea009-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea009-107">Prerequisites</span></span>
<span data-ttu-id="ea009-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea009-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea009-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea009-110">Permission type</span></span>|<span data-ttu-id="ea009-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea009-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea009-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea009-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea009-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea009-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ea009-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea009-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea009-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea009-115">Not supported.</span></span>|
|<span data-ttu-id="ea009-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea009-116">Application</span></span>|<span data-ttu-id="ea009-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea009-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea009-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea009-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="ea009-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea009-119">Request headers</span></span>
|<span data-ttu-id="ea009-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea009-120">Header</span></span>|<span data-ttu-id="ea009-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ea009-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea009-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea009-122">Authorization</span></span>|<span data-ttu-id="ea009-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea009-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea009-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ea009-124">Accept</span></span>|<span data-ttu-id="ea009-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea009-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea009-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea009-126">Request body</span></span>
<span data-ttu-id="ea009-127">В теле запроса добавьте представление объекта deviceManagementExchangeConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea009-127">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="ea009-128">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="ea009-128">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="ea009-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea009-129">Property</span></span>|<span data-ttu-id="ea009-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ea009-130">Type</span></span>|<span data-ttu-id="ea009-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ea009-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea009-132">id</span><span class="sxs-lookup"><span data-stu-id="ea009-132">id</span></span>|<span data-ttu-id="ea009-133">String</span><span class="sxs-lookup"><span data-stu-id="ea009-133">String</span></span>|<span data-ttu-id="ea009-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ea009-134">Not yet documented</span></span>|
|<span data-ttu-id="ea009-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ea009-135">lastSyncDateTime</span></span>|<span data-ttu-id="ea009-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea009-136">DateTimeOffset</span></span>|<span data-ttu-id="ea009-137">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="ea009-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="ea009-138">status</span><span class="sxs-lookup"><span data-stu-id="ea009-138">status</span></span>|[<span data-ttu-id="ea009-139">Девицеманажементексчанжеконнекторстатус</span><span class="sxs-lookup"><span data-stu-id="ea009-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="ea009-140">Состояние соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="ea009-140">Exchange Connector Status.</span></span> <span data-ttu-id="ea009-141">Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="ea009-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="ea009-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="ea009-142">primarySmtpAddress</span></span>|<span data-ttu-id="ea009-143">String</span><span class="sxs-lookup"><span data-stu-id="ea009-143">String</span></span>|<span data-ttu-id="ea009-144">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="ea009-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="ea009-145">serverName</span><span class="sxs-lookup"><span data-stu-id="ea009-145">serverName</span></span>|<span data-ttu-id="ea009-146">String</span><span class="sxs-lookup"><span data-stu-id="ea009-146">String</span></span>|<span data-ttu-id="ea009-147">Имя сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="ea009-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="ea009-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="ea009-148">connectorServerName</span></span>|<span data-ttu-id="ea009-149">String</span><span class="sxs-lookup"><span data-stu-id="ea009-149">String</span></span>|<span data-ttu-id="ea009-150">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="ea009-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="ea009-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="ea009-151">exchangeConnectorType</span></span>|[<span data-ttu-id="ea009-152">Девицеманажементексчанжеконнектортипе</span><span class="sxs-lookup"><span data-stu-id="ea009-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="ea009-153">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="ea009-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="ea009-154">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="ea009-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="ea009-155">version</span><span class="sxs-lookup"><span data-stu-id="ea009-155">version</span></span>|<span data-ttu-id="ea009-156">Строка</span><span class="sxs-lookup"><span data-stu-id="ea009-156">String</span></span>|<span data-ttu-id="ea009-157">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="ea009-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="ea009-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="ea009-158">exchangeAlias</span></span>|<span data-ttu-id="ea009-159">String</span><span class="sxs-lookup"><span data-stu-id="ea009-159">String</span></span>|<span data-ttu-id="ea009-160">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="ea009-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="ea009-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="ea009-161">exchangeOrganization</span></span>|<span data-ttu-id="ea009-162">String</span><span class="sxs-lookup"><span data-stu-id="ea009-162">String</span></span>|<span data-ttu-id="ea009-163">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="ea009-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="ea009-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea009-164">Response</span></span>
<span data-ttu-id="ea009-165">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ea009-165">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea009-166">Пример</span><span class="sxs-lookup"><span data-stu-id="ea009-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea009-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea009-167">Request</span></span>
<span data-ttu-id="ea009-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea009-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ea009-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea009-169">Response</span></span>
<span data-ttu-id="ea009-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea009-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






---
title: Обновление объекта deviceManagementExchangeConnector
description: Обновление свойств объекта deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5bb6a490f5f192a673a050f9c4711fd4981665d3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865998"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="675b8-103">Обновление объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="675b8-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="675b8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="675b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="675b8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="675b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="675b8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="675b8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="675b8-107">Обновление свойств объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="675b8-107">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="675b8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="675b8-108">Prerequisites</span></span>
<span data-ttu-id="675b8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="675b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="675b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="675b8-111">Permission type</span></span>|<span data-ttu-id="675b8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="675b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="675b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="675b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="675b8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="675b8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="675b8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="675b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="675b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="675b8-116">Not supported.</span></span>|
|<span data-ttu-id="675b8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="675b8-117">Application</span></span>|<span data-ttu-id="675b8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="675b8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="675b8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="675b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="675b8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="675b8-120">Request headers</span></span>
|<span data-ttu-id="675b8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="675b8-121">Header</span></span>|<span data-ttu-id="675b8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="675b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="675b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="675b8-123">Authorization</span></span>|<span data-ttu-id="675b8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="675b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="675b8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="675b8-125">Accept</span></span>|<span data-ttu-id="675b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="675b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="675b8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="675b8-127">Request body</span></span>
<span data-ttu-id="675b8-128">В теле запроса добавьте представление объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="675b8-128">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="675b8-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="675b8-129">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="675b8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="675b8-130">Property</span></span>|<span data-ttu-id="675b8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="675b8-131">Type</span></span>|<span data-ttu-id="675b8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="675b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="675b8-133">id</span><span class="sxs-lookup"><span data-stu-id="675b8-133">id</span></span>|<span data-ttu-id="675b8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="675b8-134">String</span></span>|<span data-ttu-id="675b8-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="675b8-135">Not yet documented</span></span>|
|<span data-ttu-id="675b8-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="675b8-136">lastSyncDateTime</span></span>|<span data-ttu-id="675b8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="675b8-137">DateTimeOffset</span></span>|<span data-ttu-id="675b8-138">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="675b8-138">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="675b8-139">status</span><span class="sxs-lookup"><span data-stu-id="675b8-139">status</span></span>|[<span data-ttu-id="675b8-140">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="675b8-140">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="675b8-141">Состояние соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="675b8-141">Exchange Connector Status.</span></span> <span data-ttu-id="675b8-142">Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="675b8-142">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="675b8-143">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="675b8-143">primarySmtpAddress</span></span>|<span data-ttu-id="675b8-144">String</span><span class="sxs-lookup"><span data-stu-id="675b8-144">String</span></span>|<span data-ttu-id="675b8-145">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="675b8-145">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="675b8-146">serverName</span><span class="sxs-lookup"><span data-stu-id="675b8-146">serverName</span></span>|<span data-ttu-id="675b8-147">String</span><span class="sxs-lookup"><span data-stu-id="675b8-147">String</span></span>|<span data-ttu-id="675b8-148">Имя сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="675b8-148">The name of the Exchange server.</span></span>|
|<span data-ttu-id="675b8-149">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="675b8-149">connectorServerName</span></span>|<span data-ttu-id="675b8-150">String</span><span class="sxs-lookup"><span data-stu-id="675b8-150">String</span></span>|<span data-ttu-id="675b8-151">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="675b8-151">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="675b8-152">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="675b8-152">exchangeConnectorType</span></span>|[<span data-ttu-id="675b8-153">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="675b8-153">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="675b8-154">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="675b8-154">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="675b8-155">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="675b8-155">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="675b8-156">version</span><span class="sxs-lookup"><span data-stu-id="675b8-156">version</span></span>|<span data-ttu-id="675b8-157">String</span><span class="sxs-lookup"><span data-stu-id="675b8-157">String</span></span>|<span data-ttu-id="675b8-158">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="675b8-158">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="675b8-159">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="675b8-159">exchangeAlias</span></span>|<span data-ttu-id="675b8-160">String</span><span class="sxs-lookup"><span data-stu-id="675b8-160">String</span></span>|<span data-ttu-id="675b8-161">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="675b8-161">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="675b8-162">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="675b8-162">exchangeOrganization</span></span>|<span data-ttu-id="675b8-163">String</span><span class="sxs-lookup"><span data-stu-id="675b8-163">String</span></span>|<span data-ttu-id="675b8-164">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="675b8-164">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="675b8-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="675b8-165">Response</span></span>
<span data-ttu-id="675b8-166">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="675b8-166">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="675b8-167">Пример</span><span class="sxs-lookup"><span data-stu-id="675b8-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="675b8-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="675b8-168">Request</span></span>
<span data-ttu-id="675b8-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="675b8-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
Content-type: application/json
Content-length: 418

{
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

### <a name="response"></a><span data-ttu-id="675b8-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="675b8-170">Response</span></span>
<span data-ttu-id="675b8-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="675b8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






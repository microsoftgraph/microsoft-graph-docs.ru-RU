---
title: Создание Девицеманажементдомаинжоинконнектор
description: Создание нового объекта Девицеманажементдомаинжоинконнектор.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 13b6e4dd2c2aff14b4c1003cf354e126d37ab75e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462647"
---
# <a name="create-devicemanagementdomainjoinconnector"></a><span data-ttu-id="48e94-103">Создание Девицеманажементдомаинжоинконнектор</span><span class="sxs-lookup"><span data-stu-id="48e94-103">Create deviceManagementDomainJoinConnector</span></span>

<span data-ttu-id="48e94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48e94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48e94-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48e94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48e94-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48e94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48e94-107">Создание нового объекта [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="48e94-107">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48e94-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="48e94-108">Prerequisites</span></span>
<span data-ttu-id="48e94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48e94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48e94-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48e94-111">Permission type</span></span>|<span data-ttu-id="48e94-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48e94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48e94-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48e94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48e94-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e94-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48e94-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48e94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48e94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48e94-116">Not supported.</span></span>|
|<span data-ttu-id="48e94-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48e94-117">Application</span></span>|<span data-ttu-id="48e94-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e94-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48e94-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48e94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="48e94-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="48e94-120">Request headers</span></span>
|<span data-ttu-id="48e94-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48e94-121">Header</span></span>|<span data-ttu-id="48e94-122">Значение</span><span class="sxs-lookup"><span data-stu-id="48e94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48e94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="48e94-123">Authorization</span></span>|<span data-ttu-id="48e94-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48e94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48e94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48e94-125">Accept</span></span>|<span data-ttu-id="48e94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48e94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48e94-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48e94-127">Request body</span></span>
<span data-ttu-id="48e94-128">В тексте запроса добавьте представление объекта Девицеманажементдомаинжоинконнектор в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48e94-128">In the request body, supply a JSON representation for the deviceManagementDomainJoinConnector object.</span></span>

<span data-ttu-id="48e94-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементдомаинжоинконнектор.</span><span class="sxs-lookup"><span data-stu-id="48e94-129">The following table shows the properties that are required when you create the deviceManagementDomainJoinConnector.</span></span>

|<span data-ttu-id="48e94-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="48e94-130">Property</span></span>|<span data-ttu-id="48e94-131">Тип</span><span class="sxs-lookup"><span data-stu-id="48e94-131">Type</span></span>|<span data-ttu-id="48e94-132">Описание</span><span class="sxs-lookup"><span data-stu-id="48e94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e94-133">id</span><span class="sxs-lookup"><span data-stu-id="48e94-133">id</span></span>|<span data-ttu-id="48e94-134">String</span><span class="sxs-lookup"><span data-stu-id="48e94-134">String</span></span>|<span data-ttu-id="48e94-135">Уникальный идентификатор, представляющий соединитель.</span><span class="sxs-lookup"><span data-stu-id="48e94-135">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="48e94-136">displayName</span><span class="sxs-lookup"><span data-stu-id="48e94-136">displayName</span></span>|<span data-ttu-id="48e94-137">Строка</span><span class="sxs-lookup"><span data-stu-id="48e94-137">String</span></span>|<span data-ttu-id="48e94-138">Отображаемое имя соединителя.</span><span class="sxs-lookup"><span data-stu-id="48e94-138">The connector display name.</span></span>|
|<span data-ttu-id="48e94-139">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="48e94-139">lastConnectionDateTime</span></span>|<span data-ttu-id="48e94-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48e94-140">DateTimeOffset</span></span>|<span data-ttu-id="48e94-141">Последний соединитель времени с обращением к Intune.</span><span class="sxs-lookup"><span data-stu-id="48e94-141">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="48e94-142">state</span><span class="sxs-lookup"><span data-stu-id="48e94-142">state</span></span>|[<span data-ttu-id="48e94-143">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="48e94-143">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="48e94-144">Состояние соединителя.</span><span class="sxs-lookup"><span data-stu-id="48e94-144">The connector state.</span></span> <span data-ttu-id="48e94-145">Возможные значения: `active`, `error`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="48e94-145">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="48e94-146">version</span><span class="sxs-lookup"><span data-stu-id="48e94-146">version</span></span>|<span data-ttu-id="48e94-147">String</span><span class="sxs-lookup"><span data-stu-id="48e94-147">String</span></span>|<span data-ttu-id="48e94-148">Версия соединителя.</span><span class="sxs-lookup"><span data-stu-id="48e94-148">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="48e94-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="48e94-149">Response</span></span>
<span data-ttu-id="48e94-150">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48e94-150">If successful, this method returns a `201 Created` response code and a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48e94-151">Пример</span><span class="sxs-lookup"><span data-stu-id="48e94-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="48e94-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="48e94-152">Request</span></span>
<span data-ttu-id="48e94-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48e94-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "error",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="48e94-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="48e94-154">Response</span></span>
<span data-ttu-id="48e94-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48e94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "77296cf7-6cf7-7729-f76c-2977f76c2977",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "error",
  "version": "Version value"
}
```




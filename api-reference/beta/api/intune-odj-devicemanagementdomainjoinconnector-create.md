---
title: Создание Девицеманажементдомаинжоинконнектор
description: Создание нового объекта Девицеманажементдомаинжоинконнектор.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 787bbde0438b9a8f8a28e42c591436cc70f1f406
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803114"
---
# <a name="create-devicemanagementdomainjoinconnector"></a><span data-ttu-id="55450-103">Создание Девицеманажементдомаинжоинконнектор</span><span class="sxs-lookup"><span data-stu-id="55450-103">Create deviceManagementDomainJoinConnector</span></span>

> <span data-ttu-id="55450-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55450-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55450-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55450-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55450-106">Создание нового объекта [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="55450-106">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55450-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="55450-107">Prerequisites</span></span>
<span data-ttu-id="55450-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55450-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55450-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55450-110">Permission type</span></span>|<span data-ttu-id="55450-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55450-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55450-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55450-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55450-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55450-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55450-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55450-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55450-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55450-115">Not supported.</span></span>|
|<span data-ttu-id="55450-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="55450-116">Application</span></span>|<span data-ttu-id="55450-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55450-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55450-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55450-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="55450-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="55450-119">Request headers</span></span>
|<span data-ttu-id="55450-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55450-120">Header</span></span>|<span data-ttu-id="55450-121">Значение</span><span class="sxs-lookup"><span data-stu-id="55450-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55450-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="55450-122">Authorization</span></span>|<span data-ttu-id="55450-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55450-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55450-124">Accept</span><span class="sxs-lookup"><span data-stu-id="55450-124">Accept</span></span>|<span data-ttu-id="55450-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55450-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55450-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55450-126">Request body</span></span>
<span data-ttu-id="55450-127">В тексте запроса добавьте представление объекта Девицеманажементдомаинжоинконнектор в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55450-127">In the request body, supply a JSON representation for the deviceManagementDomainJoinConnector object.</span></span>

<span data-ttu-id="55450-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементдомаинжоинконнектор.</span><span class="sxs-lookup"><span data-stu-id="55450-128">The following table shows the properties that are required when you create the deviceManagementDomainJoinConnector.</span></span>

|<span data-ttu-id="55450-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="55450-129">Property</span></span>|<span data-ttu-id="55450-130">Тип</span><span class="sxs-lookup"><span data-stu-id="55450-130">Type</span></span>|<span data-ttu-id="55450-131">Описание</span><span class="sxs-lookup"><span data-stu-id="55450-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55450-132">id</span><span class="sxs-lookup"><span data-stu-id="55450-132">id</span></span>|<span data-ttu-id="55450-133">String</span><span class="sxs-lookup"><span data-stu-id="55450-133">String</span></span>|<span data-ttu-id="55450-134">Уникальный идентификатор, представляющий соединитель.</span><span class="sxs-lookup"><span data-stu-id="55450-134">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="55450-135">displayName</span><span class="sxs-lookup"><span data-stu-id="55450-135">displayName</span></span>|<span data-ttu-id="55450-136">Строка</span><span class="sxs-lookup"><span data-stu-id="55450-136">String</span></span>|<span data-ttu-id="55450-137">Отображаемое имя соединителя.</span><span class="sxs-lookup"><span data-stu-id="55450-137">The connector display name.</span></span>|
|<span data-ttu-id="55450-138">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="55450-138">lastConnectionDateTime</span></span>|<span data-ttu-id="55450-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55450-139">DateTimeOffset</span></span>|<span data-ttu-id="55450-140">Последний соединитель времени с обращением к Intune.</span><span class="sxs-lookup"><span data-stu-id="55450-140">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="55450-141">state</span><span class="sxs-lookup"><span data-stu-id="55450-141">state</span></span>|[<span data-ttu-id="55450-142">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="55450-142">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="55450-143">Состояние соединителя.</span><span class="sxs-lookup"><span data-stu-id="55450-143">The connector state.</span></span> <span data-ttu-id="55450-144">Возможные значения: `active`, `error`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="55450-144">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="55450-145">version</span><span class="sxs-lookup"><span data-stu-id="55450-145">version</span></span>|<span data-ttu-id="55450-146">String</span><span class="sxs-lookup"><span data-stu-id="55450-146">String</span></span>|<span data-ttu-id="55450-147">Версия соединителя.</span><span class="sxs-lookup"><span data-stu-id="55450-147">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="55450-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="55450-148">Response</span></span>
<span data-ttu-id="55450-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55450-149">If successful, this method returns a `201 Created` response code and a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55450-150">Пример</span><span class="sxs-lookup"><span data-stu-id="55450-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="55450-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="55450-151">Request</span></span>
<span data-ttu-id="55450-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55450-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="55450-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="55450-153">Response</span></span>
<span data-ttu-id="55450-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55450-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





---
title: Обновление Девицеманажементдомаинжоинконнектор
description: Обновление свойств объекта Девицеманажементдомаинжоинконнектор.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 36443dc8702781b8429265b4e00ea510f6532e5a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941927"
---
# <a name="update-devicemanagementdomainjoinconnector"></a><span data-ttu-id="b1217-103">Обновление Девицеманажементдомаинжоинконнектор</span><span class="sxs-lookup"><span data-stu-id="b1217-103">Update deviceManagementDomainJoinConnector</span></span>

> <span data-ttu-id="b1217-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1217-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1217-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1217-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1217-106">Обновление свойств объекта [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="b1217-106">Update the properties of a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1217-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b1217-107">Prerequisites</span></span>
<span data-ttu-id="b1217-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1217-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1217-110">Permission type</span></span>|<span data-ttu-id="b1217-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1217-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1217-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1217-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1217-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1217-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1217-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1217-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1217-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1217-115">Not supported.</span></span>|
|<span data-ttu-id="b1217-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1217-116">Application</span></span>|<span data-ttu-id="b1217-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1217-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1217-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1217-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="b1217-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1217-119">Request headers</span></span>
|<span data-ttu-id="b1217-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1217-120">Header</span></span>|<span data-ttu-id="b1217-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b1217-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1217-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1217-122">Authorization</span></span>|<span data-ttu-id="b1217-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1217-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1217-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b1217-124">Accept</span></span>|<span data-ttu-id="b1217-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1217-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1217-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b1217-126">Request body</span></span>
<span data-ttu-id="b1217-127">В тексте запроса добавьте представление объекта [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1217-127">In the request body, supply a JSON representation for the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

<span data-ttu-id="b1217-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span><span class="sxs-lookup"><span data-stu-id="b1217-128">The following table shows the properties that are required when you create the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span></span>

|<span data-ttu-id="b1217-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1217-129">Property</span></span>|<span data-ttu-id="b1217-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b1217-130">Type</span></span>|<span data-ttu-id="b1217-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b1217-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1217-132">id</span><span class="sxs-lookup"><span data-stu-id="b1217-132">id</span></span>|<span data-ttu-id="b1217-133">String</span><span class="sxs-lookup"><span data-stu-id="b1217-133">String</span></span>|<span data-ttu-id="b1217-134">Уникальный идентификатор, представляющий соединитель.</span><span class="sxs-lookup"><span data-stu-id="b1217-134">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="b1217-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b1217-135">displayName</span></span>|<span data-ttu-id="b1217-136">Строка</span><span class="sxs-lookup"><span data-stu-id="b1217-136">String</span></span>|<span data-ttu-id="b1217-137">Отображаемое имя соединителя.</span><span class="sxs-lookup"><span data-stu-id="b1217-137">The connector display name.</span></span>|
|<span data-ttu-id="b1217-138">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="b1217-138">lastConnectionDateTime</span></span>|<span data-ttu-id="b1217-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1217-139">DateTimeOffset</span></span>|<span data-ttu-id="b1217-140">Последний соединитель времени с обращением к Intune.</span><span class="sxs-lookup"><span data-stu-id="b1217-140">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="b1217-141">state</span><span class="sxs-lookup"><span data-stu-id="b1217-141">state</span></span>|[<span data-ttu-id="b1217-142">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="b1217-142">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="b1217-143">Состояние соединителя.</span><span class="sxs-lookup"><span data-stu-id="b1217-143">The connector state.</span></span> <span data-ttu-id="b1217-144">Возможные значения: `active`, `error`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="b1217-144">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="b1217-145">version</span><span class="sxs-lookup"><span data-stu-id="b1217-145">version</span></span>|<span data-ttu-id="b1217-146">String</span><span class="sxs-lookup"><span data-stu-id="b1217-146">String</span></span>|<span data-ttu-id="b1217-147">Версия соединителя.</span><span class="sxs-lookup"><span data-stu-id="b1217-147">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="b1217-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1217-148">Response</span></span>
<span data-ttu-id="b1217-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1217-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1217-150">Пример</span><span class="sxs-lookup"><span data-stu-id="b1217-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1217-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1217-151">Request</span></span>
<span data-ttu-id="b1217-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1217-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
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

### <a name="response"></a><span data-ttu-id="b1217-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1217-153">Response</span></span>
<span data-ttu-id="b1217-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1217-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






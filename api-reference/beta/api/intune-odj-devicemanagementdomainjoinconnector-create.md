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
# <a name="create-devicemanagementdomainjoinconnector"></a><span data-ttu-id="dfa19-103">Создание Девицеманажементдомаинжоинконнектор</span><span class="sxs-lookup"><span data-stu-id="dfa19-103">Create deviceManagementDomainJoinConnector</span></span>

<span data-ttu-id="dfa19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfa19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dfa19-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfa19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfa19-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfa19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfa19-107">Создание нового объекта [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="dfa19-107">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfa19-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dfa19-108">Prerequisites</span></span>
<span data-ttu-id="dfa19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfa19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfa19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa19-111">Permission type</span></span>|<span data-ttu-id="dfa19-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfa19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfa19-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfa19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dfa19-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfa19-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dfa19-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfa19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfa19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfa19-116">Not supported.</span></span>|
|<span data-ttu-id="dfa19-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfa19-117">Application</span></span>|<span data-ttu-id="dfa19-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfa19-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfa19-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfa19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="dfa19-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dfa19-120">Request headers</span></span>
|<span data-ttu-id="dfa19-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dfa19-121">Header</span></span>|<span data-ttu-id="dfa19-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dfa19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfa19-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfa19-123">Authorization</span></span>|<span data-ttu-id="dfa19-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfa19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfa19-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dfa19-125">Accept</span></span>|<span data-ttu-id="dfa19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dfa19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfa19-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dfa19-127">Request body</span></span>
<span data-ttu-id="dfa19-128">В тексте запроса добавьте представление объекта Девицеманажементдомаинжоинконнектор в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfa19-128">In the request body, supply a JSON representation for the deviceManagementDomainJoinConnector object.</span></span>

<span data-ttu-id="dfa19-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементдомаинжоинконнектор.</span><span class="sxs-lookup"><span data-stu-id="dfa19-129">The following table shows the properties that are required when you create the deviceManagementDomainJoinConnector.</span></span>

|<span data-ttu-id="dfa19-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfa19-130">Property</span></span>|<span data-ttu-id="dfa19-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dfa19-131">Type</span></span>|<span data-ttu-id="dfa19-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dfa19-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfa19-133">id</span><span class="sxs-lookup"><span data-stu-id="dfa19-133">id</span></span>|<span data-ttu-id="dfa19-134">String</span><span class="sxs-lookup"><span data-stu-id="dfa19-134">String</span></span>|<span data-ttu-id="dfa19-135">Уникальный идентификатор, представляющий соединитель.</span><span class="sxs-lookup"><span data-stu-id="dfa19-135">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="dfa19-136">displayName</span><span class="sxs-lookup"><span data-stu-id="dfa19-136">displayName</span></span>|<span data-ttu-id="dfa19-137">Строка</span><span class="sxs-lookup"><span data-stu-id="dfa19-137">String</span></span>|<span data-ttu-id="dfa19-138">Отображаемое имя соединителя.</span><span class="sxs-lookup"><span data-stu-id="dfa19-138">The connector display name.</span></span>|
|<span data-ttu-id="dfa19-139">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="dfa19-139">lastConnectionDateTime</span></span>|<span data-ttu-id="dfa19-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfa19-140">DateTimeOffset</span></span>|<span data-ttu-id="dfa19-141">Последний соединитель времени с обращением к Intune.</span><span class="sxs-lookup"><span data-stu-id="dfa19-141">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="dfa19-142">state</span><span class="sxs-lookup"><span data-stu-id="dfa19-142">state</span></span>|[<span data-ttu-id="dfa19-143">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="dfa19-143">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="dfa19-144">Состояние соединителя.</span><span class="sxs-lookup"><span data-stu-id="dfa19-144">The connector state.</span></span> <span data-ttu-id="dfa19-145">Возможные значения: `active`, `error`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="dfa19-145">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="dfa19-146">version</span><span class="sxs-lookup"><span data-stu-id="dfa19-146">version</span></span>|<span data-ttu-id="dfa19-147">String</span><span class="sxs-lookup"><span data-stu-id="dfa19-147">String</span></span>|<span data-ttu-id="dfa19-148">Версия соединителя.</span><span class="sxs-lookup"><span data-stu-id="dfa19-148">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="dfa19-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfa19-149">Response</span></span>
<span data-ttu-id="dfa19-150">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa19-150">If successful, this method returns a `201 Created` response code and a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfa19-151">Пример</span><span class="sxs-lookup"><span data-stu-id="dfa19-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfa19-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfa19-152">Request</span></span>
<span data-ttu-id="dfa19-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfa19-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dfa19-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa19-154">Response</span></span>
<span data-ttu-id="dfa19-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfa19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




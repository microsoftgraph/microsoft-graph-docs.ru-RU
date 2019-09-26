---
title: Создание Девицеманажементдомаинжоинконнектор
description: Создание нового объекта Девицеманажементдомаинжоинконнектор.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 178d43f041058f4380c7b179d56d7f91d1923a6a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191101"
---
# <a name="create-devicemanagementdomainjoinconnector"></a><span data-ttu-id="5380d-103">Создание Девицеманажементдомаинжоинконнектор</span><span class="sxs-lookup"><span data-stu-id="5380d-103">Create deviceManagementDomainJoinConnector</span></span>

> <span data-ttu-id="5380d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5380d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5380d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5380d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5380d-106">Создание нового объекта [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="5380d-106">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5380d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5380d-107">Prerequisites</span></span>
<span data-ttu-id="5380d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5380d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5380d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5380d-110">Permission type</span></span>|<span data-ttu-id="5380d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5380d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5380d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5380d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5380d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5380d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5380d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5380d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5380d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5380d-115">Not supported.</span></span>|
|<span data-ttu-id="5380d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5380d-116">Application</span></span>|<span data-ttu-id="5380d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5380d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5380d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5380d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="5380d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5380d-119">Request headers</span></span>
|<span data-ttu-id="5380d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5380d-120">Header</span></span>|<span data-ttu-id="5380d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5380d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5380d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5380d-122">Authorization</span></span>|<span data-ttu-id="5380d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5380d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5380d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5380d-124">Accept</span></span>|<span data-ttu-id="5380d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5380d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5380d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5380d-126">Request body</span></span>
<span data-ttu-id="5380d-127">В тексте запроса добавьте представление объекта Девицеманажементдомаинжоинконнектор в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5380d-127">In the request body, supply a JSON representation for the deviceManagementDomainJoinConnector object.</span></span>

<span data-ttu-id="5380d-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементдомаинжоинконнектор.</span><span class="sxs-lookup"><span data-stu-id="5380d-128">The following table shows the properties that are required when you create the deviceManagementDomainJoinConnector.</span></span>

|<span data-ttu-id="5380d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5380d-129">Property</span></span>|<span data-ttu-id="5380d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5380d-130">Type</span></span>|<span data-ttu-id="5380d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5380d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5380d-132">id</span><span class="sxs-lookup"><span data-stu-id="5380d-132">id</span></span>|<span data-ttu-id="5380d-133">String</span><span class="sxs-lookup"><span data-stu-id="5380d-133">String</span></span>|<span data-ttu-id="5380d-134">Уникальный идентификатор, представляющий соединитель.</span><span class="sxs-lookup"><span data-stu-id="5380d-134">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="5380d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5380d-135">displayName</span></span>|<span data-ttu-id="5380d-136">Строка</span><span class="sxs-lookup"><span data-stu-id="5380d-136">String</span></span>|<span data-ttu-id="5380d-137">Отображаемое имя соединителя.</span><span class="sxs-lookup"><span data-stu-id="5380d-137">The connector display name.</span></span>|
|<span data-ttu-id="5380d-138">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="5380d-138">lastConnectionDateTime</span></span>|<span data-ttu-id="5380d-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5380d-139">DateTimeOffset</span></span>|<span data-ttu-id="5380d-140">Последний соединитель времени с обращением к Intune.</span><span class="sxs-lookup"><span data-stu-id="5380d-140">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="5380d-141">состояние</span><span class="sxs-lookup"><span data-stu-id="5380d-141">state</span></span>|[<span data-ttu-id="5380d-142">девицеманажементдомаинжоинконнекторстате</span><span class="sxs-lookup"><span data-stu-id="5380d-142">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="5380d-143">Состояние соединителя.</span><span class="sxs-lookup"><span data-stu-id="5380d-143">The connector state.</span></span> <span data-ttu-id="5380d-144">Возможные значения: `active`, `error`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="5380d-144">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="5380d-145">version</span><span class="sxs-lookup"><span data-stu-id="5380d-145">version</span></span>|<span data-ttu-id="5380d-146">String</span><span class="sxs-lookup"><span data-stu-id="5380d-146">String</span></span>|<span data-ttu-id="5380d-147">Версия соединителя.</span><span class="sxs-lookup"><span data-stu-id="5380d-147">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="5380d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5380d-148">Response</span></span>
<span data-ttu-id="5380d-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5380d-149">If successful, this method returns a `201 Created` response code and a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5380d-150">Пример</span><span class="sxs-lookup"><span data-stu-id="5380d-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="5380d-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="5380d-151">Request</span></span>
<span data-ttu-id="5380d-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5380d-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5380d-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="5380d-153">Response</span></span>
<span data-ttu-id="5380d-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5380d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





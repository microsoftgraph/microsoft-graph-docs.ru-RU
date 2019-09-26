---
title: Обновление Ндесконнектор
description: Обновление свойств объекта Ндесконнектор.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 052e9093bc1e29a7b988aef39546ad6d8ef39b23
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37183473"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="ec27c-103">Обновление Ндесконнектор</span><span class="sxs-lookup"><span data-stu-id="ec27c-103">Update ndesConnector</span></span>

> <span data-ttu-id="ec27c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec27c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec27c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec27c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec27c-106">Обновление свойств объекта [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="ec27c-106">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec27c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ec27c-107">Prerequisites</span></span>
<span data-ttu-id="ec27c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec27c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec27c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec27c-110">Permission type</span></span>|<span data-ttu-id="ec27c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec27c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec27c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec27c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec27c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec27c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ec27c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec27c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec27c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec27c-115">Not supported.</span></span>|
|<span data-ttu-id="ec27c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec27c-116">Application</span></span>|<span data-ttu-id="ec27c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec27c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec27c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec27c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="ec27c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec27c-119">Request headers</span></span>
|<span data-ttu-id="ec27c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec27c-120">Header</span></span>|<span data-ttu-id="ec27c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ec27c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec27c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec27c-122">Authorization</span></span>|<span data-ttu-id="ec27c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec27c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec27c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ec27c-124">Accept</span></span>|<span data-ttu-id="ec27c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ec27c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec27c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ec27c-126">Request body</span></span>
<span data-ttu-id="ec27c-127">В тексте запроса добавьте представление объекта [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec27c-127">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="ec27c-128">В следующей таблице приведены свойства, необходимые при создании [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md).</span><span class="sxs-lookup"><span data-stu-id="ec27c-128">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="ec27c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec27c-129">Property</span></span>|<span data-ttu-id="ec27c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ec27c-130">Type</span></span>|<span data-ttu-id="ec27c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ec27c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec27c-132">id</span><span class="sxs-lookup"><span data-stu-id="ec27c-132">id</span></span>|<span data-ttu-id="ec27c-133">String</span><span class="sxs-lookup"><span data-stu-id="ec27c-133">String</span></span>|<span data-ttu-id="ec27c-134">Ключ соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="ec27c-134">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="ec27c-135">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="ec27c-135">lastConnectionDateTime</span></span>|<span data-ttu-id="ec27c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec27c-136">DateTimeOffset</span></span>|<span data-ttu-id="ec27c-137">Время последнего подключения для соединителя NDES Connector</span><span class="sxs-lookup"><span data-stu-id="ec27c-137">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="ec27c-138">состояние</span><span class="sxs-lookup"><span data-stu-id="ec27c-138">state</span></span>|[<span data-ttu-id="ec27c-139">ндесконнекторстате</span><span class="sxs-lookup"><span data-stu-id="ec27c-139">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="ec27c-140">Состояние соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="ec27c-140">Ndes Connector Status.</span></span> <span data-ttu-id="ec27c-141">Возможные значения: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="ec27c-141">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="ec27c-142">displayName</span><span class="sxs-lookup"><span data-stu-id="ec27c-142">displayName</span></span>|<span data-ttu-id="ec27c-143">Строка</span><span class="sxs-lookup"><span data-stu-id="ec27c-143">String</span></span>|<span data-ttu-id="ec27c-144">Понятное имя соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="ec27c-144">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="ec27c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec27c-145">Response</span></span>
<span data-ttu-id="ec27c-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec27c-146">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec27c-147">Пример</span><span class="sxs-lookup"><span data-stu-id="ec27c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec27c-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec27c-148">Request</span></span>
<span data-ttu-id="ec27c-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec27c-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="ec27c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec27c-150">Response</span></span>
<span data-ttu-id="ec27c-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec27c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```





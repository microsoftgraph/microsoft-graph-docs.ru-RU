---
title: Обновление Ндесконнектор
description: Обновление свойств объекта Ндесконнектор.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef715625dbcd8779280ac2165b25dc2b8edda34d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49270934"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="b53df-103">Обновление Ндесконнектор</span><span class="sxs-lookup"><span data-stu-id="b53df-103">Update ndesConnector</span></span>

<span data-ttu-id="b53df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b53df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b53df-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b53df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b53df-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b53df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b53df-107">Обновление свойств объекта [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="b53df-107">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b53df-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b53df-108">Prerequisites</span></span>
<span data-ttu-id="b53df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b53df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b53df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b53df-111">Permission type</span></span>|<span data-ttu-id="b53df-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b53df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b53df-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b53df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b53df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b53df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b53df-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b53df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b53df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b53df-116">Not supported.</span></span>|
|<span data-ttu-id="b53df-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b53df-117">Application</span></span>|<span data-ttu-id="b53df-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b53df-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b53df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b53df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="b53df-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b53df-120">Request headers</span></span>
|<span data-ttu-id="b53df-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b53df-121">Header</span></span>|<span data-ttu-id="b53df-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b53df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b53df-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b53df-123">Authorization</span></span>|<span data-ttu-id="b53df-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b53df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b53df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b53df-125">Accept</span></span>|<span data-ttu-id="b53df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b53df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b53df-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b53df-127">Request body</span></span>
<span data-ttu-id="b53df-128">В тексте запроса добавьте представление объекта [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b53df-128">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="b53df-129">В следующей таблице приведены свойства, необходимые при создании [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md).</span><span class="sxs-lookup"><span data-stu-id="b53df-129">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="b53df-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b53df-130">Property</span></span>|<span data-ttu-id="b53df-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b53df-131">Type</span></span>|<span data-ttu-id="b53df-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b53df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b53df-133">id</span><span class="sxs-lookup"><span data-stu-id="b53df-133">id</span></span>|<span data-ttu-id="b53df-134">String</span><span class="sxs-lookup"><span data-stu-id="b53df-134">String</span></span>|<span data-ttu-id="b53df-135">Ключ соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="b53df-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="b53df-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="b53df-136">lastConnectionDateTime</span></span>|<span data-ttu-id="b53df-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b53df-137">DateTimeOffset</span></span>|<span data-ttu-id="b53df-138">Время последнего подключения для соединителя NDES Connector</span><span class="sxs-lookup"><span data-stu-id="b53df-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="b53df-139">state</span><span class="sxs-lookup"><span data-stu-id="b53df-139">state</span></span>|[<span data-ttu-id="b53df-140">ндесконнекторстате</span><span class="sxs-lookup"><span data-stu-id="b53df-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="b53df-141">Состояние соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="b53df-141">Ndes Connector Status.</span></span> <span data-ttu-id="b53df-142">Возможные значения: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="b53df-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="b53df-143">displayName</span><span class="sxs-lookup"><span data-stu-id="b53df-143">displayName</span></span>|<span data-ttu-id="b53df-144">String</span><span class="sxs-lookup"><span data-stu-id="b53df-144">String</span></span>|<span data-ttu-id="b53df-145">Понятное имя соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="b53df-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="b53df-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b53df-146">Response</span></span>
<span data-ttu-id="b53df-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b53df-147">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b53df-148">Пример</span><span class="sxs-lookup"><span data-stu-id="b53df-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="b53df-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="b53df-149">Request</span></span>
<span data-ttu-id="b53df-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b53df-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b53df-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="b53df-151">Response</span></span>
<span data-ttu-id="b53df-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b53df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





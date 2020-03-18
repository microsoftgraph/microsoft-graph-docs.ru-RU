---
title: Создание Ндесконнектор
description: Создание нового объекта Ндесконнектор.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e1090796b86e991f2581f185cbaaca3eba6e96ae
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42742864"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="63719-103">Создание Ндесконнектор</span><span class="sxs-lookup"><span data-stu-id="63719-103">Create ndesConnector</span></span>

> <span data-ttu-id="63719-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63719-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63719-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63719-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63719-106">Создание нового объекта [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="63719-106">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63719-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="63719-107">Prerequisites</span></span>
<span data-ttu-id="63719-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63719-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63719-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63719-110">Permission type</span></span>|<span data-ttu-id="63719-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63719-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63719-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63719-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63719-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63719-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63719-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63719-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63719-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63719-115">Not supported.</span></span>|
|<span data-ttu-id="63719-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="63719-116">Application</span></span>|<span data-ttu-id="63719-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63719-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63719-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63719-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="63719-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="63719-119">Request headers</span></span>
|<span data-ttu-id="63719-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63719-120">Header</span></span>|<span data-ttu-id="63719-121">Значение</span><span class="sxs-lookup"><span data-stu-id="63719-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63719-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="63719-122">Authorization</span></span>|<span data-ttu-id="63719-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63719-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63719-124">Accept</span><span class="sxs-lookup"><span data-stu-id="63719-124">Accept</span></span>|<span data-ttu-id="63719-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63719-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63719-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63719-126">Request body</span></span>
<span data-ttu-id="63719-127">В тексте запроса добавьте представление объекта Ндесконнектор в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63719-127">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="63719-128">В следующей таблице приведены свойства, необходимые при создании Ндесконнектор.</span><span class="sxs-lookup"><span data-stu-id="63719-128">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="63719-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="63719-129">Property</span></span>|<span data-ttu-id="63719-130">Тип</span><span class="sxs-lookup"><span data-stu-id="63719-130">Type</span></span>|<span data-ttu-id="63719-131">Описание</span><span class="sxs-lookup"><span data-stu-id="63719-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63719-132">id</span><span class="sxs-lookup"><span data-stu-id="63719-132">id</span></span>|<span data-ttu-id="63719-133">String</span><span class="sxs-lookup"><span data-stu-id="63719-133">String</span></span>|<span data-ttu-id="63719-134">Ключ соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="63719-134">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="63719-135">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="63719-135">lastConnectionDateTime</span></span>|<span data-ttu-id="63719-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63719-136">DateTimeOffset</span></span>|<span data-ttu-id="63719-137">Время последнего подключения для соединителя NDES Connector</span><span class="sxs-lookup"><span data-stu-id="63719-137">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="63719-138">state</span><span class="sxs-lookup"><span data-stu-id="63719-138">state</span></span>|[<span data-ttu-id="63719-139">ндесконнекторстате</span><span class="sxs-lookup"><span data-stu-id="63719-139">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="63719-140">Состояние соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="63719-140">Ndes Connector Status.</span></span> <span data-ttu-id="63719-141">Возможные значения: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="63719-141">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="63719-142">displayName</span><span class="sxs-lookup"><span data-stu-id="63719-142">displayName</span></span>|<span data-ttu-id="63719-143">Строка</span><span class="sxs-lookup"><span data-stu-id="63719-143">String</span></span>|<span data-ttu-id="63719-144">Понятное имя соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="63719-144">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="63719-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="63719-145">Response</span></span>
<span data-ttu-id="63719-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63719-146">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63719-147">Пример</span><span class="sxs-lookup"><span data-stu-id="63719-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="63719-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="63719-148">Request</span></span>
<span data-ttu-id="63719-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63719-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="63719-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="63719-150">Response</span></span>
<span data-ttu-id="63719-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63719-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





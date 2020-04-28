---
title: Создание Ндесконнектор
description: Создание нового объекта Ндесконнектор.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df9dce7a6157ae652cc99d5ac57df34db2c8cce6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43342937"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="b242e-103">Создание Ндесконнектор</span><span class="sxs-lookup"><span data-stu-id="b242e-103">Create ndesConnector</span></span>

<span data-ttu-id="b242e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b242e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b242e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b242e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b242e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b242e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b242e-107">Создание нового объекта [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="b242e-107">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b242e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b242e-108">Prerequisites</span></span>
<span data-ttu-id="b242e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b242e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b242e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b242e-111">Permission type</span></span>|<span data-ttu-id="b242e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b242e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b242e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b242e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b242e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b242e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b242e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b242e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b242e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b242e-116">Not supported.</span></span>|
|<span data-ttu-id="b242e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b242e-117">Application</span></span>|<span data-ttu-id="b242e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b242e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b242e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b242e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="b242e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b242e-120">Request headers</span></span>
|<span data-ttu-id="b242e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b242e-121">Header</span></span>|<span data-ttu-id="b242e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b242e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b242e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b242e-123">Authorization</span></span>|<span data-ttu-id="b242e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b242e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b242e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b242e-125">Accept</span></span>|<span data-ttu-id="b242e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b242e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b242e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b242e-127">Request body</span></span>
<span data-ttu-id="b242e-128">В тексте запроса добавьте представление объекта Ндесконнектор в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b242e-128">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="b242e-129">В следующей таблице приведены свойства, необходимые при создании Ндесконнектор.</span><span class="sxs-lookup"><span data-stu-id="b242e-129">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="b242e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b242e-130">Property</span></span>|<span data-ttu-id="b242e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b242e-131">Type</span></span>|<span data-ttu-id="b242e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b242e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b242e-133">id</span><span class="sxs-lookup"><span data-stu-id="b242e-133">id</span></span>|<span data-ttu-id="b242e-134">String</span><span class="sxs-lookup"><span data-stu-id="b242e-134">String</span></span>|<span data-ttu-id="b242e-135">Ключ соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="b242e-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="b242e-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="b242e-136">lastConnectionDateTime</span></span>|<span data-ttu-id="b242e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b242e-137">DateTimeOffset</span></span>|<span data-ttu-id="b242e-138">Время последнего подключения для соединителя NDES Connector</span><span class="sxs-lookup"><span data-stu-id="b242e-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="b242e-139">state</span><span class="sxs-lookup"><span data-stu-id="b242e-139">state</span></span>|[<span data-ttu-id="b242e-140">ндесконнекторстате</span><span class="sxs-lookup"><span data-stu-id="b242e-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="b242e-141">Состояние соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="b242e-141">Ndes Connector Status.</span></span> <span data-ttu-id="b242e-142">Возможные значения: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="b242e-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="b242e-143">displayName</span><span class="sxs-lookup"><span data-stu-id="b242e-143">displayName</span></span>|<span data-ttu-id="b242e-144">Строка</span><span class="sxs-lookup"><span data-stu-id="b242e-144">String</span></span>|<span data-ttu-id="b242e-145">Понятное имя соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="b242e-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="b242e-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="b242e-146">Response</span></span>
<span data-ttu-id="b242e-147">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b242e-147">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b242e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="b242e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="b242e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="b242e-149">Request</span></span>
<span data-ttu-id="b242e-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b242e-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b242e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="b242e-151">Response</span></span>
<span data-ttu-id="b242e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b242e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




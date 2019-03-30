---
title: Создание Ндесконнектор
description: Создание нового объекта Ндесконнектор.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33d3d832df9e14692316b9b12132c531a2b610d3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986182"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="43130-103">Создание Ндесконнектор</span><span class="sxs-lookup"><span data-stu-id="43130-103">Create ndesConnector</span></span>

> <span data-ttu-id="43130-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43130-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43130-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43130-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43130-106">Создание нового объекта [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="43130-106">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43130-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="43130-107">Prerequisites</span></span>
<span data-ttu-id="43130-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43130-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43130-110">Permission type</span></span>|<span data-ttu-id="43130-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43130-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43130-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43130-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43130-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43130-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43130-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43130-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43130-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43130-115">Not supported.</span></span>|
|<span data-ttu-id="43130-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43130-116">Application</span></span>|<span data-ttu-id="43130-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43130-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43130-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43130-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="43130-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43130-119">Request headers</span></span>
|<span data-ttu-id="43130-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43130-120">Header</span></span>|<span data-ttu-id="43130-121">Значение</span><span class="sxs-lookup"><span data-stu-id="43130-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43130-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43130-122">Authorization</span></span>|<span data-ttu-id="43130-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43130-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43130-124">Accept</span><span class="sxs-lookup"><span data-stu-id="43130-124">Accept</span></span>|<span data-ttu-id="43130-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43130-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43130-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43130-126">Request body</span></span>
<span data-ttu-id="43130-127">В тексте запроса добавьте представление объекта Ндесконнектор в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43130-127">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="43130-128">В следующей таблице приведены свойства, необходимые при создании Ндесконнектор.</span><span class="sxs-lookup"><span data-stu-id="43130-128">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="43130-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="43130-129">Property</span></span>|<span data-ttu-id="43130-130">Тип</span><span class="sxs-lookup"><span data-stu-id="43130-130">Type</span></span>|<span data-ttu-id="43130-131">Описание</span><span class="sxs-lookup"><span data-stu-id="43130-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43130-132">id</span><span class="sxs-lookup"><span data-stu-id="43130-132">id</span></span>|<span data-ttu-id="43130-133">String</span><span class="sxs-lookup"><span data-stu-id="43130-133">String</span></span>|<span data-ttu-id="43130-134">Ключ соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="43130-134">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="43130-135">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="43130-135">lastConnectionDateTime</span></span>|<span data-ttu-id="43130-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43130-136">DateTimeOffset</span></span>|<span data-ttu-id="43130-137">Время последнего подключения для соединителя NDES Connector</span><span class="sxs-lookup"><span data-stu-id="43130-137">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="43130-138">state</span><span class="sxs-lookup"><span data-stu-id="43130-138">state</span></span>|[<span data-ttu-id="43130-139">Ндесконнекторстате</span><span class="sxs-lookup"><span data-stu-id="43130-139">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="43130-140">Состояние соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="43130-140">Ndes Connector Status.</span></span> <span data-ttu-id="43130-141">Возможные значения: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="43130-141">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="43130-142">displayName</span><span class="sxs-lookup"><span data-stu-id="43130-142">displayName</span></span>|<span data-ttu-id="43130-143">String</span><span class="sxs-lookup"><span data-stu-id="43130-143">String</span></span>|<span data-ttu-id="43130-144">Понятное имя соединителя NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="43130-144">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="43130-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="43130-145">Response</span></span>
<span data-ttu-id="43130-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43130-146">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43130-147">Пример</span><span class="sxs-lookup"><span data-stu-id="43130-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="43130-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="43130-148">Request</span></span>
<span data-ttu-id="43130-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43130-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43130-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="43130-150">Response</span></span>
<span data-ttu-id="43130-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43130-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





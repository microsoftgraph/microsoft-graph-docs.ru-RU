---
title: Обновление ndesConnector
description: Обновление свойств объекта ndesConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c7bb14b89b4474b5196ee563e03d7e7419b0c40
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155073"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="ba3f2-103">Обновление ndesConnector</span><span class="sxs-lookup"><span data-stu-id="ba3f2-103">Update ndesConnector</span></span>

<span data-ttu-id="ba3f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba3f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba3f2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba3f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba3f2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba3f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba3f2-107">Обновление свойств объекта [ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)</span><span class="sxs-lookup"><span data-stu-id="ba3f2-107">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba3f2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ba3f2-108">Prerequisites</span></span>
<span data-ttu-id="ba3f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba3f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba3f2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba3f2-111">Permission type</span></span>|<span data-ttu-id="ba3f2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba3f2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba3f2-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba3f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba3f2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba3f2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba3f2-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba3f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba3f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba3f2-116">Not supported.</span></span>|
|<span data-ttu-id="ba3f2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ba3f2-117">Application</span></span>|<span data-ttu-id="ba3f2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba3f2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba3f2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba3f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="ba3f2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ba3f2-120">Request headers</span></span>
|<span data-ttu-id="ba3f2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba3f2-121">Header</span></span>|<span data-ttu-id="ba3f2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ba3f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba3f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba3f2-123">Authorization</span></span>|<span data-ttu-id="ba3f2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba3f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba3f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ba3f2-125">Accept</span></span>|<span data-ttu-id="ba3f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba3f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba3f2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba3f2-127">Request body</span></span>
<span data-ttu-id="ba3f2-128">В теле запроса поставляем представление JSON для объекта [ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)</span><span class="sxs-lookup"><span data-stu-id="ba3f2-128">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="ba3f2-129">В следующей таблице показаны свойства, необходимые при создании [ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)</span><span class="sxs-lookup"><span data-stu-id="ba3f2-129">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="ba3f2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba3f2-130">Property</span></span>|<span data-ttu-id="ba3f2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ba3f2-131">Type</span></span>|<span data-ttu-id="ba3f2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ba3f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba3f2-133">id</span><span class="sxs-lookup"><span data-stu-id="ba3f2-133">id</span></span>|<span data-ttu-id="ba3f2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ba3f2-134">String</span></span>|<span data-ttu-id="ba3f2-135">Ключ соединиттеля NDES.</span><span class="sxs-lookup"><span data-stu-id="ba3f2-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="ba3f2-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="ba3f2-136">lastConnectionDateTime</span></span>|<span data-ttu-id="ba3f2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba3f2-137">DateTimeOffset</span></span>|<span data-ttu-id="ba3f2-138">Последнее время подключения для соединитетеля Ndes</span><span class="sxs-lookup"><span data-stu-id="ba3f2-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="ba3f2-139">state</span><span class="sxs-lookup"><span data-stu-id="ba3f2-139">state</span></span>|[<span data-ttu-id="ba3f2-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="ba3f2-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="ba3f2-141">Состояние соединитетеля Ndes.</span><span class="sxs-lookup"><span data-stu-id="ba3f2-141">Ndes Connector Status.</span></span> <span data-ttu-id="ba3f2-142">Возможные значения: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="ba3f2-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="ba3f2-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ba3f2-143">displayName</span></span>|<span data-ttu-id="ba3f2-144">Строка</span><span class="sxs-lookup"><span data-stu-id="ba3f2-144">String</span></span>|<span data-ttu-id="ba3f2-145">Дружеское имя соединиттеля Ndes.</span><span class="sxs-lookup"><span data-stu-id="ba3f2-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="ba3f2-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba3f2-146">Response</span></span>
<span data-ttu-id="ba3f2-147">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ba3f2-147">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba3f2-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ba3f2-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba3f2-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba3f2-149">Request</span></span>
<span data-ttu-id="ba3f2-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba3f2-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ba3f2-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba3f2-151">Response</span></span>
<span data-ttu-id="ba3f2-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba3f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





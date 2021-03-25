---
title: Обновление deviceManagementDomainJoinConnector
description: Обновление свойств объекта deviceManagementDomainJoinConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3507f878ce94950c702ad61ca377aa7aaafb1c2d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152742"
---
# <a name="update-devicemanagementdomainjoinconnector"></a><span data-ttu-id="50e97-103">Обновление deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="50e97-103">Update deviceManagementDomainJoinConnector</span></span>

<span data-ttu-id="50e97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50e97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50e97-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50e97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50e97-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50e97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50e97-107">Обновление свойств объекта [deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)</span><span class="sxs-lookup"><span data-stu-id="50e97-107">Update the properties of a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50e97-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="50e97-108">Prerequisites</span></span>
<span data-ttu-id="50e97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50e97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50e97-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50e97-111">Permission type</span></span>|<span data-ttu-id="50e97-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50e97-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50e97-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50e97-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50e97-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50e97-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50e97-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50e97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50e97-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50e97-116">Not supported.</span></span>|
|<span data-ttu-id="50e97-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="50e97-117">Application</span></span>|<span data-ttu-id="50e97-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50e97-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50e97-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50e97-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="50e97-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="50e97-120">Request headers</span></span>
|<span data-ttu-id="50e97-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50e97-121">Header</span></span>|<span data-ttu-id="50e97-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50e97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50e97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50e97-123">Authorization</span></span>|<span data-ttu-id="50e97-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50e97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50e97-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50e97-125">Accept</span></span>|<span data-ttu-id="50e97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50e97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50e97-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50e97-127">Request body</span></span>
<span data-ttu-id="50e97-128">В теле запроса поставляем представление JSON для [объекта deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)</span><span class="sxs-lookup"><span data-stu-id="50e97-128">In the request body, supply a JSON representation for the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

<span data-ttu-id="50e97-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)</span><span class="sxs-lookup"><span data-stu-id="50e97-129">The following table shows the properties that are required when you create the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span></span>

|<span data-ttu-id="50e97-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="50e97-130">Property</span></span>|<span data-ttu-id="50e97-131">Тип</span><span class="sxs-lookup"><span data-stu-id="50e97-131">Type</span></span>|<span data-ttu-id="50e97-132">Описание</span><span class="sxs-lookup"><span data-stu-id="50e97-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50e97-133">id</span><span class="sxs-lookup"><span data-stu-id="50e97-133">id</span></span>|<span data-ttu-id="50e97-134">Строка</span><span class="sxs-lookup"><span data-stu-id="50e97-134">String</span></span>|<span data-ttu-id="50e97-135">Уникальный идентификатор для представления соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="50e97-135">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="50e97-136">displayName</span><span class="sxs-lookup"><span data-stu-id="50e97-136">displayName</span></span>|<span data-ttu-id="50e97-137">Строка</span><span class="sxs-lookup"><span data-stu-id="50e97-137">String</span></span>|<span data-ttu-id="50e97-138">Имя отображения соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="50e97-138">The connector display name.</span></span>|
|<span data-ttu-id="50e97-139">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="50e97-139">lastConnectionDateTime</span></span>|<span data-ttu-id="50e97-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50e97-140">DateTimeOffset</span></span>|<span data-ttu-id="50e97-141">Последний раз соединитель связывался с Intune.</span><span class="sxs-lookup"><span data-stu-id="50e97-141">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="50e97-142">state</span><span class="sxs-lookup"><span data-stu-id="50e97-142">state</span></span>|[<span data-ttu-id="50e97-143">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="50e97-143">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="50e97-144">Состояние соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="50e97-144">The connector state.</span></span> <span data-ttu-id="50e97-145">Возможные значения: `active`, `error`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="50e97-145">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="50e97-146">version</span><span class="sxs-lookup"><span data-stu-id="50e97-146">version</span></span>|<span data-ttu-id="50e97-147">String</span><span class="sxs-lookup"><span data-stu-id="50e97-147">String</span></span>|<span data-ttu-id="50e97-148">Версия соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="50e97-148">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="50e97-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="50e97-149">Response</span></span>
<span data-ttu-id="50e97-150">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="50e97-150">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50e97-151">Пример</span><span class="sxs-lookup"><span data-stu-id="50e97-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="50e97-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="50e97-152">Request</span></span>
<span data-ttu-id="50e97-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50e97-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="50e97-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="50e97-154">Response</span></span>
<span data-ttu-id="50e97-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50e97-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





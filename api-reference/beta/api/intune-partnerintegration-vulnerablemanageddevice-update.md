---
title: Обновление Вулнераблеманажеддевице
description: Обновление свойств объекта Вулнераблеманажеддевице.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a93ef4060f11b8478055efebda2a116d0c87645d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692893"
---
# <a name="update-vulnerablemanageddevice"></a><span data-ttu-id="f02e0-103">Обновление Вулнераблеманажеддевице</span><span class="sxs-lookup"><span data-stu-id="f02e0-103">Update vulnerableManagedDevice</span></span>

<span data-ttu-id="f02e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f02e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f02e0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f02e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f02e0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f02e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f02e0-107">Обновление свойств объекта [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="f02e0-107">Update the properties of a [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f02e0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f02e0-108">Prerequisites</span></span>
<span data-ttu-id="f02e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f02e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f02e0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f02e0-111">Permission type</span></span>|<span data-ttu-id="f02e0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f02e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f02e0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f02e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f02e0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f02e0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f02e0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f02e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f02e0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f02e0-116">Not supported.</span></span>|
|<span data-ttu-id="f02e0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f02e0-117">Application</span></span>|<span data-ttu-id="f02e0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f02e0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f02e0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f02e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="f02e0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f02e0-120">Request headers</span></span>
|<span data-ttu-id="f02e0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f02e0-121">Header</span></span>|<span data-ttu-id="f02e0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f02e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f02e0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f02e0-123">Authorization</span></span>|<span data-ttu-id="f02e0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f02e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f02e0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f02e0-125">Accept</span></span>|<span data-ttu-id="f02e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f02e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f02e0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f02e0-127">Request body</span></span>
<span data-ttu-id="f02e0-128">В тексте запроса добавьте представление объекта [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f02e0-128">In the request body, supply a JSON representation for the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

<span data-ttu-id="f02e0-129">В следующей таблице приведены свойства, необходимые при создании [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f02e0-129">The following table shows the properties that are required when you create the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md).</span></span>

|<span data-ttu-id="f02e0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f02e0-130">Property</span></span>|<span data-ttu-id="f02e0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f02e0-131">Type</span></span>|<span data-ttu-id="f02e0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f02e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f02e0-133">id</span><span class="sxs-lookup"><span data-stu-id="f02e0-133">id</span></span>|<span data-ttu-id="f02e0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f02e0-134">String</span></span>|<span data-ttu-id="f02e0-135">Ключ сущности и идентификатор устройства AAD.</span><span class="sxs-lookup"><span data-stu-id="f02e0-135">The entity key, and AAD device ID.</span></span>|
|<span data-ttu-id="f02e0-136">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="f02e0-136">managedDeviceId</span></span>|<span data-ttu-id="f02e0-137">Строка</span><span class="sxs-lookup"><span data-stu-id="f02e0-137">String</span></span>|<span data-ttu-id="f02e0-138">Идентификатор управляемого устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="f02e0-138">The Intune managed device ID.</span></span>|
|<span data-ttu-id="f02e0-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f02e0-139">displayName</span></span>|<span data-ttu-id="f02e0-140">Строка</span><span class="sxs-lookup"><span data-stu-id="f02e0-140">String</span></span>|<span data-ttu-id="f02e0-141">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="f02e0-141">The device name.</span></span>|
|<span data-ttu-id="f02e0-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f02e0-142">lastSyncDateTime</span></span>|<span data-ttu-id="f02e0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f02e0-143">DateTimeOffset</span></span>|<span data-ttu-id="f02e0-144">Дата последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f02e0-144">The last sync date.</span></span>|



## <a name="response"></a><span data-ttu-id="f02e0-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="f02e0-145">Response</span></span>
<span data-ttu-id="f02e0-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f02e0-146">If successful, this method returns a `200 OK` response code and an updated [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f02e0-147">Пример</span><span class="sxs-lookup"><span data-stu-id="f02e0-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="f02e0-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="f02e0-148">Request</span></span>
<span data-ttu-id="f02e0-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f02e0-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta** Entity URI for microsoft.management.services.api.vulnerableManagedDevice not found
Content-type: application/json
Content-length: 214

{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a><span data-ttu-id="f02e0-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f02e0-150">Response</span></span>
<span data-ttu-id="f02e0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f02e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "id": "e59891d4-91d4-e598-d491-98e5d49198e5",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```






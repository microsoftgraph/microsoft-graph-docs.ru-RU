---
title: Обновление vulnerableManagedDevice
description: Обновление свойств уязвимого объектаManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f054105fcbea0c4d6c9d5ae0411341702d46520
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158747"
---
# <a name="update-vulnerablemanageddevice"></a><span data-ttu-id="76acf-103">Обновление vulnerableManagedDevice</span><span class="sxs-lookup"><span data-stu-id="76acf-103">Update vulnerableManagedDevice</span></span>

<span data-ttu-id="76acf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76acf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76acf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76acf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76acf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76acf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76acf-107">Обновление свойств уязвимого [объектаManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="76acf-107">Update the properties of a [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76acf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="76acf-108">Prerequisites</span></span>
<span data-ttu-id="76acf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76acf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76acf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76acf-111">Permission type</span></span>|<span data-ttu-id="76acf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76acf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76acf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76acf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76acf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76acf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="76acf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76acf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76acf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76acf-116">Not supported.</span></span>|
|<span data-ttu-id="76acf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="76acf-117">Application</span></span>|<span data-ttu-id="76acf-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76acf-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76acf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76acf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="76acf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="76acf-120">Request headers</span></span>
|<span data-ttu-id="76acf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76acf-121">Header</span></span>|<span data-ttu-id="76acf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="76acf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76acf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="76acf-123">Authorization</span></span>|<span data-ttu-id="76acf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76acf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76acf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="76acf-125">Accept</span></span>|<span data-ttu-id="76acf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76acf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76acf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76acf-127">Request body</span></span>
<span data-ttu-id="76acf-128">В теле запроса поставляем представление JSON для уязвимого [объектаManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="76acf-128">In the request body, supply a JSON representation for the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

<span data-ttu-id="76acf-129">В следующей таблице показаны свойства, необходимые при создании [vulnerableManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="76acf-129">The following table shows the properties that are required when you create the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md).</span></span>

|<span data-ttu-id="76acf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="76acf-130">Property</span></span>|<span data-ttu-id="76acf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="76acf-131">Type</span></span>|<span data-ttu-id="76acf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="76acf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76acf-133">id</span><span class="sxs-lookup"><span data-stu-id="76acf-133">id</span></span>|<span data-ttu-id="76acf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="76acf-134">String</span></span>|<span data-ttu-id="76acf-135">Ключ сущности и ID устройства AAD.</span><span class="sxs-lookup"><span data-stu-id="76acf-135">The entity key, and AAD device ID.</span></span>|
|<span data-ttu-id="76acf-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="76acf-136">managedDeviceId</span></span>|<span data-ttu-id="76acf-137">Строка</span><span class="sxs-lookup"><span data-stu-id="76acf-137">String</span></span>|<span data-ttu-id="76acf-138">ID управляемого устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="76acf-138">The Intune managed device ID.</span></span>|
|<span data-ttu-id="76acf-139">displayName</span><span class="sxs-lookup"><span data-stu-id="76acf-139">displayName</span></span>|<span data-ttu-id="76acf-140">Строка</span><span class="sxs-lookup"><span data-stu-id="76acf-140">String</span></span>|<span data-ttu-id="76acf-141">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="76acf-141">The device name.</span></span>|
|<span data-ttu-id="76acf-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="76acf-142">lastSyncDateTime</span></span>|<span data-ttu-id="76acf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76acf-143">DateTimeOffset</span></span>|<span data-ttu-id="76acf-144">Последняя дата синхронизации.</span><span class="sxs-lookup"><span data-stu-id="76acf-144">The last sync date.</span></span>|



## <a name="response"></a><span data-ttu-id="76acf-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="76acf-145">Response</span></span>
<span data-ttu-id="76acf-146">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="76acf-146">If successful, this method returns a `200 OK` response code and an updated [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76acf-147">Пример</span><span class="sxs-lookup"><span data-stu-id="76acf-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="76acf-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="76acf-148">Request</span></span>
<span data-ttu-id="76acf-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76acf-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76acf-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="76acf-150">Response</span></span>
<span data-ttu-id="76acf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76acf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





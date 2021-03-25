---
title: Обновление deviceManagementScriptRunSummary
description: Обновление свойств объекта deviceManagementScriptRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58087ebd6c58607ef37a1326841fa2e47ba18452
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150390"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="1bbc7-103">Обновление deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="1bbc7-103">Update deviceManagementScriptRunSummary</span></span>

<span data-ttu-id="1bbc7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bbc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bbc7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bbc7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bbc7-107">Обновление свойств объекта [deviceManagementScriptRunSummary.](../resources/intune-devices-devicemanagementscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="1bbc7-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bbc7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1bbc7-108">Prerequisites</span></span>
<span data-ttu-id="1bbc7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bbc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bbc7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bbc7-111">Permission type</span></span>|<span data-ttu-id="1bbc7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bbc7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bbc7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bbc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bbc7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bbc7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1bbc7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bbc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bbc7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-116">Not supported.</span></span>|
|<span data-ttu-id="1bbc7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1bbc7-117">Application</span></span>|<span data-ttu-id="1bbc7-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bbc7-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bbc7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bbc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="1bbc7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1bbc7-120">Request headers</span></span>
|<span data-ttu-id="1bbc7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1bbc7-121">Header</span></span>|<span data-ttu-id="1bbc7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1bbc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bbc7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bbc7-123">Authorization</span></span>|<span data-ttu-id="1bbc7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bbc7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1bbc7-125">Accept</span></span>|<span data-ttu-id="1bbc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bbc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bbc7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bbc7-127">Request body</span></span>
<span data-ttu-id="1bbc7-128">В теле запроса поставляем представление JSON для [объекта deviceManagementScriptRunSummary.](../resources/intune-devices-devicemanagementscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="1bbc7-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="1bbc7-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementScriptRunSummary.](../resources/intune-devices-devicemanagementscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="1bbc7-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="1bbc7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bbc7-130">Property</span></span>|<span data-ttu-id="1bbc7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1bbc7-131">Type</span></span>|<span data-ttu-id="1bbc7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1bbc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bbc7-133">id</span><span class="sxs-lookup"><span data-stu-id="1bbc7-133">id</span></span>|<span data-ttu-id="1bbc7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1bbc7-134">String</span></span>|<span data-ttu-id="1bbc7-135">Клавиша скрипта управления устройствами запустит объект сводки.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-135">Key of the device management script run summary entity.</span></span> <span data-ttu-id="1bbc7-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-136">This property is read-only.</span></span>|
|<span data-ttu-id="1bbc7-137">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1bbc7-137">successDeviceCount</span></span>|<span data-ttu-id="1bbc7-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbc7-138">Int32</span></span>|<span data-ttu-id="1bbc7-139">Количество устройств успешности.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-139">Success device count.</span></span>|
|<span data-ttu-id="1bbc7-140">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1bbc7-140">errorDeviceCount</span></span>|<span data-ttu-id="1bbc7-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbc7-141">Int32</span></span>|<span data-ttu-id="1bbc7-142">Количество устройств ошибки.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-142">Error device count.</span></span>|
|<span data-ttu-id="1bbc7-143">successUserCount</span><span class="sxs-lookup"><span data-stu-id="1bbc7-143">successUserCount</span></span>|<span data-ttu-id="1bbc7-144">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbc7-144">Int32</span></span>|<span data-ttu-id="1bbc7-145">Количество пользователей успешности.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-145">Success user count.</span></span>|
|<span data-ttu-id="1bbc7-146">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="1bbc7-146">errorUserCount</span></span>|<span data-ttu-id="1bbc7-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbc7-147">Int32</span></span>|<span data-ttu-id="1bbc7-148">Количество пользователей ошибки.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-148">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="1bbc7-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bbc7-149">Response</span></span>
<span data-ttu-id="1bbc7-150">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-150">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bbc7-151">Пример</span><span class="sxs-lookup"><span data-stu-id="1bbc7-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bbc7-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bbc7-152">Request</span></span>
<span data-ttu-id="1bbc7-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="1bbc7-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bbc7-154">Response</span></span>
<span data-ttu-id="1bbc7-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bbc7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```





---
title: Обновление deviceManagementScriptRunSummary
description: Обновление свойства объекта deviceManagementScriptRunSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55582147aff81bc8d566634a5fb9fdc1ff4ff2fd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413992"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="12781-103">Обновление deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="12781-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="12781-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="12781-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="12781-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12781-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12781-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12781-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12781-107">Обновление свойства объекта [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="12781-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12781-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="12781-108">Prerequisites</span></span>
<span data-ttu-id="12781-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="12781-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="12781-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12781-111">Permission type</span></span>|<span data-ttu-id="12781-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12781-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12781-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12781-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12781-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12781-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="12781-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12781-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12781-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12781-116">Not supported.</span></span>|
|<span data-ttu-id="12781-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12781-117">Application</span></span>|<span data-ttu-id="12781-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12781-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12781-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12781-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="12781-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12781-120">Request headers</span></span>
|<span data-ttu-id="12781-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12781-121">Header</span></span>|<span data-ttu-id="12781-122">Значение</span><span class="sxs-lookup"><span data-stu-id="12781-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12781-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12781-123">Authorization</span></span>|<span data-ttu-id="12781-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="12781-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12781-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12781-125">Accept</span></span>|<span data-ttu-id="12781-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12781-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12781-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12781-127">Request body</span></span>
<span data-ttu-id="12781-128">В тексте запроса укажите представление JSON для объекта [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="12781-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="12781-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="12781-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="12781-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="12781-130">Property</span></span>|<span data-ttu-id="12781-131">Тип</span><span class="sxs-lookup"><span data-stu-id="12781-131">Type</span></span>|<span data-ttu-id="12781-132">Описание</span><span class="sxs-lookup"><span data-stu-id="12781-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12781-133">id</span><span class="sxs-lookup"><span data-stu-id="12781-133">id</span></span>|<span data-ttu-id="12781-134">String</span><span class="sxs-lookup"><span data-stu-id="12781-134">String</span></span>|<span data-ttu-id="12781-135">Клавиша сценарий управления устройства выполните сводки сущности.</span><span class="sxs-lookup"><span data-stu-id="12781-135">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="12781-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12781-136">successDeviceCount</span></span>|<span data-ttu-id="12781-137">Int32</span><span class="sxs-lookup"><span data-stu-id="12781-137">Int32</span></span>|<span data-ttu-id="12781-138">Число допустимых устройства.</span><span class="sxs-lookup"><span data-stu-id="12781-138">Success device count.</span></span>|
|<span data-ttu-id="12781-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12781-139">errorDeviceCount</span></span>|<span data-ttu-id="12781-140">Int32</span><span class="sxs-lookup"><span data-stu-id="12781-140">Int32</span></span>|<span data-ttu-id="12781-141">Число ошибок устройства.</span><span class="sxs-lookup"><span data-stu-id="12781-141">Error device count.</span></span>|
|<span data-ttu-id="12781-142">successUserCount</span><span class="sxs-lookup"><span data-stu-id="12781-142">successUserCount</span></span>|<span data-ttu-id="12781-143">Int32</span><span class="sxs-lookup"><span data-stu-id="12781-143">Int32</span></span>|<span data-ttu-id="12781-144">Число пользователей успеха.</span><span class="sxs-lookup"><span data-stu-id="12781-144">Success user count.</span></span>|
|<span data-ttu-id="12781-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="12781-145">errorUserCount</span></span>|<span data-ttu-id="12781-146">Int32</span><span class="sxs-lookup"><span data-stu-id="12781-146">Int32</span></span>|<span data-ttu-id="12781-147">Число пользователей об ошибках.</span><span class="sxs-lookup"><span data-stu-id="12781-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="12781-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="12781-148">Response</span></span>
<span data-ttu-id="12781-149">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="12781-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12781-150">Пример</span><span class="sxs-lookup"><span data-stu-id="12781-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="12781-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="12781-151">Request</span></span>
<span data-ttu-id="12781-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12781-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
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

### <a name="response"></a><span data-ttu-id="12781-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="12781-153">Response</span></span>
<span data-ttu-id="12781-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="12781-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





---
title: Обновление Виндовсманажементапфеалссуммари
description: Обновление свойств объекта Виндовсманажементапфеалссуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 323e8fdf611b25676f2b1337829a162eedb83f58
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909101"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="ee90e-103">Обновление Виндовсманажементапфеалссуммари</span><span class="sxs-lookup"><span data-stu-id="ee90e-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="ee90e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee90e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee90e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee90e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee90e-106">Обновление свойств объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ee90e-106">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee90e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee90e-107">Prerequisites</span></span>
<span data-ttu-id="ee90e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee90e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee90e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee90e-110">Permission type</span></span>|<span data-ttu-id="ee90e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee90e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee90e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee90e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee90e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee90e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ee90e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee90e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee90e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee90e-115">Not supported.</span></span>|
|<span data-ttu-id="ee90e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee90e-116">Application</span></span>|<span data-ttu-id="ee90e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee90e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee90e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee90e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="ee90e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee90e-119">Request headers</span></span>
|<span data-ttu-id="ee90e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee90e-120">Header</span></span>|<span data-ttu-id="ee90e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ee90e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee90e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee90e-122">Authorization</span></span>|<span data-ttu-id="ee90e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee90e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee90e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ee90e-124">Accept</span></span>|<span data-ttu-id="ee90e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee90e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee90e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee90e-126">Request body</span></span>
<span data-ttu-id="ee90e-127">В тексте запроса добавьте представление объекта [Виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee90e-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="ee90e-128">В следующей таблице приведены свойства, необходимые при создании [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ee90e-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="ee90e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee90e-129">Property</span></span>|<span data-ttu-id="ee90e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ee90e-130">Type</span></span>|<span data-ttu-id="ee90e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ee90e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee90e-132">id</span><span class="sxs-lookup"><span data-stu-id="ee90e-132">id</span></span>|<span data-ttu-id="ee90e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ee90e-133">String</span></span>|<span data-ttu-id="ee90e-134">Ключ объекта сводки работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="ee90e-134">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="ee90e-135">Хеалсидевицекаунт</span><span class="sxs-lookup"><span data-stu-id="ee90e-135">healthyDeviceCount</span></span>|<span data-ttu-id="ee90e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ee90e-136">Int32</span></span>|<span data-ttu-id="ee90e-137">Работоспособное число устройств.</span><span class="sxs-lookup"><span data-stu-id="ee90e-137">Healthy device count.</span></span>|
|<span data-ttu-id="ee90e-138">Унхеалсидевицекаунт</span><span class="sxs-lookup"><span data-stu-id="ee90e-138">unhealthyDeviceCount</span></span>|<span data-ttu-id="ee90e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ee90e-139">Int32</span></span>|<span data-ttu-id="ee90e-140">Неработоспособное число устройств.</span><span class="sxs-lookup"><span data-stu-id="ee90e-140">Unhealthy device count.</span></span>|
|<span data-ttu-id="ee90e-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee90e-141">unknownDeviceCount</span></span>|<span data-ttu-id="ee90e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ee90e-142">Int32</span></span>|<span data-ttu-id="ee90e-143">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="ee90e-143">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="ee90e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee90e-144">Response</span></span>
<span data-ttu-id="ee90e-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee90e-145">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee90e-146">Пример</span><span class="sxs-lookup"><span data-stu-id="ee90e-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee90e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee90e-147">Request</span></span>
<span data-ttu-id="ee90e-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee90e-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a><span data-ttu-id="ee90e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee90e-149">Response</span></span>
<span data-ttu-id="ee90e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee90e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "a9d38a9e-8a9e-a9d3-9e8a-d3a99e8ad3a9",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```





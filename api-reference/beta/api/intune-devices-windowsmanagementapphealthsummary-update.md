---
title: Обновление Виндовсманажементапфеалссуммари
description: Обновление свойств объекта Виндовсманажементапфеалссуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51dc82bea5bee9b92306c0d315f2e5b7a6500eb8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985632"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="0c922-103">Обновление Виндовсманажементапфеалссуммари</span><span class="sxs-lookup"><span data-stu-id="0c922-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="0c922-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c922-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c922-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c922-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c922-106">Обновление свойств объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="0c922-106">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c922-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0c922-107">Prerequisites</span></span>
<span data-ttu-id="0c922-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c922-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c922-110">Permission type</span></span>|<span data-ttu-id="0c922-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c922-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c922-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c922-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c922-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c922-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0c922-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c922-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c922-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c922-115">Not supported.</span></span>|
|<span data-ttu-id="0c922-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c922-116">Application</span></span>|<span data-ttu-id="0c922-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c922-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c922-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c922-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="0c922-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c922-119">Request headers</span></span>
|<span data-ttu-id="0c922-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c922-120">Header</span></span>|<span data-ttu-id="0c922-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0c922-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c922-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c922-122">Authorization</span></span>|<span data-ttu-id="0c922-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c922-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c922-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0c922-124">Accept</span></span>|<span data-ttu-id="0c922-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c922-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c922-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c922-126">Request body</span></span>
<span data-ttu-id="0c922-127">В тексте запроса добавьте представление объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c922-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="0c922-128">В следующей таблице приведены свойства, необходимые при создании [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="0c922-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="0c922-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c922-129">Property</span></span>|<span data-ttu-id="0c922-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0c922-130">Type</span></span>|<span data-ttu-id="0c922-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0c922-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c922-132">id</span><span class="sxs-lookup"><span data-stu-id="0c922-132">id</span></span>|<span data-ttu-id="0c922-133">String</span><span class="sxs-lookup"><span data-stu-id="0c922-133">String</span></span>|<span data-ttu-id="0c922-134">Ключ объекта сводки работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="0c922-134">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="0c922-135">Хеалсидевицекаунт</span><span class="sxs-lookup"><span data-stu-id="0c922-135">healthyDeviceCount</span></span>|<span data-ttu-id="0c922-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0c922-136">Int32</span></span>|<span data-ttu-id="0c922-137">Работоспособное число устройств.</span><span class="sxs-lookup"><span data-stu-id="0c922-137">Healthy device count.</span></span>|
|<span data-ttu-id="0c922-138">Унхеалсидевицекаунт</span><span class="sxs-lookup"><span data-stu-id="0c922-138">unhealthyDeviceCount</span></span>|<span data-ttu-id="0c922-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0c922-139">Int32</span></span>|<span data-ttu-id="0c922-140">Неработоспособное число устройств.</span><span class="sxs-lookup"><span data-stu-id="0c922-140">Unhealthy device count.</span></span>|
|<span data-ttu-id="0c922-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0c922-141">unknownDeviceCount</span></span>|<span data-ttu-id="0c922-142">Int32</span><span class="sxs-lookup"><span data-stu-id="0c922-142">Int32</span></span>|<span data-ttu-id="0c922-143">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="0c922-143">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="0c922-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c922-144">Response</span></span>
<span data-ttu-id="0c922-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c922-145">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c922-146">Пример</span><span class="sxs-lookup"><span data-stu-id="0c922-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c922-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c922-147">Request</span></span>
<span data-ttu-id="0c922-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c922-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c922-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c922-149">Response</span></span>
<span data-ttu-id="0c922-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c922-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






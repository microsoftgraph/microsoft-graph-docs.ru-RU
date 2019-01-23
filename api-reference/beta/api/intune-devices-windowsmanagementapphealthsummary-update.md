---
title: Обновление windowsManagementAppHealthSummary
description: Обновление свойства объекта windowsManagementAppHealthSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d7e8c077b8f06b9647e34a18fd5aa92987272e77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394168"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="54fdd-103">Обновление windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="54fdd-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="54fdd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="54fdd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54fdd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54fdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54fdd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54fdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54fdd-107">Обновление свойства объекта [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="54fdd-107">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54fdd-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="54fdd-108">Prerequisites</span></span>
<span data-ttu-id="54fdd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="54fdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="54fdd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54fdd-111">Permission type</span></span>|<span data-ttu-id="54fdd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54fdd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54fdd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54fdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54fdd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54fdd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="54fdd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54fdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54fdd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54fdd-116">Not supported.</span></span>|
|<span data-ttu-id="54fdd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54fdd-117">Application</span></span>|<span data-ttu-id="54fdd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54fdd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54fdd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54fdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="54fdd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54fdd-120">Request headers</span></span>
|<span data-ttu-id="54fdd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54fdd-121">Header</span></span>|<span data-ttu-id="54fdd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="54fdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54fdd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="54fdd-123">Authorization</span></span>|<span data-ttu-id="54fdd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="54fdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54fdd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="54fdd-125">Accept</span></span>|<span data-ttu-id="54fdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54fdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54fdd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54fdd-127">Request body</span></span>
<span data-ttu-id="54fdd-128">В тексте запроса укажите представление JSON для объекта [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="54fdd-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="54fdd-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="54fdd-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="54fdd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="54fdd-130">Property</span></span>|<span data-ttu-id="54fdd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="54fdd-131">Type</span></span>|<span data-ttu-id="54fdd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="54fdd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54fdd-133">id</span><span class="sxs-lookup"><span data-stu-id="54fdd-133">id</span></span>|<span data-ttu-id="54fdd-134">String</span><span class="sxs-lookup"><span data-stu-id="54fdd-134">String</span></span>|<span data-ttu-id="54fdd-135">Ключ сущности сводки работоспособности приложения управления, Windows.</span><span class="sxs-lookup"><span data-stu-id="54fdd-135">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="54fdd-136">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54fdd-136">healthyDeviceCount</span></span>|<span data-ttu-id="54fdd-137">Int32</span><span class="sxs-lookup"><span data-stu-id="54fdd-137">Int32</span></span>|<span data-ttu-id="54fdd-138">Счетчик работоспособном устройства.</span><span class="sxs-lookup"><span data-stu-id="54fdd-138">Healthy device count.</span></span>|
|<span data-ttu-id="54fdd-139">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54fdd-139">unhealthyDeviceCount</span></span>|<span data-ttu-id="54fdd-140">Int32</span><span class="sxs-lookup"><span data-stu-id="54fdd-140">Int32</span></span>|<span data-ttu-id="54fdd-141">Счетчик неработоспособные устройства.</span><span class="sxs-lookup"><span data-stu-id="54fdd-141">Unhealthy device count.</span></span>|
|<span data-ttu-id="54fdd-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54fdd-142">unknownDeviceCount</span></span>|<span data-ttu-id="54fdd-143">Int32</span><span class="sxs-lookup"><span data-stu-id="54fdd-143">Int32</span></span>|<span data-ttu-id="54fdd-144">Счетчик неизвестные устройства.</span><span class="sxs-lookup"><span data-stu-id="54fdd-144">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="54fdd-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="54fdd-145">Response</span></span>
<span data-ttu-id="54fdd-146">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="54fdd-146">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54fdd-147">Пример</span><span class="sxs-lookup"><span data-stu-id="54fdd-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="54fdd-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="54fdd-148">Request</span></span>
<span data-ttu-id="54fdd-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54fdd-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="54fdd-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="54fdd-150">Response</span></span>
<span data-ttu-id="54fdd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="54fdd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





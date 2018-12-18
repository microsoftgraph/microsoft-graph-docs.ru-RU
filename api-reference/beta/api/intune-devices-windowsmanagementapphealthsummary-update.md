---
title: Обновление windowsManagementAppHealthSummary
description: Обновление свойства объекта windowsManagementAppHealthSummary.
author: tfitzmac
ms.openlocfilehash: 274ffcc65706f7d730815d4a8350af2dee68f763
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307072"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="3b811-103">Обновление windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="3b811-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="3b811-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3b811-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b811-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b811-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b811-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3b811-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b811-107">Обновление свойства объекта [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3b811-107">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b811-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3b811-108">Prerequisites</span></span>
<span data-ttu-id="3b811-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b811-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b811-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b811-111">Permission type</span></span>|<span data-ttu-id="3b811-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b811-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b811-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b811-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b811-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b811-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3b811-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b811-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b811-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b811-116">Not supported.</span></span>|
|<span data-ttu-id="3b811-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b811-117">Application</span></span>|<span data-ttu-id="3b811-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b811-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b811-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b811-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="3b811-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b811-120">Request headers</span></span>
|<span data-ttu-id="3b811-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b811-121">Header</span></span>|<span data-ttu-id="3b811-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3b811-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b811-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b811-123">Authorization</span></span>|<span data-ttu-id="3b811-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3b811-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b811-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b811-125">Accept</span></span>|<span data-ttu-id="3b811-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b811-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b811-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b811-127">Request body</span></span>
<span data-ttu-id="3b811-128">В тексте запроса укажите представление JSON для объекта [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3b811-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="3b811-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3b811-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="3b811-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b811-130">Property</span></span>|<span data-ttu-id="3b811-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3b811-131">Type</span></span>|<span data-ttu-id="3b811-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3b811-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b811-133">id</span><span class="sxs-lookup"><span data-stu-id="3b811-133">id</span></span>|<span data-ttu-id="3b811-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3b811-134">String</span></span>|<span data-ttu-id="3b811-135">Ключ сущности сводки работоспособности приложения управления, Windows.</span><span class="sxs-lookup"><span data-stu-id="3b811-135">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="3b811-136">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b811-136">healthyDeviceCount</span></span>|<span data-ttu-id="3b811-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3b811-137">Int32</span></span>|<span data-ttu-id="3b811-138">Счетчик работоспособном устройства.</span><span class="sxs-lookup"><span data-stu-id="3b811-138">Healthy device count.</span></span>|
|<span data-ttu-id="3b811-139">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b811-139">unhealthyDeviceCount</span></span>|<span data-ttu-id="3b811-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3b811-140">Int32</span></span>|<span data-ttu-id="3b811-141">Счетчик неработоспособные устройства.</span><span class="sxs-lookup"><span data-stu-id="3b811-141">Unhealthy device count.</span></span>|
|<span data-ttu-id="3b811-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b811-142">unknownDeviceCount</span></span>|<span data-ttu-id="3b811-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3b811-143">Int32</span></span>|<span data-ttu-id="3b811-144">Счетчик неизвестные устройства.</span><span class="sxs-lookup"><span data-stu-id="3b811-144">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="3b811-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b811-145">Response</span></span>
<span data-ttu-id="3b811-146">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3b811-146">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b811-147">Пример</span><span class="sxs-lookup"><span data-stu-id="3b811-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b811-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b811-148">Request</span></span>
<span data-ttu-id="3b811-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b811-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
Content-type: application/json
Content-length: 89

{
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a><span data-ttu-id="3b811-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b811-150">Response</span></span>
<span data-ttu-id="3b811-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3b811-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






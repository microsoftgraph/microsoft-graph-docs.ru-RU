---
title: Обновление deviceManagementScriptRunSummary
description: Обновление свойства объекта deviceManagementScriptRunSummary.
ms.openlocfilehash: 83e45ce7cf01f0fe95b2a4240ebafc1dd88507c8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077395"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="06d4c-103">Обновление deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="06d4c-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="06d4c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06d4c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06d4c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06d4c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="06d4c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06d4c-107">Обновление свойства объекта [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="06d4c-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06d4c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="06d4c-108">Prerequisites</span></span>
<span data-ttu-id="06d4c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06d4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06d4c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06d4c-111">Permission type</span></span>|<span data-ttu-id="06d4c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06d4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06d4c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06d4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06d4c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d4c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="06d4c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06d4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06d4c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d4c-116">Not supported.</span></span>|
|<span data-ttu-id="06d4c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06d4c-117">Application</span></span>|<span data-ttu-id="06d4c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d4c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06d4c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06d4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="06d4c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06d4c-120">Request headers</span></span>
|<span data-ttu-id="06d4c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06d4c-121">Header</span></span>|<span data-ttu-id="06d4c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="06d4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06d4c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06d4c-123">Authorization</span></span>|<span data-ttu-id="06d4c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="06d4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06d4c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06d4c-125">Accept</span></span>|<span data-ttu-id="06d4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06d4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06d4c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06d4c-127">Request body</span></span>
<span data-ttu-id="06d4c-128">В тексте запроса укажите представление JSON для объекта [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="06d4c-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="06d4c-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="06d4c-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="06d4c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="06d4c-130">Property</span></span>|<span data-ttu-id="06d4c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="06d4c-131">Type</span></span>|<span data-ttu-id="06d4c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="06d4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06d4c-133">id</span><span class="sxs-lookup"><span data-stu-id="06d4c-133">id</span></span>|<span data-ttu-id="06d4c-134">String</span><span class="sxs-lookup"><span data-stu-id="06d4c-134">String</span></span>|<span data-ttu-id="06d4c-135">Клавиша сценарий управления устройства выполните сводки сущности.</span><span class="sxs-lookup"><span data-stu-id="06d4c-135">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="06d4c-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06d4c-136">successDeviceCount</span></span>|<span data-ttu-id="06d4c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="06d4c-137">Int32</span></span>|<span data-ttu-id="06d4c-138">Число допустимых устройства.</span><span class="sxs-lookup"><span data-stu-id="06d4c-138">Success device count.</span></span>|
|<span data-ttu-id="06d4c-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06d4c-139">errorDeviceCount</span></span>|<span data-ttu-id="06d4c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="06d4c-140">Int32</span></span>|<span data-ttu-id="06d4c-141">Число ошибок устройства.</span><span class="sxs-lookup"><span data-stu-id="06d4c-141">Error device count.</span></span>|
|<span data-ttu-id="06d4c-142">successUserCount</span><span class="sxs-lookup"><span data-stu-id="06d4c-142">successUserCount</span></span>|<span data-ttu-id="06d4c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="06d4c-143">Int32</span></span>|<span data-ttu-id="06d4c-144">Число пользователей успеха.</span><span class="sxs-lookup"><span data-stu-id="06d4c-144">Success user count.</span></span>|
|<span data-ttu-id="06d4c-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="06d4c-145">errorUserCount</span></span>|<span data-ttu-id="06d4c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="06d4c-146">Int32</span></span>|<span data-ttu-id="06d4c-147">Число пользователей об ошибках.</span><span class="sxs-lookup"><span data-stu-id="06d4c-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="06d4c-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="06d4c-148">Response</span></span>
<span data-ttu-id="06d4c-149">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="06d4c-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06d4c-150">Пример</span><span class="sxs-lookup"><span data-stu-id="06d4c-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="06d4c-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d4c-151">Request</span></span>
<span data-ttu-id="06d4c-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06d4c-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
Content-type: application/json
Content-length: 108

{
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="06d4c-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="06d4c-153">Response</span></span>
<span data-ttu-id="06d4c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="06d4c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






---
title: Обновление cloudPCConnectivityIssue
description: Обновление свойств объекта cloudPCConnectivityIssue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d94f7c2409bb4a0a2b09dab066d25c54f8319b87
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666014"
---
# <a name="update-cloudpcconnectivityissue"></a><span data-ttu-id="8e36e-103">Обновление cloudPCConnectivityIssue</span><span class="sxs-lookup"><span data-stu-id="8e36e-103">Update cloudPCConnectivityIssue</span></span>

<span data-ttu-id="8e36e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e36e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e36e-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e36e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e36e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e36e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e36e-107">Обновление свойств объекта [cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)</span><span class="sxs-lookup"><span data-stu-id="8e36e-107">Update the properties of a [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e36e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8e36e-108">Prerequisites</span></span>
<span data-ttu-id="8e36e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e36e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e36e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e36e-111">Permission type</span></span>|<span data-ttu-id="8e36e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e36e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e36e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e36e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e36e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e36e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8e36e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e36e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e36e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e36e-116">Not supported.</span></span>|
|<span data-ttu-id="8e36e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8e36e-117">Application</span></span>|<span data-ttu-id="8e36e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e36e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e36e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e36e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cloudPCConnectivityIssues/{cloudPCConnectivityIssueId}
```

## <a name="request-headers"></a><span data-ttu-id="8e36e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8e36e-120">Request headers</span></span>
|<span data-ttu-id="8e36e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e36e-121">Header</span></span>|<span data-ttu-id="8e36e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8e36e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e36e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e36e-123">Authorization</span></span>|<span data-ttu-id="8e36e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e36e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e36e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8e36e-125">Accept</span></span>|<span data-ttu-id="8e36e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e36e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e36e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e36e-127">Request body</span></span>
<span data-ttu-id="8e36e-128">В теле запроса поставляем представление JSON для [объекта cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)</span><span class="sxs-lookup"><span data-stu-id="8e36e-128">In the request body, supply a JSON representation for the [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) object.</span></span>

<span data-ttu-id="8e36e-129">В следующей таблице показаны свойства, необходимые при создании [cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)</span><span class="sxs-lookup"><span data-stu-id="8e36e-129">The following table shows the properties that are required when you create the [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md).</span></span>

|<span data-ttu-id="8e36e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e36e-130">Property</span></span>|<span data-ttu-id="8e36e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8e36e-131">Type</span></span>|<span data-ttu-id="8e36e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8e36e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e36e-133">id</span><span class="sxs-lookup"><span data-stu-id="8e36e-133">id</span></span>|<span data-ttu-id="8e36e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8e36e-134">String</span></span>|<span data-ttu-id="8e36e-135">Уникальный идентификатор объекта событий событий для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8e36e-135">The unique identifier of the user experience analytics connectivity issue event entity.</span></span>|
|<span data-ttu-id="8e36e-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="8e36e-136">deviceId</span></span>|<span data-ttu-id="8e36e-137">String</span><span class="sxs-lookup"><span data-stu-id="8e36e-137">String</span></span>|<span data-ttu-id="8e36e-138">Устройство Intune устройства, с которое связано подключение.</span><span class="sxs-lookup"><span data-stu-id="8e36e-138">The Intune DeviceId of the device the connection is associated with.</span></span>|
|<span data-ttu-id="8e36e-139">errorCode</span><span class="sxs-lookup"><span data-stu-id="8e36e-139">errorCode</span></span>|<span data-ttu-id="8e36e-140">String</span><span class="sxs-lookup"><span data-stu-id="8e36e-140">String</span></span>|<span data-ttu-id="8e36e-141">Код ошибки проблемы подключения.</span><span class="sxs-lookup"><span data-stu-id="8e36e-141">The error code of the connectivity issue.</span></span>|
|<span data-ttu-id="8e36e-142">errorDateTime</span><span class="sxs-lookup"><span data-stu-id="8e36e-142">errorDateTime</span></span>|<span data-ttu-id="8e36e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e36e-143">DateTimeOffset</span></span>|<span data-ttu-id="8e36e-144">Время начала подключения.</span><span class="sxs-lookup"><span data-stu-id="8e36e-144">The time that the connection initiated.</span></span> <span data-ttu-id="8e36e-145">Время отображается в формате ISO 8601 и времени скоординированного универсального времени (UTC).</span><span class="sxs-lookup"><span data-stu-id="8e36e-145">The time is shown in ISO 8601 format and Coordinated Universal Time (UTC) time.</span></span>|
|<span data-ttu-id="8e36e-146">userId</span><span class="sxs-lookup"><span data-stu-id="8e36e-146">userId</span></span>|<span data-ttu-id="8e36e-147">String</span><span class="sxs-lookup"><span data-stu-id="8e36e-147">String</span></span>|<span data-ttu-id="8e36e-148">Уникальный id пользователя, который инициализирует подключение.</span><span class="sxs-lookup"><span data-stu-id="8e36e-148">The unique id of user who initialize the connection.</span></span>|
|<span data-ttu-id="8e36e-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="8e36e-149">errorDescription</span></span>|<span data-ttu-id="8e36e-150">String</span><span class="sxs-lookup"><span data-stu-id="8e36e-150">String</span></span>|<span data-ttu-id="8e36e-151">Подробное описание того, что пошло не так.</span><span class="sxs-lookup"><span data-stu-id="8e36e-151">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="8e36e-152">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="8e36e-152">recommendedAction</span></span>|<span data-ttu-id="8e36e-153">Строка</span><span class="sxs-lookup"><span data-stu-id="8e36e-153">String</span></span>|<span data-ttu-id="8e36e-154">Рекомендуемое действие для устранения соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="8e36e-154">The recommended action to fix the corresponding error.</span></span>|



## <a name="response"></a><span data-ttu-id="8e36e-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e36e-155">Response</span></span>
<span data-ttu-id="8e36e-156">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8e36e-156">If successful, this method returns a `200 OK` response code and an updated [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e36e-157">Пример</span><span class="sxs-lookup"><span data-stu-id="8e36e-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e36e-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e36e-158">Request</span></span>
<span data-ttu-id="8e36e-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e36e-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cloudPCConnectivityIssues/{cloudPCConnectivityIssueId}
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "deviceId": "Device Id value",
  "errorCode": "Error Code value",
  "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
  "userId": "User Id value",
  "errorDescription": "Error Description value",
  "recommendedAction": "Recommended Action value"
}
```

### <a name="response"></a><span data-ttu-id="8e36e-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e36e-160">Response</span></span>
<span data-ttu-id="8e36e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e36e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "id": "e8e2bf5f-bf5f-e8e2-5fbf-e2e85fbfe2e8",
  "deviceId": "Device Id value",
  "errorCode": "Error Code value",
  "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
  "userId": "User Id value",
  "errorDescription": "Error Description value",
  "recommendedAction": "Recommended Action value"
}
```





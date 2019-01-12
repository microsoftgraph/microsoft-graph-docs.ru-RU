---
title: Обновление объекта deviceConfigurationUserStatus
description: Обновление свойств объекта deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a4f54f3e5280e6b0cdf5526e8eccc0bc7ee7b7ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972049"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="c933b-103">Обновление объекта deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="c933b-103">Update deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="c933b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c933b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c933b-105">Обновление свойств объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c933b-105">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c933b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c933b-106">Prerequisites</span></span>
<span data-ttu-id="c933b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c933b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c933b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c933b-109">Permission type</span></span>|<span data-ttu-id="c933b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c933b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c933b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c933b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c933b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c933b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c933b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c933b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c933b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c933b-114">Not supported.</span></span>|
|<span data-ttu-id="c933b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c933b-115">Application</span></span>|<span data-ttu-id="c933b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c933b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c933b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c933b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="c933b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c933b-118">Request headers</span></span>
|<span data-ttu-id="c933b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c933b-119">Header</span></span>|<span data-ttu-id="c933b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c933b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c933b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c933b-121">Authorization</span></span>|<span data-ttu-id="c933b-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c933b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c933b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c933b-123">Accept</span></span>|<span data-ttu-id="c933b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c933b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c933b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c933b-125">Request body</span></span>
<span data-ttu-id="c933b-126">В тексте запроса добавьте представление объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c933b-126">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="c933b-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c933b-127">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="c933b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c933b-128">Property</span></span>|<span data-ttu-id="c933b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c933b-129">Type</span></span>|<span data-ttu-id="c933b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c933b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c933b-131">id</span><span class="sxs-lookup"><span data-stu-id="c933b-131">id</span></span>|<span data-ttu-id="c933b-132">Строка</span><span class="sxs-lookup"><span data-stu-id="c933b-132">String</span></span>|<span data-ttu-id="c933b-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c933b-133">Key of the entity.</span></span>|
|<span data-ttu-id="c933b-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c933b-134">userDisplayName</span></span>|<span data-ttu-id="c933b-135">String</span><span class="sxs-lookup"><span data-stu-id="c933b-135">String</span></span>|<span data-ttu-id="c933b-136">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="c933b-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="c933b-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="c933b-137">devicesCount</span></span>|<span data-ttu-id="c933b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="c933b-138">Int32</span></span>|<span data-ttu-id="c933b-139">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c933b-139">Devices count for that user.</span></span>|
|<span data-ttu-id="c933b-140">status</span><span class="sxs-lookup"><span data-stu-id="c933b-140">status</span></span>|[<span data-ttu-id="c933b-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c933b-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c933b-142">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="c933b-142">Compliance status of the policy report.</span></span> <span data-ttu-id="c933b-143">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c933b-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c933b-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c933b-144">lastReportedDateTime</span></span>|<span data-ttu-id="c933b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c933b-145">DateTimeOffset</span></span>|<span data-ttu-id="c933b-146">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="c933b-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="c933b-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c933b-147">userPrincipalName</span></span>|<span data-ttu-id="c933b-148">String</span><span class="sxs-lookup"><span data-stu-id="c933b-148">String</span></span>|<span data-ttu-id="c933b-149">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="c933b-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="c933b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c933b-150">Response</span></span>
<span data-ttu-id="c933b-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c933b-151">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c933b-152">Пример</span><span class="sxs-lookup"><span data-stu-id="c933b-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="c933b-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="c933b-153">Request</span></span>
<span data-ttu-id="c933b-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c933b-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="c933b-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="c933b-155">Response</span></span>
<span data-ttu-id="c933b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c933b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




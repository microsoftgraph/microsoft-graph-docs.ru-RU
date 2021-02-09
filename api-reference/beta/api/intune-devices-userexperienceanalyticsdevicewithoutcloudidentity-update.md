---
title: Обновление объекта userExperienceAnalyticsDeviceWithoutCloudIdentity
description: Обновление свойств объекта userExperienceAnalyticsDeviceWithoutCloudIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01ed006ffdc3b3ae2d13d015edb5799324b33efb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161036"
---
# <a name="update-userexperienceanalyticsdevicewithoutcloudidentity"></a><span data-ttu-id="e2111-103">Обновление объекта userExperienceAnalyticsDeviceWithoutCloudIdentity</span><span class="sxs-lookup"><span data-stu-id="e2111-103">Update userExperienceAnalyticsDeviceWithoutCloudIdentity</span></span>

<span data-ttu-id="e2111-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2111-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2111-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2111-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2111-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2111-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2111-107">Обновление свойств объекта [userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)</span><span class="sxs-lookup"><span data-stu-id="e2111-107">Update the properties of a [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2111-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2111-108">Prerequisites</span></span>
<span data-ttu-id="e2111-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2111-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2111-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2111-111">Permission type</span></span>|<span data-ttu-id="e2111-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2111-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2111-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2111-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2111-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2111-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e2111-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2111-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2111-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2111-116">Not supported.</span></span>|
|<span data-ttu-id="e2111-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2111-117">Application</span></span>|<span data-ttu-id="e2111-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2111-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2111-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2111-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicesWithoutCloudIdentity/{userExperienceAnalyticsDeviceWithoutCloudIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="e2111-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e2111-120">Request headers</span></span>
|<span data-ttu-id="e2111-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2111-121">Header</span></span>|<span data-ttu-id="e2111-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e2111-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2111-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2111-123">Authorization</span></span>|<span data-ttu-id="e2111-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2111-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2111-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e2111-125">Accept</span></span>|<span data-ttu-id="e2111-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2111-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2111-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2111-127">Request body</span></span>
<span data-ttu-id="e2111-128">В теле запроса укажу представление объекта [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="e2111-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) object.</span></span>

<span data-ttu-id="e2111-129">В следующей таблице показаны свойства, необходимые при создании [объекта userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)</span><span class="sxs-lookup"><span data-stu-id="e2111-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md).</span></span>

|<span data-ttu-id="e2111-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2111-130">Property</span></span>|<span data-ttu-id="e2111-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e2111-131">Type</span></span>|<span data-ttu-id="e2111-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e2111-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2111-133">id</span><span class="sxs-lookup"><span data-stu-id="e2111-133">id</span></span>|<span data-ttu-id="e2111-134">String</span><span class="sxs-lookup"><span data-stu-id="e2111-134">String</span></span>|<span data-ttu-id="e2111-135">Уникальный идентификатор устройства с присоединением клиента аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="e2111-135">The unique identifier of the user experience analytics tenant attach device.</span></span>|
|<span data-ttu-id="e2111-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="e2111-136">deviceName</span></span>|<span data-ttu-id="e2111-137">String</span><span class="sxs-lookup"><span data-stu-id="e2111-137">String</span></span>|<span data-ttu-id="e2111-138">Имя устройства с присоединением клиента.</span><span class="sxs-lookup"><span data-stu-id="e2111-138">The tenant attach device's name.</span></span>|
|<span data-ttu-id="e2111-139">azureAdDeviceId</span><span class="sxs-lookup"><span data-stu-id="e2111-139">azureAdDeviceId</span></span>|<span data-ttu-id="e2111-140">String</span><span class="sxs-lookup"><span data-stu-id="e2111-140">String</span></span>|<span data-ttu-id="e2111-141">ИД устройства Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e2111-141">Azure Active Directory Device Id</span></span>|



## <a name="response"></a><span data-ttu-id="e2111-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2111-142">Response</span></span>
<span data-ttu-id="e2111-143">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2111-143">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2111-144">Пример</span><span class="sxs-lookup"><span data-stu-id="e2111-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2111-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2111-145">Request</span></span>
<span data-ttu-id="e2111-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2111-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicesWithoutCloudIdentity/{userExperienceAnalyticsDeviceWithoutCloudIdentityId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity",
  "deviceName": "Device Name value",
  "azureAdDeviceId": "Azure Ad Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="e2111-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2111-147">Response</span></span>
<span data-ttu-id="e2111-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2111-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity",
  "id": "80537287-7287-8053-8772-538087725380",
  "deviceName": "Device Name value",
  "azureAdDeviceId": "Azure Ad Device Id value"
}
```





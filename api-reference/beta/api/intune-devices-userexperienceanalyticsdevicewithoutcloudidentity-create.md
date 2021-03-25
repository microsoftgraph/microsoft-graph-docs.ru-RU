---
title: Создание userExperienceAnalyticsDeviceWithoutCloudIdentity
description: Создание нового объекта userExperienceAnalyticsDeviceWithoutCloudIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b1ba3c28e300ec44d104326e5fe11166cb18c37a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157900"
---
# <a name="create-userexperienceanalyticsdevicewithoutcloudidentity"></a><span data-ttu-id="173bf-103">Создание userExperienceAnalyticsDeviceWithoutCloudIdentity</span><span class="sxs-lookup"><span data-stu-id="173bf-103">Create userExperienceAnalyticsDeviceWithoutCloudIdentity</span></span>

<span data-ttu-id="173bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="173bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="173bf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="173bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="173bf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="173bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="173bf-107">Создание нового [объекта userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)</span><span class="sxs-lookup"><span data-stu-id="173bf-107">Create a new [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="173bf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="173bf-108">Prerequisites</span></span>
<span data-ttu-id="173bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="173bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="173bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="173bf-111">Permission type</span></span>|<span data-ttu-id="173bf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="173bf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="173bf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="173bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="173bf-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="173bf-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="173bf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="173bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="173bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="173bf-116">Not supported.</span></span>|
|<span data-ttu-id="173bf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="173bf-117">Application</span></span>|<span data-ttu-id="173bf-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="173bf-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="173bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="173bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDevicesWithoutCloudIdentity
```

## <a name="request-headers"></a><span data-ttu-id="173bf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="173bf-120">Request headers</span></span>
|<span data-ttu-id="173bf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="173bf-121">Header</span></span>|<span data-ttu-id="173bf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="173bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="173bf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="173bf-123">Authorization</span></span>|<span data-ttu-id="173bf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="173bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="173bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="173bf-125">Accept</span></span>|<span data-ttu-id="173bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="173bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="173bf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="173bf-127">Request body</span></span>
<span data-ttu-id="173bf-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsDeviceWithoutCloudIdentity.</span><span class="sxs-lookup"><span data-stu-id="173bf-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceWithoutCloudIdentity object.</span></span>

<span data-ttu-id="173bf-129">В следующей таблице показаны свойства, необходимые при создании объекта userExperienceAnalyticsDeviceWithoutCloudIdentity.</span><span class="sxs-lookup"><span data-stu-id="173bf-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceWithoutCloudIdentity.</span></span>

|<span data-ttu-id="173bf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="173bf-130">Property</span></span>|<span data-ttu-id="173bf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="173bf-131">Type</span></span>|<span data-ttu-id="173bf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="173bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="173bf-133">id</span><span class="sxs-lookup"><span data-stu-id="173bf-133">id</span></span>|<span data-ttu-id="173bf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="173bf-134">String</span></span>|<span data-ttu-id="173bf-135">Уникальный идентификатор устройства для клиентской аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="173bf-135">The unique identifier of the user experience analytics tenant attach device.</span></span>|
|<span data-ttu-id="173bf-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="173bf-136">deviceName</span></span>|<span data-ttu-id="173bf-137">String</span><span class="sxs-lookup"><span data-stu-id="173bf-137">String</span></span>|<span data-ttu-id="173bf-138">Клиент прикрепит имя устройства.</span><span class="sxs-lookup"><span data-stu-id="173bf-138">The tenant attach device's name.</span></span>|
|<span data-ttu-id="173bf-139">azureAdDeviceId</span><span class="sxs-lookup"><span data-stu-id="173bf-139">azureAdDeviceId</span></span>|<span data-ttu-id="173bf-140">Строка</span><span class="sxs-lookup"><span data-stu-id="173bf-140">String</span></span>|<span data-ttu-id="173bf-141">Azure Active Directory Device Id</span><span class="sxs-lookup"><span data-stu-id="173bf-141">Azure Active Directory Device Id</span></span>|



## <a name="response"></a><span data-ttu-id="173bf-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="173bf-142">Response</span></span>
<span data-ttu-id="173bf-143">В случае успеха этот метод возвращает код отклика и объект `201 Created` [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="173bf-143">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="173bf-144">Пример</span><span class="sxs-lookup"><span data-stu-id="173bf-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="173bf-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="173bf-145">Request</span></span>
<span data-ttu-id="173bf-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="173bf-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicesWithoutCloudIdentity
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity",
  "deviceName": "Device Name value",
  "azureAdDeviceId": "Azure Ad Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="173bf-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="173bf-147">Response</span></span>
<span data-ttu-id="173bf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="173bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity",
  "id": "80537287-7287-8053-8772-538087725380",
  "deviceName": "Device Name value",
  "azureAdDeviceId": "Azure Ad Device Id value"
}
```





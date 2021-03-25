---
title: Создание windowsPrivacyDataAccessControlItem
description: Создайте новый объект WindowsPrivacyDataAccessControlItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01b052e50bede136d1c4cf3f8ea2b555ff5fae48
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154709"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="6f16c-103">Создание windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="6f16c-103">Create windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="6f16c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f16c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f16c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f16c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f16c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f16c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f16c-107">Создайте [новый объект WindowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="6f16c-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f16c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6f16c-108">Prerequisites</span></span>
<span data-ttu-id="6f16c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f16c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f16c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f16c-111">Permission type</span></span>|<span data-ttu-id="6f16c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f16c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f16c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f16c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f16c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f16c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f16c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f16c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f16c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f16c-116">Not supported.</span></span>|
|<span data-ttu-id="6f16c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6f16c-117">Application</span></span>|<span data-ttu-id="6f16c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f16c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f16c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f16c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="6f16c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6f16c-120">Request headers</span></span>
|<span data-ttu-id="6f16c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f16c-121">Header</span></span>|<span data-ttu-id="6f16c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6f16c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f16c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f16c-123">Authorization</span></span>|<span data-ttu-id="6f16c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f16c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f16c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f16c-125">Accept</span></span>|<span data-ttu-id="6f16c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f16c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f16c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f16c-127">Request body</span></span>
<span data-ttu-id="6f16c-128">В теле запроса устройте представление JSON для объекта windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="6f16c-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="6f16c-129">В следующей таблице показаны свойства, необходимые при создании windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="6f16c-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="6f16c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f16c-130">Property</span></span>|<span data-ttu-id="6f16c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6f16c-131">Type</span></span>|<span data-ttu-id="6f16c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6f16c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f16c-133">id</span><span class="sxs-lookup"><span data-stu-id="6f16c-133">id</span></span>|<span data-ttu-id="6f16c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6f16c-134">String</span></span>|<span data-ttu-id="6f16c-135">Ключ WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="6f16c-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="6f16c-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="6f16c-136">accessLevel</span></span>|[<span data-ttu-id="6f16c-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="6f16c-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="6f16c-138">Это указывает уровень доступа к категории данных конфиденциальности, которой будет предоставлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="6f16c-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="6f16c-139">Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="6f16c-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="6f16c-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="6f16c-140">dataCategory</span></span>|[<span data-ttu-id="6f16c-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="6f16c-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="6f16c-142">Это указывает на категорию данных конфиденциальности, к которой будет применяться определенный контроль доступа.</span><span class="sxs-lookup"><span data-stu-id="6f16c-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="6f16c-143">Возможные значения: `notConfigured` `accountInfo` , , , , , `appsRunInBackground` , , , `calendar` `callHistory` , , `camera` `contacts` `diagnosticsInfo` `email` , `location` `messaging` `microphone` `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices` .</span><span class="sxs-lookup"><span data-stu-id="6f16c-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="6f16c-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="6f16c-144">appPackageFamilyName</span></span>|<span data-ttu-id="6f16c-145">Строка</span><span class="sxs-lookup"><span data-stu-id="6f16c-145">String</span></span>|<span data-ttu-id="6f16c-146">Семейная фамилия пакета приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="6f16c-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="6f16c-147">При наборе уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="6f16c-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="6f16c-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="6f16c-148">appDisplayName</span></span>|<span data-ttu-id="6f16c-149">String</span><span class="sxs-lookup"><span data-stu-id="6f16c-149">String</span></span>|<span data-ttu-id="6f16c-150">Семейная фамилия пакета приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="6f16c-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="6f16c-151">При наборе уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="6f16c-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="6f16c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f16c-152">Response</span></span>
<span data-ttu-id="6f16c-153">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6f16c-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f16c-154">Пример</span><span class="sxs-lookup"><span data-stu-id="6f16c-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f16c-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f16c-155">Request</span></span>
<span data-ttu-id="6f16c-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f16c-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="6f16c-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f16c-157">Response</span></span>
<span data-ttu-id="6f16c-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f16c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 299

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "03b15556-5556-03b1-5655-b1035655b103",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```





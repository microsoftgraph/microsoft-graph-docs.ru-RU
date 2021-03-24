---
title: Обновление windowsPrivacyDataAccessControlItem
description: Обновление свойств объекта windowsPrivacyDataAccesssControlItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 85c912c244d2554fd9a05ccaedf16bf60cfc565d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147086"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="d68d9-103">Обновление windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="d68d9-103">Update windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="d68d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d68d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d68d9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d68d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d68d9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d68d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d68d9-107">Обновление свойств объекта [windowsPrivacyDataAccesssControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="d68d9-107">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d68d9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d68d9-108">Prerequisites</span></span>
<span data-ttu-id="d68d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d68d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d68d9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d68d9-111">Permission type</span></span>|<span data-ttu-id="d68d9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d68d9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d68d9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d68d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d68d9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d68d9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d68d9-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d68d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d68d9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d68d9-116">Not supported.</span></span>|
|<span data-ttu-id="d68d9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d68d9-117">Application</span></span>|<span data-ttu-id="d68d9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d68d9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d68d9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d68d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="d68d9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d68d9-120">Request headers</span></span>
|<span data-ttu-id="d68d9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d68d9-121">Header</span></span>|<span data-ttu-id="d68d9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d68d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d68d9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d68d9-123">Authorization</span></span>|<span data-ttu-id="d68d9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d68d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d68d9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d68d9-125">Accept</span></span>|<span data-ttu-id="d68d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d68d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d68d9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d68d9-127">Request body</span></span>
<span data-ttu-id="d68d9-128">В теле запроса устройте представление JSON для [объекта windowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="d68d9-128">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="d68d9-129">В следующей таблице показаны свойства, необходимые при создании [windowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="d68d9-129">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="d68d9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d68d9-130">Property</span></span>|<span data-ttu-id="d68d9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d68d9-131">Type</span></span>|<span data-ttu-id="d68d9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d68d9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d68d9-133">id</span><span class="sxs-lookup"><span data-stu-id="d68d9-133">id</span></span>|<span data-ttu-id="d68d9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d68d9-134">String</span></span>|<span data-ttu-id="d68d9-135">Ключ WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="d68d9-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="d68d9-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="d68d9-136">accessLevel</span></span>|[<span data-ttu-id="d68d9-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="d68d9-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="d68d9-138">Это указывает уровень доступа к категории данных конфиденциальности, которой будет предоставлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="d68d9-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="d68d9-139">Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="d68d9-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="d68d9-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="d68d9-140">dataCategory</span></span>|[<span data-ttu-id="d68d9-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="d68d9-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="d68d9-142">Это указывает на категорию данных конфиденциальности, к которой будет применяться определенный контроль доступа.</span><span class="sxs-lookup"><span data-stu-id="d68d9-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="d68d9-143">Возможные значения: `notConfigured` `accountInfo` , , , , , `appsRunInBackground` , , , `calendar` `callHistory` , , `camera` `contacts` `diagnosticsInfo` `email` , `location` `messaging` `microphone` `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices` .</span><span class="sxs-lookup"><span data-stu-id="d68d9-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="d68d9-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="d68d9-144">appPackageFamilyName</span></span>|<span data-ttu-id="d68d9-145">Строка</span><span class="sxs-lookup"><span data-stu-id="d68d9-145">String</span></span>|<span data-ttu-id="d68d9-146">Семейная фамилия пакета приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="d68d9-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="d68d9-147">При наборе уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="d68d9-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="d68d9-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="d68d9-148">appDisplayName</span></span>|<span data-ttu-id="d68d9-149">String</span><span class="sxs-lookup"><span data-stu-id="d68d9-149">String</span></span>|<span data-ttu-id="d68d9-150">Семейная фамилия пакета приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="d68d9-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="d68d9-151">При наборе уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="d68d9-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="d68d9-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d68d9-152">Response</span></span>
<span data-ttu-id="d68d9-153">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d68d9-153">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d68d9-154">Пример</span><span class="sxs-lookup"><span data-stu-id="d68d9-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="d68d9-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="d68d9-155">Request</span></span>
<span data-ttu-id="d68d9-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d68d9-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
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

### <a name="response"></a><span data-ttu-id="d68d9-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="d68d9-157">Response</span></span>
<span data-ttu-id="d68d9-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d68d9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





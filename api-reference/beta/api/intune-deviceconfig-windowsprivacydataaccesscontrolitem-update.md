---
title: Обновление Виндовспривацидатаакцессконтролитем
description: Обновление свойств объекта Виндовспривацидатаакцессконтролитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 22ca8ba09f46397f158f7c1320c1706e218400b2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49278515"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="67cc5-103">Обновление Виндовспривацидатаакцессконтролитем</span><span class="sxs-lookup"><span data-stu-id="67cc5-103">Update windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="67cc5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67cc5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67cc5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67cc5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67cc5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67cc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67cc5-107">Обновление свойств объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="67cc5-107">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67cc5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="67cc5-108">Prerequisites</span></span>
<span data-ttu-id="67cc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67cc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67cc5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67cc5-111">Permission type</span></span>|<span data-ttu-id="67cc5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="67cc5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67cc5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67cc5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67cc5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67cc5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67cc5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67cc5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67cc5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67cc5-116">Not supported.</span></span>|
|<span data-ttu-id="67cc5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67cc5-117">Application</span></span>|<span data-ttu-id="67cc5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67cc5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67cc5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67cc5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="67cc5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="67cc5-120">Request headers</span></span>
|<span data-ttu-id="67cc5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67cc5-121">Header</span></span>|<span data-ttu-id="67cc5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="67cc5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67cc5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67cc5-123">Authorization</span></span>|<span data-ttu-id="67cc5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67cc5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67cc5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="67cc5-125">Accept</span></span>|<span data-ttu-id="67cc5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67cc5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67cc5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67cc5-127">Request body</span></span>
<span data-ttu-id="67cc5-128">В тексте запроса добавьте представление объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67cc5-128">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="67cc5-129">В следующей таблице приведены свойства, необходимые при создании [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span><span class="sxs-lookup"><span data-stu-id="67cc5-129">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="67cc5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="67cc5-130">Property</span></span>|<span data-ttu-id="67cc5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="67cc5-131">Type</span></span>|<span data-ttu-id="67cc5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="67cc5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67cc5-133">id</span><span class="sxs-lookup"><span data-stu-id="67cc5-133">id</span></span>|<span data-ttu-id="67cc5-134">String</span><span class="sxs-lookup"><span data-stu-id="67cc5-134">String</span></span>|<span data-ttu-id="67cc5-135">Ключ Виндовспривацидатаакцессконтролитем.</span><span class="sxs-lookup"><span data-stu-id="67cc5-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="67cc5-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="67cc5-136">accessLevel</span></span>|[<span data-ttu-id="67cc5-137">виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="67cc5-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="67cc5-138">Указывает уровень доступа для категории данных о конфиденциальности, в которую будет передано указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="67cc5-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="67cc5-139">Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="67cc5-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="67cc5-140">Категория "</span><span class="sxs-lookup"><span data-stu-id="67cc5-140">dataCategory</span></span>|[<span data-ttu-id="67cc5-141">виндовспривацидатакатегори</span><span class="sxs-lookup"><span data-stu-id="67cc5-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="67cc5-142">Указывает категорию данных о конфиденциальности, к которой будет применяться конкретное управление доступом.</span><span class="sxs-lookup"><span data-stu-id="67cc5-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="67cc5-143">Возможные значения:,,,,,,,,,,,,, `notConfigured` `accountInfo` `appsRunInBackground` `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone` `motion` `notifications` , `phone` , `radios` `tasks` `syncWithDevices` `trustedDevices` ,, и.</span><span class="sxs-lookup"><span data-stu-id="67cc5-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="67cc5-144">апппаккажефамилинаме</span><span class="sxs-lookup"><span data-stu-id="67cc5-144">appPackageFamilyName</span></span>|<span data-ttu-id="67cc5-145">String</span><span class="sxs-lookup"><span data-stu-id="67cc5-145">String</span></span>|<span data-ttu-id="67cc5-146">Имя семейства пакетов для приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="67cc5-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="67cc5-147">Если этот параметр установлен, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="67cc5-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="67cc5-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="67cc5-148">appDisplayName</span></span>|<span data-ttu-id="67cc5-149">String</span><span class="sxs-lookup"><span data-stu-id="67cc5-149">String</span></span>|<span data-ttu-id="67cc5-150">Имя семейства пакетов для приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="67cc5-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="67cc5-151">Если этот параметр установлен, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="67cc5-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="67cc5-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="67cc5-152">Response</span></span>
<span data-ttu-id="67cc5-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67cc5-153">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67cc5-154">Пример</span><span class="sxs-lookup"><span data-stu-id="67cc5-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="67cc5-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="67cc5-155">Request</span></span>
<span data-ttu-id="67cc5-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67cc5-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67cc5-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="67cc5-157">Response</span></span>
<span data-ttu-id="67cc5-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67cc5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





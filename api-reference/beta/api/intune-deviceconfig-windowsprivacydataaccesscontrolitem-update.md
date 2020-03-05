---
title: Обновление Виндовспривацидатаакцессконтролитем
description: Обновление свойств объекта Виндовспривацидатаакцессконтролитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3305b7337f84c3b38b0169770a020c30b5d828fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42473803"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="bacaa-103">Обновление Виндовспривацидатаакцессконтролитем</span><span class="sxs-lookup"><span data-stu-id="bacaa-103">Update windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="bacaa-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bacaa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bacaa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bacaa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bacaa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bacaa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bacaa-107">Обновление свойств объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="bacaa-107">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bacaa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bacaa-108">Prerequisites</span></span>
<span data-ttu-id="bacaa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bacaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bacaa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bacaa-111">Permission type</span></span>|<span data-ttu-id="bacaa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bacaa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bacaa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bacaa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bacaa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bacaa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bacaa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bacaa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bacaa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bacaa-116">Not supported.</span></span>|
|<span data-ttu-id="bacaa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bacaa-117">Application</span></span>|<span data-ttu-id="bacaa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bacaa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bacaa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bacaa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="bacaa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bacaa-120">Request headers</span></span>
|<span data-ttu-id="bacaa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bacaa-121">Header</span></span>|<span data-ttu-id="bacaa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bacaa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bacaa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bacaa-123">Authorization</span></span>|<span data-ttu-id="bacaa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bacaa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bacaa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bacaa-125">Accept</span></span>|<span data-ttu-id="bacaa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bacaa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bacaa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bacaa-127">Request body</span></span>
<span data-ttu-id="bacaa-128">В тексте запроса добавьте представление объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bacaa-128">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="bacaa-129">В следующей таблице приведены свойства, необходимые при создании [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span><span class="sxs-lookup"><span data-stu-id="bacaa-129">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="bacaa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bacaa-130">Property</span></span>|<span data-ttu-id="bacaa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bacaa-131">Type</span></span>|<span data-ttu-id="bacaa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bacaa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bacaa-133">id</span><span class="sxs-lookup"><span data-stu-id="bacaa-133">id</span></span>|<span data-ttu-id="bacaa-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bacaa-134">String</span></span>|<span data-ttu-id="bacaa-135">Ключ Виндовспривацидатаакцессконтролитем.</span><span class="sxs-lookup"><span data-stu-id="bacaa-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="bacaa-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="bacaa-136">accessLevel</span></span>|[<span data-ttu-id="bacaa-137">виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="bacaa-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="bacaa-138">Указывает уровень доступа для категории данных о конфиденциальности, в которую будет передано указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="bacaa-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="bacaa-139">Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="bacaa-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="bacaa-140">Категория "</span><span class="sxs-lookup"><span data-stu-id="bacaa-140">dataCategory</span></span>|[<span data-ttu-id="bacaa-141">виндовспривацидатакатегори</span><span class="sxs-lookup"><span data-stu-id="bacaa-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="bacaa-142">Указывает категорию данных о конфиденциальности, к которой будет применяться конкретное управление доступом.</span><span class="sxs-lookup"><span data-stu-id="bacaa-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="bacaa-143">Возможные `notConfigured`значения: `accountInfo`,, `appsRunInBackground`, `calendar` `callHistory` `camera` `contacts` `tasks` `syncWithDevices` `radios` `notifications` `phone` `trustedDevices`,, `email`,,,,,,,,,,,, и. `diagnosticsInfo` `location` `messaging` `microphone` `motion`</span><span class="sxs-lookup"><span data-stu-id="bacaa-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="bacaa-144">апппаккажефамилинаме</span><span class="sxs-lookup"><span data-stu-id="bacaa-144">appPackageFamilyName</span></span>|<span data-ttu-id="bacaa-145">String</span><span class="sxs-lookup"><span data-stu-id="bacaa-145">String</span></span>|<span data-ttu-id="bacaa-146">Имя семейства пакетов для приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="bacaa-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="bacaa-147">Если этот параметр установлен, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="bacaa-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="bacaa-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="bacaa-148">appDisplayName</span></span>|<span data-ttu-id="bacaa-149">String</span><span class="sxs-lookup"><span data-stu-id="bacaa-149">String</span></span>|<span data-ttu-id="bacaa-150">Имя семейства пакетов для приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="bacaa-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="bacaa-151">Если этот параметр установлен, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="bacaa-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="bacaa-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="bacaa-152">Response</span></span>
<span data-ttu-id="bacaa-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bacaa-153">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bacaa-154">Пример</span><span class="sxs-lookup"><span data-stu-id="bacaa-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="bacaa-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="bacaa-155">Request</span></span>
<span data-ttu-id="bacaa-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bacaa-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bacaa-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="bacaa-157">Response</span></span>
<span data-ttu-id="bacaa-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bacaa-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






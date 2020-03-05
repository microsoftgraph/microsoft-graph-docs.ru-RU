---
title: Создание Виндовспривацидатаакцессконтролитем
description: Создание нового объекта Виндовспривацидатаакцессконтролитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91a9ed35325ec9d85ead030d07ddef973cbde0d0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42473957"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="e3740-103">Создание Виндовспривацидатаакцессконтролитем</span><span class="sxs-lookup"><span data-stu-id="e3740-103">Create windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="e3740-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e3740-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3740-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3740-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3740-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3740-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3740-107">Создание нового объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="e3740-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3740-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e3740-108">Prerequisites</span></span>
<span data-ttu-id="e3740-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3740-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3740-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3740-111">Permission type</span></span>|<span data-ttu-id="e3740-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3740-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3740-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3740-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3740-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3740-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3740-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3740-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3740-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3740-116">Not supported.</span></span>|
|<span data-ttu-id="e3740-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3740-117">Application</span></span>|<span data-ttu-id="e3740-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3740-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3740-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3740-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="e3740-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e3740-120">Request headers</span></span>
|<span data-ttu-id="e3740-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3740-121">Header</span></span>|<span data-ttu-id="e3740-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e3740-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3740-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3740-123">Authorization</span></span>|<span data-ttu-id="e3740-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3740-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3740-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3740-125">Accept</span></span>|<span data-ttu-id="e3740-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3740-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3740-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3740-127">Request body</span></span>
<span data-ttu-id="e3740-128">В тексте запроса добавьте представление объекта Виндовспривацидатаакцессконтролитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3740-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="e3740-129">В следующей таблице приведены свойства, необходимые при создании Виндовспривацидатаакцессконтролитем.</span><span class="sxs-lookup"><span data-stu-id="e3740-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="e3740-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3740-130">Property</span></span>|<span data-ttu-id="e3740-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e3740-131">Type</span></span>|<span data-ttu-id="e3740-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e3740-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3740-133">id</span><span class="sxs-lookup"><span data-stu-id="e3740-133">id</span></span>|<span data-ttu-id="e3740-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e3740-134">String</span></span>|<span data-ttu-id="e3740-135">Ключ Виндовспривацидатаакцессконтролитем.</span><span class="sxs-lookup"><span data-stu-id="e3740-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="e3740-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="e3740-136">accessLevel</span></span>|[<span data-ttu-id="e3740-137">виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="e3740-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="e3740-138">Указывает уровень доступа для категории данных о конфиденциальности, в которую будет передано указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="e3740-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="e3740-139">Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="e3740-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="e3740-140">Категория "</span><span class="sxs-lookup"><span data-stu-id="e3740-140">dataCategory</span></span>|[<span data-ttu-id="e3740-141">виндовспривацидатакатегори</span><span class="sxs-lookup"><span data-stu-id="e3740-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="e3740-142">Указывает категорию данных о конфиденциальности, к которой будет применяться конкретное управление доступом.</span><span class="sxs-lookup"><span data-stu-id="e3740-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="e3740-143">Возможные `notConfigured`значения: `accountInfo`,, `appsRunInBackground`, `calendar` `callHistory` `camera` `contacts` `tasks` `syncWithDevices` `radios` `notifications` `phone` `trustedDevices`,, `email`,,,,,,,,,,,, и. `diagnosticsInfo` `location` `messaging` `microphone` `motion`</span><span class="sxs-lookup"><span data-stu-id="e3740-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="e3740-144">апппаккажефамилинаме</span><span class="sxs-lookup"><span data-stu-id="e3740-144">appPackageFamilyName</span></span>|<span data-ttu-id="e3740-145">String</span><span class="sxs-lookup"><span data-stu-id="e3740-145">String</span></span>|<span data-ttu-id="e3740-146">Имя семейства пакетов для приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="e3740-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="e3740-147">Если этот параметр установлен, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="e3740-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="e3740-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="e3740-148">appDisplayName</span></span>|<span data-ttu-id="e3740-149">String</span><span class="sxs-lookup"><span data-stu-id="e3740-149">String</span></span>|<span data-ttu-id="e3740-150">Имя семейства пакетов для приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="e3740-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="e3740-151">Если этот параметр установлен, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="e3740-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="e3740-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3740-152">Response</span></span>
<span data-ttu-id="e3740-153">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3740-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3740-154">Пример</span><span class="sxs-lookup"><span data-stu-id="e3740-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3740-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3740-155">Request</span></span>
<span data-ttu-id="e3740-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3740-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3740-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3740-157">Response</span></span>
<span data-ttu-id="e3740-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3740-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






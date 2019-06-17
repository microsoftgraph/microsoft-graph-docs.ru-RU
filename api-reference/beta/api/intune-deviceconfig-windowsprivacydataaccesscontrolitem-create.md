---
title: Создание Виндовспривацидатаакцессконтролитем
description: Создание нового объекта Виндовспривацидатаакцессконтролитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad45bc27fb97024d40e4522083d766519ac4f017
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961436"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="a76a3-103">Создание Виндовспривацидатаакцессконтролитем</span><span class="sxs-lookup"><span data-stu-id="a76a3-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="a76a3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a76a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a76a3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a76a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a76a3-106">Создание нового объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="a76a3-106">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a76a3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a76a3-107">Prerequisites</span></span>
<span data-ttu-id="a76a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a76a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a76a3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a76a3-110">Permission type</span></span>|<span data-ttu-id="a76a3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a76a3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a76a3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a76a3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a76a3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a76a3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a76a3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a76a3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a76a3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a76a3-115">Not supported.</span></span>|
|<span data-ttu-id="a76a3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a76a3-116">Application</span></span>|<span data-ttu-id="a76a3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a76a3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a76a3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a76a3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="a76a3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a76a3-119">Request headers</span></span>
|<span data-ttu-id="a76a3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a76a3-120">Header</span></span>|<span data-ttu-id="a76a3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a76a3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a76a3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a76a3-122">Authorization</span></span>|<span data-ttu-id="a76a3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a76a3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a76a3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a76a3-124">Accept</span></span>|<span data-ttu-id="a76a3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a76a3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a76a3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a76a3-126">Request body</span></span>
<span data-ttu-id="a76a3-127">В тексте запроса добавьте представление объекта Виндовспривацидатаакцессконтролитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a76a3-127">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="a76a3-128">В следующей таблице приведены свойства, необходимые при создании Виндовспривацидатаакцессконтролитем.</span><span class="sxs-lookup"><span data-stu-id="a76a3-128">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="a76a3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a76a3-129">Property</span></span>|<span data-ttu-id="a76a3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a76a3-130">Type</span></span>|<span data-ttu-id="a76a3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a76a3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a76a3-132">id</span><span class="sxs-lookup"><span data-stu-id="a76a3-132">id</span></span>|<span data-ttu-id="a76a3-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a76a3-133">String</span></span>|<span data-ttu-id="a76a3-134">Ключ Виндовспривацидатаакцессконтролитем.</span><span class="sxs-lookup"><span data-stu-id="a76a3-134">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="a76a3-135">accessLevel</span><span class="sxs-lookup"><span data-stu-id="a76a3-135">accessLevel</span></span>|[<span data-ttu-id="a76a3-136">Виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="a76a3-136">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="a76a3-137">Указывает уровень доступа для категории данных о конфиденциальности, в которую будет передано указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="a76a3-137">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="a76a3-138">Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="a76a3-138">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="a76a3-139">Категория "</span><span class="sxs-lookup"><span data-stu-id="a76a3-139">dataCategory</span></span>|[<span data-ttu-id="a76a3-140">Виндовспривацидатакатегори</span><span class="sxs-lookup"><span data-stu-id="a76a3-140">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="a76a3-141">Указывает категорию данных о конфиденциальности, к которой будет применяться конкретное управление доступом.</span><span class="sxs-lookup"><span data-stu-id="a76a3-141">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="a76a3-142">Возможные значения: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar` `callHistory` `camera` `contacts` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices` `microphone` `motion`,,,,,,,,,,,,,,,,,,,,, `diagnosticsInfo` `email` `location` `messaging` .</span><span class="sxs-lookup"><span data-stu-id="a76a3-142">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="a76a3-143">Апппаккажефамилинаме</span><span class="sxs-lookup"><span data-stu-id="a76a3-143">appPackageFamilyName</span></span>|<span data-ttu-id="a76a3-144">String</span><span class="sxs-lookup"><span data-stu-id="a76a3-144">String</span></span>|<span data-ttu-id="a76a3-145">Имя семейства пакетов для приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="a76a3-145">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="a76a3-146">Если этот параметр установлен, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="a76a3-146">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="a76a3-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="a76a3-147">appDisplayName</span></span>|<span data-ttu-id="a76a3-148">String</span><span class="sxs-lookup"><span data-stu-id="a76a3-148">String</span></span>|<span data-ttu-id="a76a3-149">Имя семейства пакетов для приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="a76a3-149">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="a76a3-150">Если этот параметр установлен, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="a76a3-150">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="a76a3-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="a76a3-151">Response</span></span>
<span data-ttu-id="a76a3-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a76a3-152">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a76a3-153">Пример</span><span class="sxs-lookup"><span data-stu-id="a76a3-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a76a3-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="a76a3-154">Request</span></span>
<span data-ttu-id="a76a3-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a76a3-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a76a3-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a76a3-156">Response</span></span>
<span data-ttu-id="a76a3-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a76a3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






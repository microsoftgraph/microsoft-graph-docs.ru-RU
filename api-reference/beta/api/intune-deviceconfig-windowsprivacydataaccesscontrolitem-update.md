---
title: Обновление windowsPrivacyDataAccessControlItem
description: Обновление свойства объекта windowsPrivacyDataAccessControlItem.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bc73bc6a47441cef45c102ecaa552bd66a7ddc60
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412746"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="3af50-103">Обновление windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="3af50-103">Update windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="3af50-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3af50-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3af50-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3af50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3af50-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3af50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3af50-107">Обновление свойства объекта [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3af50-107">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3af50-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="3af50-108">Prerequisites</span></span>
<span data-ttu-id="3af50-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3af50-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3af50-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3af50-111">Permission type</span></span>|<span data-ttu-id="3af50-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3af50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3af50-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3af50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3af50-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3af50-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3af50-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3af50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3af50-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3af50-116">Not supported.</span></span>|
|<span data-ttu-id="3af50-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3af50-117">Application</span></span>|<span data-ttu-id="3af50-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3af50-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3af50-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3af50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="3af50-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3af50-120">Request headers</span></span>
|<span data-ttu-id="3af50-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3af50-121">Header</span></span>|<span data-ttu-id="3af50-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3af50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3af50-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3af50-123">Authorization</span></span>|<span data-ttu-id="3af50-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3af50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3af50-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3af50-125">Accept</span></span>|<span data-ttu-id="3af50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3af50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3af50-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3af50-127">Request body</span></span>
<span data-ttu-id="3af50-128">В тексте запроса укажите представление JSON для объекта [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3af50-128">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="3af50-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span><span class="sxs-lookup"><span data-stu-id="3af50-129">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="3af50-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3af50-130">Property</span></span>|<span data-ttu-id="3af50-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3af50-131">Type</span></span>|<span data-ttu-id="3af50-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3af50-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3af50-133">id</span><span class="sxs-lookup"><span data-stu-id="3af50-133">id</span></span>|<span data-ttu-id="3af50-134">String</span><span class="sxs-lookup"><span data-stu-id="3af50-134">String</span></span>|<span data-ttu-id="3af50-135">Ключ WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="3af50-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="3af50-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="3af50-136">accessLevel</span></span>|[<span data-ttu-id="3af50-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="3af50-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="3af50-138">Указывает уровень доступа для категории конфиденциальности данных, к которому будет предоставлен указанного приложения к.</span><span class="sxs-lookup"><span data-stu-id="3af50-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="3af50-139">Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="3af50-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="3af50-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="3af50-140">dataCategory</span></span>|[<span data-ttu-id="3af50-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="3af50-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="3af50-142">Указывает категорию конфиденциальности данных, к которому будет применяться контроля доступа к определенным.</span><span class="sxs-lookup"><span data-stu-id="3af50-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="3af50-143">Возможные значения: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices` .</span><span class="sxs-lookup"><span data-stu-id="3af50-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="3af50-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="3af50-144">appPackageFamilyName</span></span>|<span data-ttu-id="3af50-145">String</span><span class="sxs-lookup"><span data-stu-id="3af50-145">String</span></span>|<span data-ttu-id="3af50-146">Имя семейства пакет приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="3af50-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="3af50-147">Если задано, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="3af50-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="3af50-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="3af50-148">appDisplayName</span></span>|<span data-ttu-id="3af50-149">String</span><span class="sxs-lookup"><span data-stu-id="3af50-149">String</span></span>|<span data-ttu-id="3af50-150">Имя семейства пакет приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="3af50-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="3af50-151">Если задано, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="3af50-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="3af50-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3af50-152">Response</span></span>
<span data-ttu-id="3af50-153">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3af50-153">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3af50-154">Пример</span><span class="sxs-lookup"><span data-stu-id="3af50-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="3af50-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="3af50-155">Request</span></span>
<span data-ttu-id="3af50-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3af50-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3af50-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="3af50-157">Response</span></span>
<span data-ttu-id="3af50-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3af50-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





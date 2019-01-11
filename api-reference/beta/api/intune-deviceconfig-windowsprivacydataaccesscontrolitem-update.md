---
title: Обновление windowsPrivacyDataAccessControlItem
description: Обновление свойства объекта windowsPrivacyDataAccessControlItem.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3a989f4c05bff61f86c93873ad817013b6fab2bf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807128"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="4c49c-103">Обновление windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="4c49c-103">Update windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="4c49c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4c49c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c49c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c49c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c49c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4c49c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c49c-107">Обновление свойства объекта [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="4c49c-107">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c49c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4c49c-108">Prerequisites</span></span>
<span data-ttu-id="4c49c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c49c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c49c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c49c-111">Permission type</span></span>|<span data-ttu-id="4c49c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c49c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c49c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c49c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c49c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c49c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c49c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c49c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c49c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c49c-116">Not supported.</span></span>|
|<span data-ttu-id="4c49c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c49c-117">Application</span></span>|<span data-ttu-id="4c49c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c49c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c49c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c49c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="4c49c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c49c-120">Request headers</span></span>
|<span data-ttu-id="4c49c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c49c-121">Header</span></span>|<span data-ttu-id="4c49c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4c49c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c49c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c49c-123">Authorization</span></span>|<span data-ttu-id="4c49c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4c49c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c49c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c49c-125">Accept</span></span>|<span data-ttu-id="4c49c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c49c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c49c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c49c-127">Request body</span></span>
<span data-ttu-id="4c49c-128">В тексте запроса укажите представление JSON для объекта [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="4c49c-128">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="4c49c-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span><span class="sxs-lookup"><span data-stu-id="4c49c-129">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="4c49c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c49c-130">Property</span></span>|<span data-ttu-id="4c49c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4c49c-131">Type</span></span>|<span data-ttu-id="4c49c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4c49c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c49c-133">id</span><span class="sxs-lookup"><span data-stu-id="4c49c-133">id</span></span>|<span data-ttu-id="4c49c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4c49c-134">String</span></span>|<span data-ttu-id="4c49c-135">Ключ WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="4c49c-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="4c49c-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="4c49c-136">accessLevel</span></span>|[<span data-ttu-id="4c49c-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="4c49c-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="4c49c-138">Указывает уровень доступа для категории конфиденциальности данных, к которому будет предоставлен указанного приложения к.</span><span class="sxs-lookup"><span data-stu-id="4c49c-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="4c49c-139">Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="4c49c-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="4c49c-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="4c49c-140">dataCategory</span></span>|[<span data-ttu-id="4c49c-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="4c49c-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="4c49c-142">Указывает категорию конфиденциальности данных, к которому будет применяться контроля доступа к определенным.</span><span class="sxs-lookup"><span data-stu-id="4c49c-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="4c49c-143">Возможные значения: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices` .</span><span class="sxs-lookup"><span data-stu-id="4c49c-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="4c49c-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="4c49c-144">appPackageFamilyName</span></span>|<span data-ttu-id="4c49c-145">Строка</span><span class="sxs-lookup"><span data-stu-id="4c49c-145">String</span></span>|<span data-ttu-id="4c49c-146">Имя семейства пакет приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="4c49c-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="4c49c-147">Если задано, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="4c49c-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="4c49c-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="4c49c-148">appDisplayName</span></span>|<span data-ttu-id="4c49c-149">Строка</span><span class="sxs-lookup"><span data-stu-id="4c49c-149">String</span></span>|<span data-ttu-id="4c49c-150">Имя семейства пакет приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="4c49c-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="4c49c-151">Если задано, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="4c49c-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="4c49c-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c49c-152">Response</span></span>
<span data-ttu-id="4c49c-153">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4c49c-153">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c49c-154">Пример</span><span class="sxs-lookup"><span data-stu-id="4c49c-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c49c-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c49c-155">Request</span></span>
<span data-ttu-id="4c49c-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c49c-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
Content-type: application/json
Content-length: 176

{
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="4c49c-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c49c-157">Response</span></span>
<span data-ttu-id="4c49c-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4c49c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






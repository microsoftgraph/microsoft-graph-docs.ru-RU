---
title: Создание windowsPrivacyDataAccessControlItem
description: Создание нового объекта windowsPrivacyDataAccessControlItem.
author: tfitzmac
ms.openlocfilehash: 262f6866c37d3ed624916189a25ce5a5b5fd0634
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337683"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="d631a-103">Создание windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="d631a-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="d631a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d631a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d631a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d631a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d631a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d631a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d631a-107">Создание нового объекта [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="d631a-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d631a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d631a-108">Prerequisites</span></span>
<span data-ttu-id="d631a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d631a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d631a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d631a-111">Permission type</span></span>|<span data-ttu-id="d631a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d631a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d631a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d631a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d631a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d631a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d631a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d631a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d631a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d631a-116">Not supported.</span></span>|
|<span data-ttu-id="d631a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d631a-117">Application</span></span>|<span data-ttu-id="d631a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d631a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d631a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d631a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="d631a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d631a-120">Request headers</span></span>
|<span data-ttu-id="d631a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d631a-121">Header</span></span>|<span data-ttu-id="d631a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d631a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d631a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d631a-123">Authorization</span></span>|<span data-ttu-id="d631a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d631a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d631a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d631a-125">Accept</span></span>|<span data-ttu-id="d631a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d631a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d631a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d631a-127">Request body</span></span>
<span data-ttu-id="d631a-128">В тексте запроса укажите представление JSON для объекта windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="d631a-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="d631a-129">В следующей таблице показаны свойства, которые необходимы для создания windowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="d631a-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="d631a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d631a-130">Property</span></span>|<span data-ttu-id="d631a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d631a-131">Type</span></span>|<span data-ttu-id="d631a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d631a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d631a-133">id</span><span class="sxs-lookup"><span data-stu-id="d631a-133">id</span></span>|<span data-ttu-id="d631a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d631a-134">String</span></span>|<span data-ttu-id="d631a-135">Ключ WindowsPrivacyDataAccessControlItem.</span><span class="sxs-lookup"><span data-stu-id="d631a-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="d631a-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="d631a-136">accessLevel</span></span>|[<span data-ttu-id="d631a-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="d631a-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="d631a-138">Указывает уровень доступа для категории конфиденциальности данных, к которому будет предоставлен указанного приложения к.</span><span class="sxs-lookup"><span data-stu-id="d631a-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="d631a-139">Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="d631a-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="d631a-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="d631a-140">dataCategory</span></span>|[<span data-ttu-id="d631a-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="d631a-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="d631a-142">Указывает категорию конфиденциальности данных, к которому будет применяться контроля доступа к определенным.</span><span class="sxs-lookup"><span data-stu-id="d631a-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="d631a-143">Возможные значения: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices` .</span><span class="sxs-lookup"><span data-stu-id="d631a-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="d631a-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="d631a-144">appPackageFamilyName</span></span>|<span data-ttu-id="d631a-145">String.</span><span class="sxs-lookup"><span data-stu-id="d631a-145">String</span></span>|<span data-ttu-id="d631a-146">Имя семейства пакет приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="d631a-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="d631a-147">Если задано, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="d631a-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="d631a-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="d631a-148">appDisplayName</span></span>|<span data-ttu-id="d631a-149">String.</span><span class="sxs-lookup"><span data-stu-id="d631a-149">String</span></span>|<span data-ttu-id="d631a-150">Имя семейства пакет приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="d631a-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="d631a-151">Если задано, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="d631a-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="d631a-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="d631a-152">Response</span></span>
<span data-ttu-id="d631a-153">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d631a-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d631a-154">Пример</span><span class="sxs-lookup"><span data-stu-id="d631a-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="d631a-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="d631a-155">Request</span></span>
<span data-ttu-id="d631a-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d631a-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d631a-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="d631a-157">Response</span></span>
<span data-ttu-id="d631a-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d631a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






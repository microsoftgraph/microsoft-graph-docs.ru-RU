---
title: Тип ресурса intuneBrand
description: Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d31b4ab9931fd0693776646161528aa73e31205e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527726"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="c2e37-103">Тип ресурса intuneBrand</span><span class="sxs-lookup"><span data-stu-id="c2e37-103">intuneBrand resource type</span></span>

<span data-ttu-id="c2e37-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c2e37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2e37-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2e37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2e37-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2e37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2e37-107">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2e37-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="c2e37-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2e37-108">Properties</span></span>
|<span data-ttu-id="c2e37-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2e37-109">Property</span></span>|<span data-ttu-id="c2e37-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c2e37-110">Type</span></span>|<span data-ttu-id="c2e37-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c2e37-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2e37-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c2e37-112">displayName</span></span>|<span data-ttu-id="c2e37-113">String</span><span class="sxs-lookup"><span data-stu-id="c2e37-113">String</span></span>|<span data-ttu-id="c2e37-114">Название компании или организации, которое отображается пользователям.</span><span class="sxs-lookup"><span data-stu-id="c2e37-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="c2e37-115">themeColor</span><span class="sxs-lookup"><span data-stu-id="c2e37-115">themeColor</span></span>|[<span data-ttu-id="c2e37-116">rgbColor</span><span class="sxs-lookup"><span data-stu-id="c2e37-116">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="c2e37-117">Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.</span><span class="sxs-lookup"><span data-stu-id="c2e37-117">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="c2e37-118">showLogo</span><span class="sxs-lookup"><span data-stu-id="c2e37-118">showLogo</span></span>|<span data-ttu-id="c2e37-119">Логический</span><span class="sxs-lookup"><span data-stu-id="c2e37-119">Boolean</span></span>|<span data-ttu-id="c2e37-120">Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.</span><span class="sxs-lookup"><span data-stu-id="c2e37-120">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="c2e37-121">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="c2e37-121">lightBackgroundLogo</span></span>|<span data-ttu-id="c2e37-122">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="c2e37-122">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="c2e37-123">Изображение с логотипом на светлом фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="c2e37-123">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="c2e37-124">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="c2e37-124">darkBackgroundLogo</span></span>|[<span data-ttu-id="c2e37-125">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c2e37-125">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c2e37-126">Изображение с логотипом на темном фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="c2e37-126">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="c2e37-127">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="c2e37-127">showNameNextToLogo</span></span>|<span data-ttu-id="c2e37-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2e37-128">Boolean</span></span>|<span data-ttu-id="c2e37-129">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c2e37-129">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="c2e37-130">ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="c2e37-130">landingPageCustomizedImage</span></span>|<span data-ttu-id="c2e37-131">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="c2e37-131">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="c2e37-132">Настраиваемое изображение, отображаемое на начальной странице приложения корпоративного портала</span><span class="sxs-lookup"><span data-stu-id="c2e37-132">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="c2e37-133">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="c2e37-133">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="c2e37-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2e37-134">Boolean</span></span>|<span data-ttu-id="c2e37-135">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c2e37-135">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="c2e37-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c2e37-136">roleScopeTagIds</span></span>|<span data-ttu-id="c2e37-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c2e37-137">String collection</span></span>|<span data-ttu-id="c2e37-138">Список тегов областей, назначенных профилю фирменной символики по умолчанию</span><span class="sxs-lookup"><span data-stu-id="c2e37-138">List of scope tags assigned to the default branding profile</span></span>|
|<span data-ttu-id="c2e37-139">contactITName</span><span class="sxs-lookup"><span data-stu-id="c2e37-139">contactITName</span></span>|<span data-ttu-id="c2e37-140">String</span><span class="sxs-lookup"><span data-stu-id="c2e37-140">String</span></span>|<span data-ttu-id="c2e37-141">Имя пользователя или название организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="c2e37-141">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c2e37-142">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="c2e37-142">contactITPhoneNumber</span></span>|<span data-ttu-id="c2e37-143">String</span><span class="sxs-lookup"><span data-stu-id="c2e37-143">String</span></span>|<span data-ttu-id="c2e37-144">Номер телефона пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="c2e37-144">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c2e37-145">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c2e37-145">contactITEmailAddress</span></span>|<span data-ttu-id="c2e37-146">String</span><span class="sxs-lookup"><span data-stu-id="c2e37-146">String</span></span>|<span data-ttu-id="c2e37-147">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="c2e37-147">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c2e37-148">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="c2e37-148">contactITNotes</span></span>|<span data-ttu-id="c2e37-149">String</span><span class="sxs-lookup"><span data-stu-id="c2e37-149">String</span></span>|<span data-ttu-id="c2e37-150">Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="c2e37-150">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c2e37-151">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="c2e37-151">onlineSupportSiteUrl</span></span>|<span data-ttu-id="c2e37-152">String</span><span class="sxs-lookup"><span data-stu-id="c2e37-152">String</span></span>|<span data-ttu-id="c2e37-153">URL-адрес сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="c2e37-153">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="c2e37-154">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="c2e37-154">onlineSupportSiteName</span></span>|<span data-ttu-id="c2e37-155">String</span><span class="sxs-lookup"><span data-stu-id="c2e37-155">String</span></span>|<span data-ttu-id="c2e37-156">Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="c2e37-156">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="c2e37-157">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="c2e37-157">privacyUrl</span></span>|<span data-ttu-id="c2e37-158">String</span><span class="sxs-lookup"><span data-stu-id="c2e37-158">String</span></span>|<span data-ttu-id="c2e37-159">URL-адрес страницы с политикой конфиденциальности компании или организации.</span><span class="sxs-lookup"><span data-stu-id="c2e37-159">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="c2e37-160">кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="c2e37-160">customPrivacyMessage</span></span>|<span data-ttu-id="c2e37-161">String</span><span class="sxs-lookup"><span data-stu-id="c2e37-161">String</span></span>|<span data-ttu-id="c2e37-162">Пользовательское сообщение о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c2e37-162">Custom privacy message.</span></span>|
|<span data-ttu-id="c2e37-163">исремоведевицедисаблед</span><span class="sxs-lookup"><span data-stu-id="c2e37-163">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="c2e37-164">Логический</span><span class="sxs-lookup"><span data-stu-id="c2e37-164">Boolean</span></span>|<span data-ttu-id="c2e37-165">Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="c2e37-165">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="c2e37-166">исфакториресетдисаблед</span><span class="sxs-lookup"><span data-stu-id="c2e37-166">isFactoryResetDisabled</span></span>|<span data-ttu-id="c2e37-167">Логический</span><span class="sxs-lookup"><span data-stu-id="c2e37-167">Boolean</span></span>|<span data-ttu-id="c2e37-168">Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="c2e37-168">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="c2e37-169">компанипорталблоккедактионс</span><span class="sxs-lookup"><span data-stu-id="c2e37-169">companyPortalBlockedActions</span></span>|<span data-ttu-id="c2e37-170">Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="c2e37-170">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="c2e37-171">Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="c2e37-171">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="c2e37-172">шовазуреадентерприсеаппс</span><span class="sxs-lookup"><span data-stu-id="c2e37-172">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="c2e37-173">Логический</span><span class="sxs-lookup"><span data-stu-id="c2e37-173">Boolean</span></span>|<span data-ttu-id="c2e37-174">Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.</span><span class="sxs-lookup"><span data-stu-id="c2e37-174">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="c2e37-175">шовоффицевебаппс</span><span class="sxs-lookup"><span data-stu-id="c2e37-175">showOfficeWebApps</span></span>|<span data-ttu-id="c2e37-176">Логический</span><span class="sxs-lookup"><span data-stu-id="c2e37-176">Boolean</span></span>|<span data-ttu-id="c2e37-177">Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.</span><span class="sxs-lookup"><span data-stu-id="c2e37-177">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="c2e37-178">сенддевицеовнершипчанжепушнотификатион</span><span class="sxs-lookup"><span data-stu-id="c2e37-178">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="c2e37-179">Логический</span><span class="sxs-lookup"><span data-stu-id="c2e37-179">Boolean</span></span>|<span data-ttu-id="c2e37-180">Логическое значение, указывающее, отправляются ли пользователям push-уведомления, если их тип собственности изменяется от персонального к корпоративному.</span><span class="sxs-lookup"><span data-stu-id="c2e37-180">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="c2e37-181">енроллментаваилабилити</span><span class="sxs-lookup"><span data-stu-id="c2e37-181">enrollmentAvailability</span></span>|[<span data-ttu-id="c2e37-182">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="c2e37-182">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="c2e37-183">Настраиваемый процесс регистрации устройства, отображаемый для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2e37-183">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="c2e37-184">Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="c2e37-184">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2e37-185">Связи</span><span class="sxs-lookup"><span data-stu-id="c2e37-185">Relationships</span></span>
<span data-ttu-id="c2e37-186">Нет</span><span class="sxs-lookup"><span data-stu-id="c2e37-186">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2e37-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2e37-187">JSON Representation</span></span>
<span data-ttu-id="c2e37-188">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2e37-188">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showDisplayNameNextToLogo": true,
  "roleScopeTagIds": [
    "String"
  ],
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String",
  "customPrivacyMessage": "String",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "String",
      "ownerType": "String",
      "action": "String"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "String"
}
```




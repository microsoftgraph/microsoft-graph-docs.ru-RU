---
title: Тип ресурса intuneBrand
description: Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 92b706fee0e1b0a6af0d877d040339416d9b78c4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455576"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="043c8-103">Тип ресурса intuneBrand</span><span class="sxs-lookup"><span data-stu-id="043c8-103">intuneBrand resource type</span></span>

<span data-ttu-id="043c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="043c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="043c8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="043c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="043c8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="043c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="043c8-107">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="043c8-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="043c8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="043c8-108">Properties</span></span>
|<span data-ttu-id="043c8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="043c8-109">Property</span></span>|<span data-ttu-id="043c8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="043c8-110">Type</span></span>|<span data-ttu-id="043c8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="043c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="043c8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="043c8-112">displayName</span></span>|<span data-ttu-id="043c8-113">String</span><span class="sxs-lookup"><span data-stu-id="043c8-113">String</span></span>|<span data-ttu-id="043c8-114">Название компании или организации, которое отображается пользователям.</span><span class="sxs-lookup"><span data-stu-id="043c8-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="043c8-115">themeColor</span><span class="sxs-lookup"><span data-stu-id="043c8-115">themeColor</span></span>|[<span data-ttu-id="043c8-116">rgbColor</span><span class="sxs-lookup"><span data-stu-id="043c8-116">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="043c8-117">Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.</span><span class="sxs-lookup"><span data-stu-id="043c8-117">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="043c8-118">showLogo</span><span class="sxs-lookup"><span data-stu-id="043c8-118">showLogo</span></span>|<span data-ttu-id="043c8-119">Логическое</span><span class="sxs-lookup"><span data-stu-id="043c8-119">Boolean</span></span>|<span data-ttu-id="043c8-120">Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.</span><span class="sxs-lookup"><span data-stu-id="043c8-120">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="043c8-121">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="043c8-121">lightBackgroundLogo</span></span>|<span data-ttu-id="043c8-122">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="043c8-122">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="043c8-123">Изображение с логотипом на светлом фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="043c8-123">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="043c8-124">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="043c8-124">darkBackgroundLogo</span></span>|[<span data-ttu-id="043c8-125">mimeContent</span><span class="sxs-lookup"><span data-stu-id="043c8-125">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="043c8-126">Изображение с логотипом на темном фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="043c8-126">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="043c8-127">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="043c8-127">showNameNextToLogo</span></span>|<span data-ttu-id="043c8-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="043c8-128">Boolean</span></span>|<span data-ttu-id="043c8-129">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="043c8-129">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="043c8-130">ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="043c8-130">landingPageCustomizedImage</span></span>|<span data-ttu-id="043c8-131">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="043c8-131">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="043c8-132">Настраиваемое изображение, отображаемое на начальной странице приложения корпоративного портала</span><span class="sxs-lookup"><span data-stu-id="043c8-132">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="043c8-133">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="043c8-133">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="043c8-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="043c8-134">Boolean</span></span>|<span data-ttu-id="043c8-135">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="043c8-135">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="043c8-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="043c8-136">roleScopeTagIds</span></span>|<span data-ttu-id="043c8-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="043c8-137">String collection</span></span>|<span data-ttu-id="043c8-138">Список тегов областей, назначенных профилю фирменной символики по умолчанию</span><span class="sxs-lookup"><span data-stu-id="043c8-138">List of scope tags assigned to the default branding profile</span></span>|
|<span data-ttu-id="043c8-139">contactITName</span><span class="sxs-lookup"><span data-stu-id="043c8-139">contactITName</span></span>|<span data-ttu-id="043c8-140">String</span><span class="sxs-lookup"><span data-stu-id="043c8-140">String</span></span>|<span data-ttu-id="043c8-141">Имя пользователя или название организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="043c8-141">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="043c8-142">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="043c8-142">contactITPhoneNumber</span></span>|<span data-ttu-id="043c8-143">String</span><span class="sxs-lookup"><span data-stu-id="043c8-143">String</span></span>|<span data-ttu-id="043c8-144">Номер телефона пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="043c8-144">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="043c8-145">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="043c8-145">contactITEmailAddress</span></span>|<span data-ttu-id="043c8-146">String</span><span class="sxs-lookup"><span data-stu-id="043c8-146">String</span></span>|<span data-ttu-id="043c8-147">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="043c8-147">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="043c8-148">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="043c8-148">contactITNotes</span></span>|<span data-ttu-id="043c8-149">String</span><span class="sxs-lookup"><span data-stu-id="043c8-149">String</span></span>|<span data-ttu-id="043c8-150">Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="043c8-150">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="043c8-151">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="043c8-151">onlineSupportSiteUrl</span></span>|<span data-ttu-id="043c8-152">String</span><span class="sxs-lookup"><span data-stu-id="043c8-152">String</span></span>|<span data-ttu-id="043c8-153">URL-адрес сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="043c8-153">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="043c8-154">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="043c8-154">onlineSupportSiteName</span></span>|<span data-ttu-id="043c8-155">String</span><span class="sxs-lookup"><span data-stu-id="043c8-155">String</span></span>|<span data-ttu-id="043c8-156">Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="043c8-156">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="043c8-157">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="043c8-157">privacyUrl</span></span>|<span data-ttu-id="043c8-158">String</span><span class="sxs-lookup"><span data-stu-id="043c8-158">String</span></span>|<span data-ttu-id="043c8-159">URL-адрес страницы с политикой конфиденциальности компании или организации.</span><span class="sxs-lookup"><span data-stu-id="043c8-159">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="043c8-160">кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="043c8-160">customPrivacyMessage</span></span>|<span data-ttu-id="043c8-161">String</span><span class="sxs-lookup"><span data-stu-id="043c8-161">String</span></span>|<span data-ttu-id="043c8-162">Пользовательское сообщение о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="043c8-162">Custom privacy message.</span></span>|
|<span data-ttu-id="043c8-163">исремоведевицедисаблед</span><span class="sxs-lookup"><span data-stu-id="043c8-163">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="043c8-164">Логическое</span><span class="sxs-lookup"><span data-stu-id="043c8-164">Boolean</span></span>|<span data-ttu-id="043c8-165">Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="043c8-165">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="043c8-166">исфакториресетдисаблед</span><span class="sxs-lookup"><span data-stu-id="043c8-166">isFactoryResetDisabled</span></span>|<span data-ttu-id="043c8-167">Логическое</span><span class="sxs-lookup"><span data-stu-id="043c8-167">Boolean</span></span>|<span data-ttu-id="043c8-168">Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="043c8-168">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="043c8-169">компанипорталблоккедактионс</span><span class="sxs-lookup"><span data-stu-id="043c8-169">companyPortalBlockedActions</span></span>|<span data-ttu-id="043c8-170">Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="043c8-170">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="043c8-171">Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="043c8-171">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="043c8-172">шовазуреадентерприсеаппс</span><span class="sxs-lookup"><span data-stu-id="043c8-172">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="043c8-173">Логическое</span><span class="sxs-lookup"><span data-stu-id="043c8-173">Boolean</span></span>|<span data-ttu-id="043c8-174">Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.</span><span class="sxs-lookup"><span data-stu-id="043c8-174">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="043c8-175">шовоффицевебаппс</span><span class="sxs-lookup"><span data-stu-id="043c8-175">showOfficeWebApps</span></span>|<span data-ttu-id="043c8-176">Логическое</span><span class="sxs-lookup"><span data-stu-id="043c8-176">Boolean</span></span>|<span data-ttu-id="043c8-177">Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.</span><span class="sxs-lookup"><span data-stu-id="043c8-177">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="043c8-178">сенддевицеовнершипчанжепушнотификатион</span><span class="sxs-lookup"><span data-stu-id="043c8-178">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="043c8-179">Логическое</span><span class="sxs-lookup"><span data-stu-id="043c8-179">Boolean</span></span>|<span data-ttu-id="043c8-180">Логическое значение, указывающее, отправляются ли пользователям push-уведомления, если их тип собственности изменяется от персонального к корпоративному.</span><span class="sxs-lookup"><span data-stu-id="043c8-180">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="043c8-181">енроллментаваилабилити</span><span class="sxs-lookup"><span data-stu-id="043c8-181">enrollmentAvailability</span></span>|[<span data-ttu-id="043c8-182">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="043c8-182">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="043c8-183">Настраиваемый процесс регистрации устройства, отображаемый для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="043c8-183">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="043c8-184">Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="043c8-184">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="043c8-185">Связи</span><span class="sxs-lookup"><span data-stu-id="043c8-185">Relationships</span></span>
<span data-ttu-id="043c8-186">Нет</span><span class="sxs-lookup"><span data-stu-id="043c8-186">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="043c8-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="043c8-187">JSON Representation</span></span>
<span data-ttu-id="043c8-188">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="043c8-188">Here is a JSON representation of the resource.</span></span>
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




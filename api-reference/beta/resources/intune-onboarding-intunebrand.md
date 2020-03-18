---
title: Тип ресурса intuneBrand
description: Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c50e0b3a55a3df4e1c1f71f9058f407a7f912516
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42778374"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="62856-103">Тип ресурса intuneBrand</span><span class="sxs-lookup"><span data-stu-id="62856-103">intuneBrand resource type</span></span>

> <span data-ttu-id="62856-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62856-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62856-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62856-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62856-106">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="62856-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="62856-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="62856-107">Properties</span></span>
|<span data-ttu-id="62856-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="62856-108">Property</span></span>|<span data-ttu-id="62856-109">Тип</span><span class="sxs-lookup"><span data-stu-id="62856-109">Type</span></span>|<span data-ttu-id="62856-110">Описание</span><span class="sxs-lookup"><span data-stu-id="62856-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62856-111">displayName</span><span class="sxs-lookup"><span data-stu-id="62856-111">displayName</span></span>|<span data-ttu-id="62856-112">String</span><span class="sxs-lookup"><span data-stu-id="62856-112">String</span></span>|<span data-ttu-id="62856-113">Название компании или организации, которое отображается пользователям.</span><span class="sxs-lookup"><span data-stu-id="62856-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="62856-114">themeColor</span><span class="sxs-lookup"><span data-stu-id="62856-114">themeColor</span></span>|[<span data-ttu-id="62856-115">rgbColor</span><span class="sxs-lookup"><span data-stu-id="62856-115">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="62856-116">Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.</span><span class="sxs-lookup"><span data-stu-id="62856-116">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="62856-117">showLogo</span><span class="sxs-lookup"><span data-stu-id="62856-117">showLogo</span></span>|<span data-ttu-id="62856-118">Логический</span><span class="sxs-lookup"><span data-stu-id="62856-118">Boolean</span></span>|<span data-ttu-id="62856-119">Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.</span><span class="sxs-lookup"><span data-stu-id="62856-119">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="62856-120">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="62856-120">lightBackgroundLogo</span></span>|<span data-ttu-id="62856-121">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="62856-121">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="62856-122">Изображение с логотипом на светлом фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="62856-122">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="62856-123">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="62856-123">darkBackgroundLogo</span></span>|[<span data-ttu-id="62856-124">mimeContent</span><span class="sxs-lookup"><span data-stu-id="62856-124">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="62856-125">Изображение с логотипом на темном фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="62856-125">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="62856-126">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="62856-126">showNameNextToLogo</span></span>|<span data-ttu-id="62856-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="62856-127">Boolean</span></span>|<span data-ttu-id="62856-128">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="62856-128">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="62856-129">ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="62856-129">landingPageCustomizedImage</span></span>|<span data-ttu-id="62856-130">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="62856-130">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="62856-131">Настраиваемое изображение, отображаемое на начальной странице приложения корпоративного портала</span><span class="sxs-lookup"><span data-stu-id="62856-131">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="62856-132">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="62856-132">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="62856-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="62856-133">Boolean</span></span>|<span data-ttu-id="62856-134">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="62856-134">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="62856-135">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62856-135">roleScopeTagIds</span></span>|<span data-ttu-id="62856-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="62856-136">String collection</span></span>|<span data-ttu-id="62856-137">Список тегов областей, назначенных профилю фирменной символики по умолчанию</span><span class="sxs-lookup"><span data-stu-id="62856-137">List of scope tags assigned to the default branding profile</span></span>|
|<span data-ttu-id="62856-138">contactITName</span><span class="sxs-lookup"><span data-stu-id="62856-138">contactITName</span></span>|<span data-ttu-id="62856-139">String</span><span class="sxs-lookup"><span data-stu-id="62856-139">String</span></span>|<span data-ttu-id="62856-140">Имя пользователя или название организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="62856-140">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="62856-141">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="62856-141">contactITPhoneNumber</span></span>|<span data-ttu-id="62856-142">String</span><span class="sxs-lookup"><span data-stu-id="62856-142">String</span></span>|<span data-ttu-id="62856-143">Номер телефона пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="62856-143">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="62856-144">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="62856-144">contactITEmailAddress</span></span>|<span data-ttu-id="62856-145">String</span><span class="sxs-lookup"><span data-stu-id="62856-145">String</span></span>|<span data-ttu-id="62856-146">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="62856-146">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="62856-147">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="62856-147">contactITNotes</span></span>|<span data-ttu-id="62856-148">String</span><span class="sxs-lookup"><span data-stu-id="62856-148">String</span></span>|<span data-ttu-id="62856-149">Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="62856-149">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="62856-150">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="62856-150">onlineSupportSiteUrl</span></span>|<span data-ttu-id="62856-151">String</span><span class="sxs-lookup"><span data-stu-id="62856-151">String</span></span>|<span data-ttu-id="62856-152">URL-адрес сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="62856-152">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="62856-153">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="62856-153">onlineSupportSiteName</span></span>|<span data-ttu-id="62856-154">String</span><span class="sxs-lookup"><span data-stu-id="62856-154">String</span></span>|<span data-ttu-id="62856-155">Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="62856-155">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="62856-156">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="62856-156">privacyUrl</span></span>|<span data-ttu-id="62856-157">String</span><span class="sxs-lookup"><span data-stu-id="62856-157">String</span></span>|<span data-ttu-id="62856-158">URL-адрес страницы с политикой конфиденциальности компании или организации.</span><span class="sxs-lookup"><span data-stu-id="62856-158">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="62856-159">кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="62856-159">customPrivacyMessage</span></span>|<span data-ttu-id="62856-160">String</span><span class="sxs-lookup"><span data-stu-id="62856-160">String</span></span>|<span data-ttu-id="62856-161">Пользовательское сообщение о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="62856-161">Custom privacy message.</span></span>|
|<span data-ttu-id="62856-162">исремоведевицедисаблед</span><span class="sxs-lookup"><span data-stu-id="62856-162">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="62856-163">Логический</span><span class="sxs-lookup"><span data-stu-id="62856-163">Boolean</span></span>|<span data-ttu-id="62856-164">Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="62856-164">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="62856-165">исфакториресетдисаблед</span><span class="sxs-lookup"><span data-stu-id="62856-165">isFactoryResetDisabled</span></span>|<span data-ttu-id="62856-166">Логический</span><span class="sxs-lookup"><span data-stu-id="62856-166">Boolean</span></span>|<span data-ttu-id="62856-167">Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="62856-167">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="62856-168">компанипорталблоккедактионс</span><span class="sxs-lookup"><span data-stu-id="62856-168">companyPortalBlockedActions</span></span>|<span data-ttu-id="62856-169">Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="62856-169">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="62856-170">Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="62856-170">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="62856-171">шовазуреадентерприсеаппс</span><span class="sxs-lookup"><span data-stu-id="62856-171">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="62856-172">Логический</span><span class="sxs-lookup"><span data-stu-id="62856-172">Boolean</span></span>|<span data-ttu-id="62856-173">Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.</span><span class="sxs-lookup"><span data-stu-id="62856-173">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="62856-174">шовоффицевебаппс</span><span class="sxs-lookup"><span data-stu-id="62856-174">showOfficeWebApps</span></span>|<span data-ttu-id="62856-175">Логический</span><span class="sxs-lookup"><span data-stu-id="62856-175">Boolean</span></span>|<span data-ttu-id="62856-176">Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.</span><span class="sxs-lookup"><span data-stu-id="62856-176">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="62856-177">сенддевицеовнершипчанжепушнотификатион</span><span class="sxs-lookup"><span data-stu-id="62856-177">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="62856-178">Логический</span><span class="sxs-lookup"><span data-stu-id="62856-178">Boolean</span></span>|<span data-ttu-id="62856-179">Логическое значение, указывающее, отправляются ли пользователям push-уведомления, если их тип собственности изменяется от персонального к корпоративному.</span><span class="sxs-lookup"><span data-stu-id="62856-179">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="62856-180">енроллментаваилабилити</span><span class="sxs-lookup"><span data-stu-id="62856-180">enrollmentAvailability</span></span>|[<span data-ttu-id="62856-181">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="62856-181">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="62856-182">Настраиваемый процесс регистрации устройства, отображаемый для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="62856-182">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="62856-183">Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="62856-183">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62856-184">Связи</span><span class="sxs-lookup"><span data-stu-id="62856-184">Relationships</span></span>
<span data-ttu-id="62856-185">Нет</span><span class="sxs-lookup"><span data-stu-id="62856-185">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62856-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62856-186">JSON Representation</span></span>
<span data-ttu-id="62856-187">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62856-187">Here is a JSON representation of the resource.</span></span>
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




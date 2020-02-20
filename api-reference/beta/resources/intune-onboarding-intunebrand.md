---
title: Тип ресурса intuneBrand
description: Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1b6b913f115ee73566a688a90355377a7ff495eb
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160349"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="4dddd-103">Тип ресурса intuneBrand</span><span class="sxs-lookup"><span data-stu-id="4dddd-103">intuneBrand resource type</span></span>

> <span data-ttu-id="4dddd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dddd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dddd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4dddd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dddd-106">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="4dddd-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="4dddd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4dddd-107">Properties</span></span>
|<span data-ttu-id="4dddd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dddd-108">Property</span></span>|<span data-ttu-id="4dddd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4dddd-109">Type</span></span>|<span data-ttu-id="4dddd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4dddd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dddd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4dddd-111">displayName</span></span>|<span data-ttu-id="4dddd-112">String</span><span class="sxs-lookup"><span data-stu-id="4dddd-112">String</span></span>|<span data-ttu-id="4dddd-113">Название компании или организации, которое отображается пользователям.</span><span class="sxs-lookup"><span data-stu-id="4dddd-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="4dddd-114">themeColor</span><span class="sxs-lookup"><span data-stu-id="4dddd-114">themeColor</span></span>|[<span data-ttu-id="4dddd-115">rgbColor</span><span class="sxs-lookup"><span data-stu-id="4dddd-115">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="4dddd-116">Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.</span><span class="sxs-lookup"><span data-stu-id="4dddd-116">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="4dddd-117">showLogo</span><span class="sxs-lookup"><span data-stu-id="4dddd-117">showLogo</span></span>|<span data-ttu-id="4dddd-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dddd-118">Boolean</span></span>|<span data-ttu-id="4dddd-119">Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.</span><span class="sxs-lookup"><span data-stu-id="4dddd-119">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="4dddd-120">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="4dddd-120">lightBackgroundLogo</span></span>|<span data-ttu-id="4dddd-121">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="4dddd-121">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="4dddd-122">Изображение с логотипом на светлом фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="4dddd-122">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="4dddd-123">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="4dddd-123">darkBackgroundLogo</span></span>|[<span data-ttu-id="4dddd-124">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4dddd-124">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4dddd-125">Изображение с логотипом на темном фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="4dddd-125">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="4dddd-126">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="4dddd-126">showNameNextToLogo</span></span>|<span data-ttu-id="4dddd-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dddd-127">Boolean</span></span>|<span data-ttu-id="4dddd-128">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="4dddd-128">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="4dddd-129">ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="4dddd-129">landingPageCustomizedImage</span></span>|<span data-ttu-id="4dddd-130">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="4dddd-130">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="4dddd-131">Настраиваемое изображение, отображаемое на начальной странице приложения корпоративного портала</span><span class="sxs-lookup"><span data-stu-id="4dddd-131">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="4dddd-132">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="4dddd-132">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="4dddd-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dddd-133">Boolean</span></span>|<span data-ttu-id="4dddd-134">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="4dddd-134">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="4dddd-135">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4dddd-135">roleScopeTagIds</span></span>|<span data-ttu-id="4dddd-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4dddd-136">String collection</span></span>|<span data-ttu-id="4dddd-137">Список тегов областей, назначенных профилю фирменной символики по умолчанию</span><span class="sxs-lookup"><span data-stu-id="4dddd-137">List of scope tags assigned to the default branding profile</span></span>|
|<span data-ttu-id="4dddd-138">contactITName</span><span class="sxs-lookup"><span data-stu-id="4dddd-138">contactITName</span></span>|<span data-ttu-id="4dddd-139">String</span><span class="sxs-lookup"><span data-stu-id="4dddd-139">String</span></span>|<span data-ttu-id="4dddd-140">Имя пользователя или название организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="4dddd-140">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="4dddd-141">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="4dddd-141">contactITPhoneNumber</span></span>|<span data-ttu-id="4dddd-142">String</span><span class="sxs-lookup"><span data-stu-id="4dddd-142">String</span></span>|<span data-ttu-id="4dddd-143">Номер телефона пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="4dddd-143">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="4dddd-144">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="4dddd-144">contactITEmailAddress</span></span>|<span data-ttu-id="4dddd-145">String</span><span class="sxs-lookup"><span data-stu-id="4dddd-145">String</span></span>|<span data-ttu-id="4dddd-146">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="4dddd-146">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="4dddd-147">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="4dddd-147">contactITNotes</span></span>|<span data-ttu-id="4dddd-148">String</span><span class="sxs-lookup"><span data-stu-id="4dddd-148">String</span></span>|<span data-ttu-id="4dddd-149">Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="4dddd-149">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="4dddd-150">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="4dddd-150">onlineSupportSiteUrl</span></span>|<span data-ttu-id="4dddd-151">String</span><span class="sxs-lookup"><span data-stu-id="4dddd-151">String</span></span>|<span data-ttu-id="4dddd-152">URL-адрес сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="4dddd-152">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="4dddd-153">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="4dddd-153">onlineSupportSiteName</span></span>|<span data-ttu-id="4dddd-154">String</span><span class="sxs-lookup"><span data-stu-id="4dddd-154">String</span></span>|<span data-ttu-id="4dddd-155">Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="4dddd-155">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="4dddd-156">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="4dddd-156">privacyUrl</span></span>|<span data-ttu-id="4dddd-157">String</span><span class="sxs-lookup"><span data-stu-id="4dddd-157">String</span></span>|<span data-ttu-id="4dddd-158">URL-адрес страницы с политикой конфиденциальности компании или организации.</span><span class="sxs-lookup"><span data-stu-id="4dddd-158">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="4dddd-159">кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="4dddd-159">customPrivacyMessage</span></span>|<span data-ttu-id="4dddd-160">String</span><span class="sxs-lookup"><span data-stu-id="4dddd-160">String</span></span>|<span data-ttu-id="4dddd-161">Пользовательское сообщение о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4dddd-161">Custom privacy message.</span></span>|
|<span data-ttu-id="4dddd-162">исремоведевицедисаблед</span><span class="sxs-lookup"><span data-stu-id="4dddd-162">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="4dddd-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dddd-163">Boolean</span></span>|<span data-ttu-id="4dddd-164">Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="4dddd-164">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="4dddd-165">исфакториресетдисаблед</span><span class="sxs-lookup"><span data-stu-id="4dddd-165">isFactoryResetDisabled</span></span>|<span data-ttu-id="4dddd-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dddd-166">Boolean</span></span>|<span data-ttu-id="4dddd-167">Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="4dddd-167">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="4dddd-168">компанипорталблоккедактионс</span><span class="sxs-lookup"><span data-stu-id="4dddd-168">companyPortalBlockedActions</span></span>|<span data-ttu-id="4dddd-169">Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="4dddd-169">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="4dddd-170">Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="4dddd-170">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="4dddd-171">шовазуреадентерприсеаппс</span><span class="sxs-lookup"><span data-stu-id="4dddd-171">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="4dddd-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dddd-172">Boolean</span></span>|<span data-ttu-id="4dddd-173">Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.</span><span class="sxs-lookup"><span data-stu-id="4dddd-173">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="4dddd-174">шовоффицевебаппс</span><span class="sxs-lookup"><span data-stu-id="4dddd-174">showOfficeWebApps</span></span>|<span data-ttu-id="4dddd-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dddd-175">Boolean</span></span>|<span data-ttu-id="4dddd-176">Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.</span><span class="sxs-lookup"><span data-stu-id="4dddd-176">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="4dddd-177">сенддевицеовнершипчанжепушнотификатион</span><span class="sxs-lookup"><span data-stu-id="4dddd-177">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="4dddd-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dddd-178">Boolean</span></span>|<span data-ttu-id="4dddd-179">Логическое значение, указывающее, отправляются ли пользователям push-уведомления, если их тип собственности изменяется от персонального к корпоративному.</span><span class="sxs-lookup"><span data-stu-id="4dddd-179">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="4dddd-180">енроллментаваилабилити</span><span class="sxs-lookup"><span data-stu-id="4dddd-180">enrollmentAvailability</span></span>|[<span data-ttu-id="4dddd-181">енроллментаваилабилитйоптионс</span><span class="sxs-lookup"><span data-stu-id="4dddd-181">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="4dddd-182">Настраиваемый процесс регистрации устройства, отображаемый для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4dddd-182">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="4dddd-183">Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="4dddd-183">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dddd-184">Отношения</span><span class="sxs-lookup"><span data-stu-id="4dddd-184">Relationships</span></span>
<span data-ttu-id="4dddd-185">Нет</span><span class="sxs-lookup"><span data-stu-id="4dddd-185">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dddd-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4dddd-186">JSON Representation</span></span>
<span data-ttu-id="4dddd-187">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dddd-187">Here is a JSON representation of the resource.</span></span>
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




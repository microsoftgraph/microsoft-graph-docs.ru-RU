---
title: Тип ресурса intuneBrand
description: Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d97ecb5a0cb55ca717da3ceb6870d71c70df199a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266531"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="71bb9-103">Тип ресурса intuneBrand</span><span class="sxs-lookup"><span data-stu-id="71bb9-103">intuneBrand resource type</span></span>

<span data-ttu-id="71bb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71bb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71bb9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71bb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71bb9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71bb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71bb9-107">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="71bb9-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="71bb9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="71bb9-108">Properties</span></span>
|<span data-ttu-id="71bb9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="71bb9-109">Property</span></span>|<span data-ttu-id="71bb9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="71bb9-110">Type</span></span>|<span data-ttu-id="71bb9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="71bb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71bb9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="71bb9-112">displayName</span></span>|<span data-ttu-id="71bb9-113">String</span><span class="sxs-lookup"><span data-stu-id="71bb9-113">String</span></span>|<span data-ttu-id="71bb9-114">Название компании или организации, которое отображается пользователям.</span><span class="sxs-lookup"><span data-stu-id="71bb9-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="71bb9-115">themeColor</span><span class="sxs-lookup"><span data-stu-id="71bb9-115">themeColor</span></span>|[<span data-ttu-id="71bb9-116">rgbColor</span><span class="sxs-lookup"><span data-stu-id="71bb9-116">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="71bb9-117">Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.</span><span class="sxs-lookup"><span data-stu-id="71bb9-117">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="71bb9-118">showLogo</span><span class="sxs-lookup"><span data-stu-id="71bb9-118">showLogo</span></span>|<span data-ttu-id="71bb9-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="71bb9-119">Boolean</span></span>|<span data-ttu-id="71bb9-120">Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.</span><span class="sxs-lookup"><span data-stu-id="71bb9-120">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="71bb9-121">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="71bb9-121">lightBackgroundLogo</span></span>|[<span data-ttu-id="71bb9-122">mimeContent</span><span class="sxs-lookup"><span data-stu-id="71bb9-122">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="71bb9-123">Изображение с логотипом на светлом фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="71bb9-123">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="71bb9-124">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="71bb9-124">darkBackgroundLogo</span></span>|[<span data-ttu-id="71bb9-125">mimeContent</span><span class="sxs-lookup"><span data-stu-id="71bb9-125">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="71bb9-126">Изображение с логотипом на темном фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="71bb9-126">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="71bb9-127">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="71bb9-127">showNameNextToLogo</span></span>|<span data-ttu-id="71bb9-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="71bb9-128">Boolean</span></span>|<span data-ttu-id="71bb9-129">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="71bb9-129">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="71bb9-130">ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="71bb9-130">landingPageCustomizedImage</span></span>|<span data-ttu-id="71bb9-131">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="71bb9-131">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="71bb9-132">Настраиваемое изображение, отображаемое на начальной странице приложения корпоративного портала</span><span class="sxs-lookup"><span data-stu-id="71bb9-132">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="71bb9-133">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="71bb9-133">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="71bb9-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="71bb9-134">Boolean</span></span>|<span data-ttu-id="71bb9-135">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="71bb9-135">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="71bb9-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71bb9-136">roleScopeTagIds</span></span>|<span data-ttu-id="71bb9-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="71bb9-137">String collection</span></span>|<span data-ttu-id="71bb9-138">Список тегов областей, назначенных профилю фирменной символики по умолчанию</span><span class="sxs-lookup"><span data-stu-id="71bb9-138">List of scope tags assigned to the default branding profile</span></span>|
|<span data-ttu-id="71bb9-139">contactITName</span><span class="sxs-lookup"><span data-stu-id="71bb9-139">contactITName</span></span>|<span data-ttu-id="71bb9-140">String</span><span class="sxs-lookup"><span data-stu-id="71bb9-140">String</span></span>|<span data-ttu-id="71bb9-141">Имя пользователя или название организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="71bb9-141">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="71bb9-142">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="71bb9-142">contactITPhoneNumber</span></span>|<span data-ttu-id="71bb9-143">String</span><span class="sxs-lookup"><span data-stu-id="71bb9-143">String</span></span>|<span data-ttu-id="71bb9-144">Номер телефона пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="71bb9-144">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="71bb9-145">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="71bb9-145">contactITEmailAddress</span></span>|<span data-ttu-id="71bb9-146">String</span><span class="sxs-lookup"><span data-stu-id="71bb9-146">String</span></span>|<span data-ttu-id="71bb9-147">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="71bb9-147">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="71bb9-148">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="71bb9-148">contactITNotes</span></span>|<span data-ttu-id="71bb9-149">String</span><span class="sxs-lookup"><span data-stu-id="71bb9-149">String</span></span>|<span data-ttu-id="71bb9-150">Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="71bb9-150">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="71bb9-151">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="71bb9-151">onlineSupportSiteUrl</span></span>|<span data-ttu-id="71bb9-152">String</span><span class="sxs-lookup"><span data-stu-id="71bb9-152">String</span></span>|<span data-ttu-id="71bb9-153">URL-адрес сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="71bb9-153">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="71bb9-154">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="71bb9-154">onlineSupportSiteName</span></span>|<span data-ttu-id="71bb9-155">String</span><span class="sxs-lookup"><span data-stu-id="71bb9-155">String</span></span>|<span data-ttu-id="71bb9-156">Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="71bb9-156">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="71bb9-157">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="71bb9-157">privacyUrl</span></span>|<span data-ttu-id="71bb9-158">String</span><span class="sxs-lookup"><span data-stu-id="71bb9-158">String</span></span>|<span data-ttu-id="71bb9-159">URL-адрес страницы с политикой конфиденциальности компании или организации.</span><span class="sxs-lookup"><span data-stu-id="71bb9-159">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="71bb9-160">кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="71bb9-160">customPrivacyMessage</span></span>|<span data-ttu-id="71bb9-161">String</span><span class="sxs-lookup"><span data-stu-id="71bb9-161">String</span></span>|<span data-ttu-id="71bb9-162">Настраиваемое сообщение о конфиденциальности, используемое для объяснения того, что Организация не может просматривать или делать на управляемых устройствах.</span><span class="sxs-lookup"><span data-stu-id="71bb9-162">The custom privacy message used to explain what the organization can’t see or do on managed devices.</span></span>|
|<span data-ttu-id="71bb9-163">кустомкантсипривацимессаже</span><span class="sxs-lookup"><span data-stu-id="71bb9-163">customCantSeePrivacyMessage</span></span>|<span data-ttu-id="71bb9-164">String</span><span class="sxs-lookup"><span data-stu-id="71bb9-164">String</span></span>|<span data-ttu-id="71bb9-165">Настраиваемое сообщение о конфиденциальности, используемое для объяснения того, что Организация не может просматривать или делать на управляемых устройствах.</span><span class="sxs-lookup"><span data-stu-id="71bb9-165">The custom privacy message used to explain what the organization can’t see or do on managed devices.</span></span>|
|<span data-ttu-id="71bb9-166">кустомкансипривацимессаже</span><span class="sxs-lookup"><span data-stu-id="71bb9-166">customCanSeePrivacyMessage</span></span>|<span data-ttu-id="71bb9-167">String</span><span class="sxs-lookup"><span data-stu-id="71bb9-167">String</span></span>|<span data-ttu-id="71bb9-168">Настраиваемое сообщение о конфиденциальности, используемое для объяснения того, что Организация может просматривать и выполнять на управляемых устройствах.</span><span class="sxs-lookup"><span data-stu-id="71bb9-168">The custom privacy message used to explain what the organization can see and do on managed devices.</span></span>|
|<span data-ttu-id="71bb9-169">исремоведевицедисаблед</span><span class="sxs-lookup"><span data-stu-id="71bb9-169">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="71bb9-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="71bb9-170">Boolean</span></span>|<span data-ttu-id="71bb9-171">Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="71bb9-171">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="71bb9-172">исфакториресетдисаблед</span><span class="sxs-lookup"><span data-stu-id="71bb9-172">isFactoryResetDisabled</span></span>|<span data-ttu-id="71bb9-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="71bb9-173">Boolean</span></span>|<span data-ttu-id="71bb9-174">Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="71bb9-174">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="71bb9-175">компанипорталблоккедактионс</span><span class="sxs-lookup"><span data-stu-id="71bb9-175">companyPortalBlockedActions</span></span>|<span data-ttu-id="71bb9-176">Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="71bb9-176">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="71bb9-177">Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="71bb9-177">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="71bb9-178">шовазуреадентерприсеаппс</span><span class="sxs-lookup"><span data-stu-id="71bb9-178">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="71bb9-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="71bb9-179">Boolean</span></span>|<span data-ttu-id="71bb9-180">Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.</span><span class="sxs-lookup"><span data-stu-id="71bb9-180">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="71bb9-181">шовоффицевебаппс</span><span class="sxs-lookup"><span data-stu-id="71bb9-181">showOfficeWebApps</span></span>|<span data-ttu-id="71bb9-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="71bb9-182">Boolean</span></span>|<span data-ttu-id="71bb9-183">Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.</span><span class="sxs-lookup"><span data-stu-id="71bb9-183">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="71bb9-184">сенддевицеовнершипчанжепушнотификатион</span><span class="sxs-lookup"><span data-stu-id="71bb9-184">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="71bb9-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="71bb9-185">Boolean</span></span>|<span data-ttu-id="71bb9-186">Логическое значение, указывающее, отправляются ли пользователям push-уведомления, если их тип собственности изменяется от персонального к корпоративному.</span><span class="sxs-lookup"><span data-stu-id="71bb9-186">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="71bb9-187">енроллментаваилабилити</span><span class="sxs-lookup"><span data-stu-id="71bb9-187">enrollmentAvailability</span></span>|[<span data-ttu-id="71bb9-188">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="71bb9-188">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="71bb9-189">Настраиваемый процесс регистрации устройства, отображаемый для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="71bb9-189">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="71bb9-190">Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="71bb9-190">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="71bb9-191">дисаблеклиенттелеметри</span><span class="sxs-lookup"><span data-stu-id="71bb9-191">disableClientTelemetry</span></span>|<span data-ttu-id="71bb9-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="71bb9-192">Boolean</span></span>|<span data-ttu-id="71bb9-193">Применяется к телеметрии, отправляемой со всех клиентов в службу Intune.</span><span class="sxs-lookup"><span data-stu-id="71bb9-193">Applies to telemetry sent from all clients to the Intune service.</span></span> <span data-ttu-id="71bb9-194">Если этот параметр отключен, все предупреждения об устранении неполадок и неполадки в клиенте отключаются, и параметры телеметрии отображаются как неактивные или скрытые для пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="71bb9-194">When disabled, all proactive troubleshooting and issue warnings within the client are turned off, and telemetry settings appear inactive or hidden to the device user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71bb9-195">Связи</span><span class="sxs-lookup"><span data-stu-id="71bb9-195">Relationships</span></span>
<span data-ttu-id="71bb9-196">Нет</span><span class="sxs-lookup"><span data-stu-id="71bb9-196">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71bb9-197">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71bb9-197">JSON Representation</span></span>
<span data-ttu-id="71bb9-198">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71bb9-198">Here is a JSON representation of the resource.</span></span>
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
  "customCantSeePrivacyMessage": "String",
  "customCanSeePrivacyMessage": "String",
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
  "enrollmentAvailability": "String",
  "disableClientTelemetry": true
}
```





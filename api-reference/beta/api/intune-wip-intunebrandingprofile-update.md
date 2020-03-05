---
title: Обновление Интунебрандингпрофиле
description: Обновление свойств объекта Интунебрандингпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1a2bb95404c3976b8702e752b5d9d17ad3872191
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457428"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="730a0-103">Обновление Интунебрандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="730a0-103">Update intuneBrandingProfile</span></span>

<span data-ttu-id="730a0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="730a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="730a0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="730a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="730a0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="730a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="730a0-107">Обновление свойств объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="730a0-107">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="730a0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="730a0-108">Prerequisites</span></span>
<span data-ttu-id="730a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="730a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="730a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="730a0-111">Permission type</span></span>|<span data-ttu-id="730a0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="730a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="730a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="730a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="730a0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="730a0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="730a0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="730a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="730a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="730a0-116">Not supported.</span></span>|
|<span data-ttu-id="730a0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="730a0-117">Application</span></span>|<span data-ttu-id="730a0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="730a0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="730a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="730a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="730a0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="730a0-120">Request headers</span></span>
|<span data-ttu-id="730a0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="730a0-121">Header</span></span>|<span data-ttu-id="730a0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="730a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="730a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="730a0-123">Authorization</span></span>|<span data-ttu-id="730a0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="730a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="730a0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="730a0-125">Accept</span></span>|<span data-ttu-id="730a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="730a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="730a0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="730a0-127">Request body</span></span>
<span data-ttu-id="730a0-128">В тексте запроса добавьте представление объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="730a0-128">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="730a0-129">В следующей таблице приведены свойства, необходимые при создании [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="730a0-129">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="730a0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="730a0-130">Property</span></span>|<span data-ttu-id="730a0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="730a0-131">Type</span></span>|<span data-ttu-id="730a0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="730a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="730a0-133">id</span><span class="sxs-lookup"><span data-stu-id="730a0-133">id</span></span>|<span data-ttu-id="730a0-134">String</span><span class="sxs-lookup"><span data-stu-id="730a0-134">String</span></span>|<span data-ttu-id="730a0-135">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="730a0-135">Profile Key</span></span>|
|<span data-ttu-id="730a0-136">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="730a0-136">profileName</span></span>|<span data-ttu-id="730a0-137">String</span><span class="sxs-lookup"><span data-stu-id="730a0-137">String</span></span>|<span data-ttu-id="730a0-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="730a0-138">Name of the profile</span></span>|
|<span data-ttu-id="730a0-139">профиледескриптион</span><span class="sxs-lookup"><span data-stu-id="730a0-139">profileDescription</span></span>|<span data-ttu-id="730a0-140">String</span><span class="sxs-lookup"><span data-stu-id="730a0-140">String</span></span>|<span data-ttu-id="730a0-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="730a0-141">Description of the profile</span></span>|
|<span data-ttu-id="730a0-142">исдефаултпрофиле</span><span class="sxs-lookup"><span data-stu-id="730a0-142">isDefaultProfile</span></span>|<span data-ttu-id="730a0-143">Логический</span><span class="sxs-lookup"><span data-stu-id="730a0-143">Boolean</span></span>|<span data-ttu-id="730a0-144">Логическое значение, указывающее, используется ли профиль по умолчанию или нет</span><span class="sxs-lookup"><span data-stu-id="730a0-144">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="730a0-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="730a0-145">createdDateTime</span></span>|<span data-ttu-id="730a0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="730a0-146">DateTimeOffset</span></span>|<span data-ttu-id="730a0-147">Время создания Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="730a0-147">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="730a0-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="730a0-148">lastModifiedDateTime</span></span>|<span data-ttu-id="730a0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="730a0-149">DateTimeOffset</span></span>|<span data-ttu-id="730a0-150">Время последнего изменения Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="730a0-150">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="730a0-151">displayName</span><span class="sxs-lookup"><span data-stu-id="730a0-151">displayName</span></span>|<span data-ttu-id="730a0-152">Строка</span><span class="sxs-lookup"><span data-stu-id="730a0-152">String</span></span>|<span data-ttu-id="730a0-153">Название компании или организации, которое отображается для конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="730a0-153">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="730a0-154">themeColor</span><span class="sxs-lookup"><span data-stu-id="730a0-154">themeColor</span></span>|[<span data-ttu-id="730a0-155">rgbColor</span><span class="sxs-lookup"><span data-stu-id="730a0-155">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="730a0-156">Основной цвет темы, используемый в приложениях портала компании и на веб-портале</span><span class="sxs-lookup"><span data-stu-id="730a0-156">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="730a0-157">showLogo</span><span class="sxs-lookup"><span data-stu-id="730a0-157">showLogo</span></span>|<span data-ttu-id="730a0-158">Логический</span><span class="sxs-lookup"><span data-stu-id="730a0-158">Boolean</span></span>|<span data-ttu-id="730a0-159">Логическое значение, указывающее, отображаются ли изображения логотипа, предоставленные администратором.</span><span class="sxs-lookup"><span data-stu-id="730a0-159">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="730a0-160">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="730a0-160">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="730a0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="730a0-161">Boolean</span></span>|<span data-ttu-id="730a0-162">Логическое значение, указывающее, будет ли отображаться отображаемое имя, предоставленное администратором, рядом с изображением логотипа.</span><span class="sxs-lookup"><span data-stu-id="730a0-162">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="730a0-163">семеколорлого</span><span class="sxs-lookup"><span data-stu-id="730a0-163">themeColorLogo</span></span>|<span data-ttu-id="730a0-164">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="730a0-164">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="730a0-165">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть фоновый цвет темы позади логотипа</span><span class="sxs-lookup"><span data-stu-id="730a0-165">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="730a0-166">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="730a0-166">lightBackgroundLogo</span></span>|[<span data-ttu-id="730a0-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="730a0-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="730a0-168">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть светлый фон позади логотипа</span><span class="sxs-lookup"><span data-stu-id="730a0-168">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="730a0-169">ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="730a0-169">landingPageCustomizedImage</span></span>|<span data-ttu-id="730a0-170">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="730a0-170">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="730a0-171">Настраиваемое изображение, отображаемое на начальной странице "приложения корпоративного портала"</span><span class="sxs-lookup"><span data-stu-id="730a0-171">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="730a0-172">contactITName</span><span class="sxs-lookup"><span data-stu-id="730a0-172">contactITName</span></span>|<span data-ttu-id="730a0-173">String</span><span class="sxs-lookup"><span data-stu-id="730a0-173">String</span></span>|<span data-ttu-id="730a0-174">Имя пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="730a0-174">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="730a0-175">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="730a0-175">contactITPhoneNumber</span></span>|<span data-ttu-id="730a0-176">String</span><span class="sxs-lookup"><span data-stu-id="730a0-176">String</span></span>|<span data-ttu-id="730a0-177">Номер телефона пользователя или организации, ответственного за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="730a0-177">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="730a0-178">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="730a0-178">contactITEmailAddress</span></span>|<span data-ttu-id="730a0-179">String</span><span class="sxs-lookup"><span data-stu-id="730a0-179">String</span></span>|<span data-ttu-id="730a0-180">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="730a0-180">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="730a0-181">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="730a0-181">contactITNotes</span></span>|<span data-ttu-id="730a0-182">String</span><span class="sxs-lookup"><span data-stu-id="730a0-182">String</span></span>|<span data-ttu-id="730a0-183">Текстовые комментарии о лице или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="730a0-183">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="730a0-184">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="730a0-184">onlineSupportSiteUrl</span></span>|<span data-ttu-id="730a0-185">String</span><span class="sxs-lookup"><span data-stu-id="730a0-185">String</span></span>|<span data-ttu-id="730a0-186">URL-адрес сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="730a0-186">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="730a0-187">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="730a0-187">onlineSupportSiteName</span></span>|<span data-ttu-id="730a0-188">String</span><span class="sxs-lookup"><span data-stu-id="730a0-188">String</span></span>|<span data-ttu-id="730a0-189">Отображаемое имя сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="730a0-189">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="730a0-190">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="730a0-190">privacyUrl</span></span>|<span data-ttu-id="730a0-191">String</span><span class="sxs-lookup"><span data-stu-id="730a0-191">String</span></span>|<span data-ttu-id="730a0-192">URL-адрес политики конфиденциальности компании или Организации</span><span class="sxs-lookup"><span data-stu-id="730a0-192">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="730a0-193">кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="730a0-193">customPrivacyMessage</span></span>|<span data-ttu-id="730a0-194">String</span><span class="sxs-lookup"><span data-stu-id="730a0-194">String</span></span>|<span data-ttu-id="730a0-195">Текстовые комментарии относительно того, что у администратора есть доступ к устройству.</span><span class="sxs-lookup"><span data-stu-id="730a0-195">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="730a0-196">исремоведевицедисаблед</span><span class="sxs-lookup"><span data-stu-id="730a0-196">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="730a0-197">Логический</span><span class="sxs-lookup"><span data-stu-id="730a0-197">Boolean</span></span>|<span data-ttu-id="730a0-198">Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="730a0-198">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="730a0-199">исфакториресетдисаблед</span><span class="sxs-lookup"><span data-stu-id="730a0-199">isFactoryResetDisabled</span></span>|<span data-ttu-id="730a0-200">Логический</span><span class="sxs-lookup"><span data-stu-id="730a0-200">Boolean</span></span>|<span data-ttu-id="730a0-201">Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="730a0-201">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="730a0-202">компанипорталблоккедактионс</span><span class="sxs-lookup"><span data-stu-id="730a0-202">companyPortalBlockedActions</span></span>|<span data-ttu-id="730a0-203">Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="730a0-203">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="730a0-204">Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="730a0-204">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="730a0-205">шовазуреадентерприсеаппс</span><span class="sxs-lookup"><span data-stu-id="730a0-205">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="730a0-206">Логический</span><span class="sxs-lookup"><span data-stu-id="730a0-206">Boolean</span></span>|<span data-ttu-id="730a0-207">Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.</span><span class="sxs-lookup"><span data-stu-id="730a0-207">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="730a0-208">шовоффицевебаппс</span><span class="sxs-lookup"><span data-stu-id="730a0-208">showOfficeWebApps</span></span>|<span data-ttu-id="730a0-209">Логический</span><span class="sxs-lookup"><span data-stu-id="730a0-209">Boolean</span></span>|<span data-ttu-id="730a0-210">Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.</span><span class="sxs-lookup"><span data-stu-id="730a0-210">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="730a0-211">сенддевицеовнершипчанжепушнотификатион</span><span class="sxs-lookup"><span data-stu-id="730a0-211">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="730a0-212">Логический</span><span class="sxs-lookup"><span data-stu-id="730a0-212">Boolean</span></span>|<span data-ttu-id="730a0-213">Логическое значение, указывающее, отправляются ли пользователям push-уведомления, если их тип собственности изменяется от персонального к корпоративному.</span><span class="sxs-lookup"><span data-stu-id="730a0-213">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="730a0-214">енроллментаваилабилити</span><span class="sxs-lookup"><span data-stu-id="730a0-214">enrollmentAvailability</span></span>|[<span data-ttu-id="730a0-215">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="730a0-215">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="730a0-216">Настраиваемый процесс регистрации устройства, отображаемый для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="730a0-216">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="730a0-217">Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="730a0-217">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="730a0-218">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="730a0-218">roleScopeTagIds</span></span>|<span data-ttu-id="730a0-219">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="730a0-219">String collection</span></span>|<span data-ttu-id="730a0-220">Список тегов области, назначенных профилю фирменной символики</span><span class="sxs-lookup"><span data-stu-id="730a0-220">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="730a0-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="730a0-221">Response</span></span>
<span data-ttu-id="730a0-222">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="730a0-222">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="730a0-223">Пример</span><span class="sxs-lookup"><span data-stu-id="730a0-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="730a0-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="730a0-224">Request</span></span>
<span data-ttu-id="730a0-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="730a0-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1792

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "androidForWork",
      "ownerType": "company",
      "action": "remove"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "availableWithoutPrompts",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="730a0-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="730a0-226">Response</span></span>
<span data-ttu-id="730a0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="730a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1964

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "androidForWork",
      "ownerType": "company",
      "action": "remove"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "availableWithoutPrompts",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```






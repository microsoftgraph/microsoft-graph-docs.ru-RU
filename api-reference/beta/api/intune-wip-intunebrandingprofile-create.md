---
title: Создание Интунебрандингпрофиле
description: Создание нового объекта Интунебрандингпрофиле.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e67b58af13ec67d157a44b657e019a0bd4c37204
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799740"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="d11b4-103">Создание Интунебрандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="d11b4-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="d11b4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d11b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d11b4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d11b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d11b4-106">Создание нового объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d11b4-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d11b4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d11b4-107">Prerequisites</span></span>
<span data-ttu-id="d11b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d11b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d11b4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d11b4-110">Permission type</span></span>|<span data-ttu-id="d11b4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d11b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d11b4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d11b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d11b4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d11b4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d11b4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d11b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d11b4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d11b4-115">Not supported.</span></span>|
|<span data-ttu-id="d11b4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d11b4-116">Application</span></span>|<span data-ttu-id="d11b4-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d11b4-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d11b4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d11b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="d11b4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d11b4-119">Request headers</span></span>
|<span data-ttu-id="d11b4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d11b4-120">Header</span></span>|<span data-ttu-id="d11b4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d11b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d11b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d11b4-122">Authorization</span></span>|<span data-ttu-id="d11b4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d11b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d11b4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d11b4-124">Accept</span></span>|<span data-ttu-id="d11b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d11b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d11b4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d11b4-126">Request body</span></span>
<span data-ttu-id="d11b4-127">В тексте запроса добавьте представление объекта Интунебрандингпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d11b4-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="d11b4-128">В следующей таблице приведены свойства, необходимые при создании Интунебрандингпрофиле.</span><span class="sxs-lookup"><span data-stu-id="d11b4-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="d11b4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d11b4-129">Property</span></span>|<span data-ttu-id="d11b4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d11b4-130">Type</span></span>|<span data-ttu-id="d11b4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d11b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d11b4-132">id</span><span class="sxs-lookup"><span data-stu-id="d11b4-132">id</span></span>|<span data-ttu-id="d11b4-133">String</span><span class="sxs-lookup"><span data-stu-id="d11b4-133">String</span></span>|<span data-ttu-id="d11b4-134">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="d11b4-134">Profile Key</span></span>|
|<span data-ttu-id="d11b4-135">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="d11b4-135">profileName</span></span>|<span data-ttu-id="d11b4-136">String</span><span class="sxs-lookup"><span data-stu-id="d11b4-136">String</span></span>|<span data-ttu-id="d11b4-137">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="d11b4-137">Name of the profile</span></span>|
|<span data-ttu-id="d11b4-138">профиледескриптион</span><span class="sxs-lookup"><span data-stu-id="d11b4-138">profileDescription</span></span>|<span data-ttu-id="d11b4-139">String</span><span class="sxs-lookup"><span data-stu-id="d11b4-139">String</span></span>|<span data-ttu-id="d11b4-140">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="d11b4-140">Description of the profile</span></span>|
|<span data-ttu-id="d11b4-141">исдефаултпрофиле</span><span class="sxs-lookup"><span data-stu-id="d11b4-141">isDefaultProfile</span></span>|<span data-ttu-id="d11b4-142">Логический</span><span class="sxs-lookup"><span data-stu-id="d11b4-142">Boolean</span></span>|<span data-ttu-id="d11b4-143">Логическое значение, указывающее, используется ли профиль по умолчанию или нет</span><span class="sxs-lookup"><span data-stu-id="d11b4-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="d11b4-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d11b4-144">createdDateTime</span></span>|<span data-ttu-id="d11b4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d11b4-145">DateTimeOffset</span></span>|<span data-ttu-id="d11b4-146">Время создания Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="d11b4-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="d11b4-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d11b4-147">lastModifiedDateTime</span></span>|<span data-ttu-id="d11b4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d11b4-148">DateTimeOffset</span></span>|<span data-ttu-id="d11b4-149">Время последнего изменения Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="d11b4-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="d11b4-150">displayName</span><span class="sxs-lookup"><span data-stu-id="d11b4-150">displayName</span></span>|<span data-ttu-id="d11b4-151">Строка</span><span class="sxs-lookup"><span data-stu-id="d11b4-151">String</span></span>|<span data-ttu-id="d11b4-152">Название компании или организации, которое отображается для конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="d11b4-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="d11b4-153">themeColor</span><span class="sxs-lookup"><span data-stu-id="d11b4-153">themeColor</span></span>|[<span data-ttu-id="d11b4-154">rgbColor</span><span class="sxs-lookup"><span data-stu-id="d11b4-154">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="d11b4-155">Основной цвет темы, используемый в приложениях портала компании и на веб-портале</span><span class="sxs-lookup"><span data-stu-id="d11b4-155">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="d11b4-156">showLogo</span><span class="sxs-lookup"><span data-stu-id="d11b4-156">showLogo</span></span>|<span data-ttu-id="d11b4-157">Логический</span><span class="sxs-lookup"><span data-stu-id="d11b4-157">Boolean</span></span>|<span data-ttu-id="d11b4-158">Логическое значение, указывающее, отображаются ли изображения логотипа, предоставленные администратором.</span><span class="sxs-lookup"><span data-stu-id="d11b4-158">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="d11b4-159">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="d11b4-159">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="d11b4-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="d11b4-160">Boolean</span></span>|<span data-ttu-id="d11b4-161">Логическое значение, указывающее, будет ли отображаться отображаемое имя, предоставленное администратором, рядом с изображением логотипа.</span><span class="sxs-lookup"><span data-stu-id="d11b4-161">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="d11b4-162">семеколорлого</span><span class="sxs-lookup"><span data-stu-id="d11b4-162">themeColorLogo</span></span>|<span data-ttu-id="d11b4-163">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="d11b4-163">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="d11b4-164">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть фоновый цвет темы позади логотипа</span><span class="sxs-lookup"><span data-stu-id="d11b4-164">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="d11b4-165">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="d11b4-165">lightBackgroundLogo</span></span>|[<span data-ttu-id="d11b4-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d11b4-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d11b4-167">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть светлый фон позади логотипа</span><span class="sxs-lookup"><span data-stu-id="d11b4-167">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="d11b4-168">ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="d11b4-168">landingPageCustomizedImage</span></span>|<span data-ttu-id="d11b4-169">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="d11b4-169">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="d11b4-170">Настраиваемое изображение, отображаемое на начальной странице "приложения корпоративного портала"</span><span class="sxs-lookup"><span data-stu-id="d11b4-170">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="d11b4-171">contactITName</span><span class="sxs-lookup"><span data-stu-id="d11b4-171">contactITName</span></span>|<span data-ttu-id="d11b4-172">String</span><span class="sxs-lookup"><span data-stu-id="d11b4-172">String</span></span>|<span data-ttu-id="d11b4-173">Имя пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="d11b4-173">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="d11b4-174">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d11b4-174">contactITPhoneNumber</span></span>|<span data-ttu-id="d11b4-175">String</span><span class="sxs-lookup"><span data-stu-id="d11b4-175">String</span></span>|<span data-ttu-id="d11b4-176">Номер телефона пользователя или организации, ответственного за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="d11b4-176">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="d11b4-177">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d11b4-177">contactITEmailAddress</span></span>|<span data-ttu-id="d11b4-178">String</span><span class="sxs-lookup"><span data-stu-id="d11b4-178">String</span></span>|<span data-ttu-id="d11b4-179">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="d11b4-179">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="d11b4-180">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="d11b4-180">contactITNotes</span></span>|<span data-ttu-id="d11b4-181">String</span><span class="sxs-lookup"><span data-stu-id="d11b4-181">String</span></span>|<span data-ttu-id="d11b4-182">Текстовые комментарии о лице или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="d11b4-182">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="d11b4-183">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="d11b4-183">onlineSupportSiteUrl</span></span>|<span data-ttu-id="d11b4-184">String</span><span class="sxs-lookup"><span data-stu-id="d11b4-184">String</span></span>|<span data-ttu-id="d11b4-185">URL-адрес сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="d11b4-185">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="d11b4-186">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="d11b4-186">onlineSupportSiteName</span></span>|<span data-ttu-id="d11b4-187">String</span><span class="sxs-lookup"><span data-stu-id="d11b4-187">String</span></span>|<span data-ttu-id="d11b4-188">Отображаемое имя сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="d11b4-188">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="d11b4-189">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="d11b4-189">privacyUrl</span></span>|<span data-ttu-id="d11b4-190">String</span><span class="sxs-lookup"><span data-stu-id="d11b4-190">String</span></span>|<span data-ttu-id="d11b4-191">URL-адрес политики конфиденциальности компании или Организации</span><span class="sxs-lookup"><span data-stu-id="d11b4-191">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="d11b4-192">кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="d11b4-192">customPrivacyMessage</span></span>|<span data-ttu-id="d11b4-193">String</span><span class="sxs-lookup"><span data-stu-id="d11b4-193">String</span></span>|<span data-ttu-id="d11b4-194">Текстовые комментарии относительно того, что у администратора есть доступ к устройству.</span><span class="sxs-lookup"><span data-stu-id="d11b4-194">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="d11b4-195">исремоведевицедисаблед</span><span class="sxs-lookup"><span data-stu-id="d11b4-195">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="d11b4-196">Логический</span><span class="sxs-lookup"><span data-stu-id="d11b4-196">Boolean</span></span>|<span data-ttu-id="d11b4-197">Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="d11b4-197">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="d11b4-198">исфакториресетдисаблед</span><span class="sxs-lookup"><span data-stu-id="d11b4-198">isFactoryResetDisabled</span></span>|<span data-ttu-id="d11b4-199">Логический</span><span class="sxs-lookup"><span data-stu-id="d11b4-199">Boolean</span></span>|<span data-ttu-id="d11b4-200">Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="d11b4-200">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="d11b4-201">компанипорталблоккедактионс</span><span class="sxs-lookup"><span data-stu-id="d11b4-201">companyPortalBlockedActions</span></span>|<span data-ttu-id="d11b4-202">Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="d11b4-202">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="d11b4-203">Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="d11b4-203">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="d11b4-204">шовазуреадентерприсеаппс</span><span class="sxs-lookup"><span data-stu-id="d11b4-204">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="d11b4-205">Логический</span><span class="sxs-lookup"><span data-stu-id="d11b4-205">Boolean</span></span>|<span data-ttu-id="d11b4-206">Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.</span><span class="sxs-lookup"><span data-stu-id="d11b4-206">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="d11b4-207">шовоффицевебаппс</span><span class="sxs-lookup"><span data-stu-id="d11b4-207">showOfficeWebApps</span></span>|<span data-ttu-id="d11b4-208">Логический</span><span class="sxs-lookup"><span data-stu-id="d11b4-208">Boolean</span></span>|<span data-ttu-id="d11b4-209">Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.</span><span class="sxs-lookup"><span data-stu-id="d11b4-209">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="d11b4-210">сенддевицеовнершипчанжепушнотификатион</span><span class="sxs-lookup"><span data-stu-id="d11b4-210">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="d11b4-211">Логический</span><span class="sxs-lookup"><span data-stu-id="d11b4-211">Boolean</span></span>|<span data-ttu-id="d11b4-212">Логическое значение, указывающее, отправляются ли пользователям push-уведомления, если их тип собственности изменяется от персонального к корпоративному.</span><span class="sxs-lookup"><span data-stu-id="d11b4-212">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="d11b4-213">енроллментаваилабилити</span><span class="sxs-lookup"><span data-stu-id="d11b4-213">enrollmentAvailability</span></span>|[<span data-ttu-id="d11b4-214">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="d11b4-214">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="d11b4-215">Настраиваемый процесс регистрации устройства, отображаемый для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d11b4-215">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="d11b4-216">Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="d11b4-216">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="d11b4-217">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d11b4-217">roleScopeTagIds</span></span>|<span data-ttu-id="d11b4-218">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d11b4-218">String collection</span></span>|<span data-ttu-id="d11b4-219">Список тегов области, назначенных профилю фирменной символики</span><span class="sxs-lookup"><span data-stu-id="d11b4-219">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="d11b4-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="d11b4-220">Response</span></span>
<span data-ttu-id="d11b4-221">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d11b4-221">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d11b4-222">Пример</span><span class="sxs-lookup"><span data-stu-id="d11b4-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="d11b4-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="d11b4-223">Request</span></span>
<span data-ttu-id="d11b4-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d11b4-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
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

### <a name="response"></a><span data-ttu-id="d11b4-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="d11b4-225">Response</span></span>
<span data-ttu-id="d11b4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d11b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





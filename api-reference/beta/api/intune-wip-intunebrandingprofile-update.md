---
title: Обновление Интунебрандингпрофиле
description: Обновление свойств объекта Интунебрандингпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e12edcc8e292cd140a9628d48e3e263c65f4f496
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43386715"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="a2f9d-103">Обновление Интунебрандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="a2f9d-103">Update intuneBrandingProfile</span></span>

<span data-ttu-id="a2f9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2f9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2f9d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2f9d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2f9d-107">Обновление свойств объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a2f9d-107">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2f9d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a2f9d-108">Prerequisites</span></span>
<span data-ttu-id="a2f9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2f9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2f9d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2f9d-111">Permission type</span></span>|<span data-ttu-id="a2f9d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2f9d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2f9d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2f9d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2f9d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2f9d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2f9d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2f9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2f9d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-116">Not supported.</span></span>|
|<span data-ttu-id="a2f9d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2f9d-117">Application</span></span>|<span data-ttu-id="a2f9d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2f9d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2f9d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2f9d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="a2f9d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a2f9d-120">Request headers</span></span>
|<span data-ttu-id="a2f9d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2f9d-121">Header</span></span>|<span data-ttu-id="a2f9d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a2f9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2f9d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2f9d-123">Authorization</span></span>|<span data-ttu-id="a2f9d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2f9d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2f9d-125">Accept</span></span>|<span data-ttu-id="a2f9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2f9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2f9d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2f9d-127">Request body</span></span>
<span data-ttu-id="a2f9d-128">В тексте запроса добавьте представление объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-128">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="a2f9d-129">В следующей таблице приведены свойства, необходимые при создании [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="a2f9d-129">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="a2f9d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2f9d-130">Property</span></span>|<span data-ttu-id="a2f9d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a2f9d-131">Type</span></span>|<span data-ttu-id="a2f9d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a2f9d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2f9d-133">id</span><span class="sxs-lookup"><span data-stu-id="a2f9d-133">id</span></span>|<span data-ttu-id="a2f9d-134">String</span><span class="sxs-lookup"><span data-stu-id="a2f9d-134">String</span></span>|<span data-ttu-id="a2f9d-135">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="a2f9d-135">Profile Key</span></span>|
|<span data-ttu-id="a2f9d-136">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="a2f9d-136">profileName</span></span>|<span data-ttu-id="a2f9d-137">String</span><span class="sxs-lookup"><span data-stu-id="a2f9d-137">String</span></span>|<span data-ttu-id="a2f9d-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="a2f9d-138">Name of the profile</span></span>|
|<span data-ttu-id="a2f9d-139">профиледескриптион</span><span class="sxs-lookup"><span data-stu-id="a2f9d-139">profileDescription</span></span>|<span data-ttu-id="a2f9d-140">String</span><span class="sxs-lookup"><span data-stu-id="a2f9d-140">String</span></span>|<span data-ttu-id="a2f9d-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="a2f9d-141">Description of the profile</span></span>|
|<span data-ttu-id="a2f9d-142">исдефаултпрофиле</span><span class="sxs-lookup"><span data-stu-id="a2f9d-142">isDefaultProfile</span></span>|<span data-ttu-id="a2f9d-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2f9d-143">Boolean</span></span>|<span data-ttu-id="a2f9d-144">Логическое значение, указывающее, используется ли профиль по умолчанию или нет</span><span class="sxs-lookup"><span data-stu-id="a2f9d-144">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="a2f9d-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2f9d-145">createdDateTime</span></span>|<span data-ttu-id="a2f9d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2f9d-146">DateTimeOffset</span></span>|<span data-ttu-id="a2f9d-147">Время создания Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="a2f9d-147">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="a2f9d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2f9d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a2f9d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2f9d-149">DateTimeOffset</span></span>|<span data-ttu-id="a2f9d-150">Время последнего изменения Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="a2f9d-150">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="a2f9d-151">displayName</span><span class="sxs-lookup"><span data-stu-id="a2f9d-151">displayName</span></span>|<span data-ttu-id="a2f9d-152">Строка</span><span class="sxs-lookup"><span data-stu-id="a2f9d-152">String</span></span>|<span data-ttu-id="a2f9d-153">Название компании или организации, которое отображается для конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="a2f9d-153">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="a2f9d-154">themeColor</span><span class="sxs-lookup"><span data-stu-id="a2f9d-154">themeColor</span></span>|[<span data-ttu-id="a2f9d-155">rgbColor</span><span class="sxs-lookup"><span data-stu-id="a2f9d-155">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="a2f9d-156">Основной цвет темы, используемый в приложениях портала компании и на веб-портале</span><span class="sxs-lookup"><span data-stu-id="a2f9d-156">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="a2f9d-157">showLogo</span><span class="sxs-lookup"><span data-stu-id="a2f9d-157">showLogo</span></span>|<span data-ttu-id="a2f9d-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2f9d-158">Boolean</span></span>|<span data-ttu-id="a2f9d-159">Логическое значение, указывающее, отображаются ли изображения логотипа, предоставленные администратором.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-159">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="a2f9d-160">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="a2f9d-160">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="a2f9d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2f9d-161">Boolean</span></span>|<span data-ttu-id="a2f9d-162">Логическое значение, указывающее, будет ли отображаться отображаемое имя, предоставленное администратором, рядом с изображением логотипа.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-162">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="a2f9d-163">семеколорлого</span><span class="sxs-lookup"><span data-stu-id="a2f9d-163">themeColorLogo</span></span>|<span data-ttu-id="a2f9d-164">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="a2f9d-164">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="a2f9d-165">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть фоновый цвет темы позади логотипа</span><span class="sxs-lookup"><span data-stu-id="a2f9d-165">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="a2f9d-166">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="a2f9d-166">lightBackgroundLogo</span></span>|[<span data-ttu-id="a2f9d-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a2f9d-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a2f9d-168">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть светлый фон позади логотипа</span><span class="sxs-lookup"><span data-stu-id="a2f9d-168">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="a2f9d-169">ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="a2f9d-169">landingPageCustomizedImage</span></span>|<span data-ttu-id="a2f9d-170">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="a2f9d-170">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="a2f9d-171">Настраиваемое изображение, отображаемое на начальной странице "приложения корпоративного портала"</span><span class="sxs-lookup"><span data-stu-id="a2f9d-171">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="a2f9d-172">contactITName</span><span class="sxs-lookup"><span data-stu-id="a2f9d-172">contactITName</span></span>|<span data-ttu-id="a2f9d-173">String</span><span class="sxs-lookup"><span data-stu-id="a2f9d-173">String</span></span>|<span data-ttu-id="a2f9d-174">Имя пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="a2f9d-174">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="a2f9d-175">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="a2f9d-175">contactITPhoneNumber</span></span>|<span data-ttu-id="a2f9d-176">String</span><span class="sxs-lookup"><span data-stu-id="a2f9d-176">String</span></span>|<span data-ttu-id="a2f9d-177">Номер телефона пользователя или организации, ответственного за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="a2f9d-177">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="a2f9d-178">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a2f9d-178">contactITEmailAddress</span></span>|<span data-ttu-id="a2f9d-179">String</span><span class="sxs-lookup"><span data-stu-id="a2f9d-179">String</span></span>|<span data-ttu-id="a2f9d-180">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="a2f9d-180">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="a2f9d-181">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="a2f9d-181">contactITNotes</span></span>|<span data-ttu-id="a2f9d-182">String</span><span class="sxs-lookup"><span data-stu-id="a2f9d-182">String</span></span>|<span data-ttu-id="a2f9d-183">Текстовые комментарии о лице или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="a2f9d-183">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="a2f9d-184">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="a2f9d-184">onlineSupportSiteUrl</span></span>|<span data-ttu-id="a2f9d-185">String</span><span class="sxs-lookup"><span data-stu-id="a2f9d-185">String</span></span>|<span data-ttu-id="a2f9d-186">URL-адрес сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="a2f9d-186">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="a2f9d-187">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="a2f9d-187">onlineSupportSiteName</span></span>|<span data-ttu-id="a2f9d-188">String</span><span class="sxs-lookup"><span data-stu-id="a2f9d-188">String</span></span>|<span data-ttu-id="a2f9d-189">Отображаемое имя сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="a2f9d-189">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="a2f9d-190">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="a2f9d-190">privacyUrl</span></span>|<span data-ttu-id="a2f9d-191">String</span><span class="sxs-lookup"><span data-stu-id="a2f9d-191">String</span></span>|<span data-ttu-id="a2f9d-192">URL-адрес политики конфиденциальности компании или Организации</span><span class="sxs-lookup"><span data-stu-id="a2f9d-192">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="a2f9d-193">кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="a2f9d-193">customPrivacyMessage</span></span>|<span data-ttu-id="a2f9d-194">String</span><span class="sxs-lookup"><span data-stu-id="a2f9d-194">String</span></span>|<span data-ttu-id="a2f9d-195">Текстовые комментарии относительно того, что у администратора есть доступ к устройству.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-195">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="a2f9d-196">исремоведевицедисаблед</span><span class="sxs-lookup"><span data-stu-id="a2f9d-196">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="a2f9d-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2f9d-197">Boolean</span></span>|<span data-ttu-id="a2f9d-198">Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-198">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="a2f9d-199">исфакториресетдисаблед</span><span class="sxs-lookup"><span data-stu-id="a2f9d-199">isFactoryResetDisabled</span></span>|<span data-ttu-id="a2f9d-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2f9d-200">Boolean</span></span>|<span data-ttu-id="a2f9d-201">Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-201">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="a2f9d-202">компанипорталблоккедактионс</span><span class="sxs-lookup"><span data-stu-id="a2f9d-202">companyPortalBlockedActions</span></span>|<span data-ttu-id="a2f9d-203">Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="a2f9d-203">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="a2f9d-204">Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-204">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="a2f9d-205">шовазуреадентерприсеаппс</span><span class="sxs-lookup"><span data-stu-id="a2f9d-205">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="a2f9d-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2f9d-206">Boolean</span></span>|<span data-ttu-id="a2f9d-207">Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-207">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="a2f9d-208">шовоффицевебаппс</span><span class="sxs-lookup"><span data-stu-id="a2f9d-208">showOfficeWebApps</span></span>|<span data-ttu-id="a2f9d-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2f9d-209">Boolean</span></span>|<span data-ttu-id="a2f9d-210">Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-210">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="a2f9d-211">сенддевицеовнершипчанжепушнотификатион</span><span class="sxs-lookup"><span data-stu-id="a2f9d-211">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="a2f9d-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2f9d-212">Boolean</span></span>|<span data-ttu-id="a2f9d-213">Логическое значение, указывающее, отправляются ли пользователям push-уведомления, если их тип собственности изменяется от персонального к корпоративному.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-213">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="a2f9d-214">енроллментаваилабилити</span><span class="sxs-lookup"><span data-stu-id="a2f9d-214">enrollmentAvailability</span></span>|[<span data-ttu-id="a2f9d-215">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="a2f9d-215">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="a2f9d-216">Настраиваемый процесс регистрации устройства, отображаемый для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-216">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="a2f9d-217">Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-217">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="a2f9d-218">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a2f9d-218">roleScopeTagIds</span></span>|<span data-ttu-id="a2f9d-219">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a2f9d-219">String collection</span></span>|<span data-ttu-id="a2f9d-220">Список тегов области, назначенных профилю фирменной символики</span><span class="sxs-lookup"><span data-stu-id="a2f9d-220">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="a2f9d-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2f9d-221">Response</span></span>
<span data-ttu-id="a2f9d-222">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-222">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2f9d-223">Пример</span><span class="sxs-lookup"><span data-stu-id="a2f9d-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2f9d-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2f9d-224">Request</span></span>
<span data-ttu-id="a2f9d-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a2f9d-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2f9d-226">Response</span></span>
<span data-ttu-id="a2f9d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2f9d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




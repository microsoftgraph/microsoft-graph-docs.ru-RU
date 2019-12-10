---
title: Обновление Интунебрандингпрофиле
description: Обновление свойств объекта Интунебрандингпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0cd72b310ad29e5ff32520945d63a80f7fb1b370
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938476"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="10e3b-103">Обновление Интунебрандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="10e3b-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="10e3b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10e3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10e3b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10e3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10e3b-106">Обновление свойств объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="10e3b-106">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10e3b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="10e3b-107">Prerequisites</span></span>
<span data-ttu-id="10e3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10e3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10e3b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10e3b-110">Permission type</span></span>|<span data-ttu-id="10e3b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10e3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10e3b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10e3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10e3b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10e3b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="10e3b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10e3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10e3b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10e3b-115">Not supported.</span></span>|
|<span data-ttu-id="10e3b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10e3b-116">Application</span></span>|<span data-ttu-id="10e3b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10e3b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10e3b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10e3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="10e3b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="10e3b-119">Request headers</span></span>
|<span data-ttu-id="10e3b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10e3b-120">Header</span></span>|<span data-ttu-id="10e3b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="10e3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10e3b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10e3b-122">Authorization</span></span>|<span data-ttu-id="10e3b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10e3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10e3b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="10e3b-124">Accept</span></span>|<span data-ttu-id="10e3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10e3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10e3b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10e3b-126">Request body</span></span>
<span data-ttu-id="10e3b-127">В тексте запроса добавьте представление объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10e3b-127">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="10e3b-128">В следующей таблице приведены свойства, необходимые при создании [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="10e3b-128">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="10e3b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="10e3b-129">Property</span></span>|<span data-ttu-id="10e3b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="10e3b-130">Type</span></span>|<span data-ttu-id="10e3b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="10e3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10e3b-132">id</span><span class="sxs-lookup"><span data-stu-id="10e3b-132">id</span></span>|<span data-ttu-id="10e3b-133">String</span><span class="sxs-lookup"><span data-stu-id="10e3b-133">String</span></span>|<span data-ttu-id="10e3b-134">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="10e3b-134">Profile Key</span></span>|
|<span data-ttu-id="10e3b-135">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="10e3b-135">profileName</span></span>|<span data-ttu-id="10e3b-136">Строка</span><span class="sxs-lookup"><span data-stu-id="10e3b-136">String</span></span>|<span data-ttu-id="10e3b-137">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="10e3b-137">Name of the profile</span></span>|
|<span data-ttu-id="10e3b-138">профиледескриптион</span><span class="sxs-lookup"><span data-stu-id="10e3b-138">profileDescription</span></span>|<span data-ttu-id="10e3b-139">Строка</span><span class="sxs-lookup"><span data-stu-id="10e3b-139">String</span></span>|<span data-ttu-id="10e3b-140">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="10e3b-140">Description of the profile</span></span>|
|<span data-ttu-id="10e3b-141">исдефаултпрофиле</span><span class="sxs-lookup"><span data-stu-id="10e3b-141">isDefaultProfile</span></span>|<span data-ttu-id="10e3b-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="10e3b-142">Boolean</span></span>|<span data-ttu-id="10e3b-143">Логическое значение, указывающее, используется ли профиль по умолчанию или нет</span><span class="sxs-lookup"><span data-stu-id="10e3b-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="10e3b-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10e3b-144">createdDateTime</span></span>|<span data-ttu-id="10e3b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10e3b-145">DateTimeOffset</span></span>|<span data-ttu-id="10e3b-146">Время создания Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="10e3b-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="10e3b-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10e3b-147">lastModifiedDateTime</span></span>|<span data-ttu-id="10e3b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10e3b-148">DateTimeOffset</span></span>|<span data-ttu-id="10e3b-149">Время последнего изменения Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="10e3b-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="10e3b-150">displayName</span><span class="sxs-lookup"><span data-stu-id="10e3b-150">displayName</span></span>|<span data-ttu-id="10e3b-151">Строка</span><span class="sxs-lookup"><span data-stu-id="10e3b-151">String</span></span>|<span data-ttu-id="10e3b-152">Название компании или организации, которое отображается для конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="10e3b-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="10e3b-153">themeColor</span><span class="sxs-lookup"><span data-stu-id="10e3b-153">themeColor</span></span>|[<span data-ttu-id="10e3b-154">rgbColor</span><span class="sxs-lookup"><span data-stu-id="10e3b-154">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="10e3b-155">Основной цвет темы, используемый в приложениях портала компании и на веб-портале</span><span class="sxs-lookup"><span data-stu-id="10e3b-155">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="10e3b-156">showLogo</span><span class="sxs-lookup"><span data-stu-id="10e3b-156">showLogo</span></span>|<span data-ttu-id="10e3b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="10e3b-157">Boolean</span></span>|<span data-ttu-id="10e3b-158">Логическое значение, указывающее, отображаются ли изображения логотипа, предоставленные администратором.</span><span class="sxs-lookup"><span data-stu-id="10e3b-158">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="10e3b-159">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="10e3b-159">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="10e3b-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="10e3b-160">Boolean</span></span>|<span data-ttu-id="10e3b-161">Логическое значение, указывающее, будет ли отображаться отображаемое имя, предоставленное администратором, рядом с изображением логотипа.</span><span class="sxs-lookup"><span data-stu-id="10e3b-161">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="10e3b-162">семеколорлого</span><span class="sxs-lookup"><span data-stu-id="10e3b-162">themeColorLogo</span></span>|<span data-ttu-id="10e3b-163">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="10e3b-163">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="10e3b-164">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть фоновый цвет темы позади логотипа</span><span class="sxs-lookup"><span data-stu-id="10e3b-164">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="10e3b-165">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="10e3b-165">lightBackgroundLogo</span></span>|[<span data-ttu-id="10e3b-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="10e3b-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="10e3b-167">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть светлый фон позади логотипа</span><span class="sxs-lookup"><span data-stu-id="10e3b-167">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="10e3b-168">ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="10e3b-168">landingPageCustomizedImage</span></span>|<span data-ttu-id="10e3b-169">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="10e3b-169">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="10e3b-170">Настраиваемое изображение, отображаемое на начальной странице "приложения корпоративного портала"</span><span class="sxs-lookup"><span data-stu-id="10e3b-170">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="10e3b-171">contactITName</span><span class="sxs-lookup"><span data-stu-id="10e3b-171">contactITName</span></span>|<span data-ttu-id="10e3b-172">Строка</span><span class="sxs-lookup"><span data-stu-id="10e3b-172">String</span></span>|<span data-ttu-id="10e3b-173">Имя пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="10e3b-173">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="10e3b-174">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="10e3b-174">contactITPhoneNumber</span></span>|<span data-ttu-id="10e3b-175">Строка</span><span class="sxs-lookup"><span data-stu-id="10e3b-175">String</span></span>|<span data-ttu-id="10e3b-176">Номер телефона пользователя или организации, ответственного за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="10e3b-176">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="10e3b-177">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="10e3b-177">contactITEmailAddress</span></span>|<span data-ttu-id="10e3b-178">Строка</span><span class="sxs-lookup"><span data-stu-id="10e3b-178">String</span></span>|<span data-ttu-id="10e3b-179">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="10e3b-179">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="10e3b-180">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="10e3b-180">contactITNotes</span></span>|<span data-ttu-id="10e3b-181">Строка</span><span class="sxs-lookup"><span data-stu-id="10e3b-181">String</span></span>|<span data-ttu-id="10e3b-182">Текстовые комментарии о лице или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="10e3b-182">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="10e3b-183">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="10e3b-183">onlineSupportSiteUrl</span></span>|<span data-ttu-id="10e3b-184">Строка</span><span class="sxs-lookup"><span data-stu-id="10e3b-184">String</span></span>|<span data-ttu-id="10e3b-185">URL-адрес сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="10e3b-185">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="10e3b-186">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="10e3b-186">onlineSupportSiteName</span></span>|<span data-ttu-id="10e3b-187">String</span><span class="sxs-lookup"><span data-stu-id="10e3b-187">String</span></span>|<span data-ttu-id="10e3b-188">Отображаемое имя сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="10e3b-188">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="10e3b-189">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="10e3b-189">privacyUrl</span></span>|<span data-ttu-id="10e3b-190">Строка</span><span class="sxs-lookup"><span data-stu-id="10e3b-190">String</span></span>|<span data-ttu-id="10e3b-191">URL-адрес политики конфиденциальности компании или Организации</span><span class="sxs-lookup"><span data-stu-id="10e3b-191">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="10e3b-192">кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="10e3b-192">customPrivacyMessage</span></span>|<span data-ttu-id="10e3b-193">Строка</span><span class="sxs-lookup"><span data-stu-id="10e3b-193">String</span></span>|<span data-ttu-id="10e3b-194">Текстовые комментарии относительно того, что у администратора есть доступ к устройству.</span><span class="sxs-lookup"><span data-stu-id="10e3b-194">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="10e3b-195">исремоведевицедисаблед</span><span class="sxs-lookup"><span data-stu-id="10e3b-195">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="10e3b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="10e3b-196">Boolean</span></span>|<span data-ttu-id="10e3b-197">Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="10e3b-197">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="10e3b-198">исфакториресетдисаблед</span><span class="sxs-lookup"><span data-stu-id="10e3b-198">isFactoryResetDisabled</span></span>|<span data-ttu-id="10e3b-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="10e3b-199">Boolean</span></span>|<span data-ttu-id="10e3b-200">Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="10e3b-200">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="10e3b-201">компанипорталблоккедактионс</span><span class="sxs-lookup"><span data-stu-id="10e3b-201">companyPortalBlockedActions</span></span>|<span data-ttu-id="10e3b-202">Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="10e3b-202">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="10e3b-203">Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="10e3b-203">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="10e3b-204">шовазуреадентерприсеаппс</span><span class="sxs-lookup"><span data-stu-id="10e3b-204">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="10e3b-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="10e3b-205">Boolean</span></span>|<span data-ttu-id="10e3b-206">Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.</span><span class="sxs-lookup"><span data-stu-id="10e3b-206">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="10e3b-207">шовоффицевебаппс</span><span class="sxs-lookup"><span data-stu-id="10e3b-207">showOfficeWebApps</span></span>|<span data-ttu-id="10e3b-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="10e3b-208">Boolean</span></span>|<span data-ttu-id="10e3b-209">Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.</span><span class="sxs-lookup"><span data-stu-id="10e3b-209">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|



## <a name="response"></a><span data-ttu-id="10e3b-210">Ответ</span><span class="sxs-lookup"><span data-stu-id="10e3b-210">Response</span></span>
<span data-ttu-id="10e3b-211">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10e3b-211">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10e3b-212">Пример</span><span class="sxs-lookup"><span data-stu-id="10e3b-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="10e3b-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="10e3b-213">Request</span></span>
<span data-ttu-id="10e3b-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10e3b-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1620

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
  "showOfficeWebApps": true
}
```

### <a name="response"></a><span data-ttu-id="10e3b-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="10e3b-215">Response</span></span>
<span data-ttu-id="10e3b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10e3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1792

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
  "showOfficeWebApps": true
}
```






---
title: Создание Интунебрандингпрофиле
description: Создание нового объекта Интунебрандингпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a575a68e399735a012f884c93f644676ffbdf3f7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209824"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="c1510-103">Создание Интунебрандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="c1510-103">Create intuneBrandingProfile</span></span>

<span data-ttu-id="c1510-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1510-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1510-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1510-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1510-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1510-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1510-107">Создание нового объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c1510-107">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1510-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c1510-108">Prerequisites</span></span>
<span data-ttu-id="c1510-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1510-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1510-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1510-111">Permission type</span></span>|<span data-ttu-id="c1510-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1510-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1510-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1510-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1510-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1510-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c1510-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1510-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1510-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1510-116">Not supported.</span></span>|
|<span data-ttu-id="c1510-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c1510-117">Application</span></span>|<span data-ttu-id="c1510-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1510-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1510-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1510-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c1510-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c1510-120">Request headers</span></span>
|<span data-ttu-id="c1510-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1510-121">Header</span></span>|<span data-ttu-id="c1510-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c1510-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1510-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1510-123">Authorization</span></span>|<span data-ttu-id="c1510-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1510-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1510-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1510-125">Accept</span></span>|<span data-ttu-id="c1510-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1510-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1510-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1510-127">Request body</span></span>
<span data-ttu-id="c1510-128">В тексте запроса добавьте представление объекта Интунебрандингпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1510-128">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="c1510-129">В следующей таблице приведены свойства, необходимые при создании Интунебрандингпрофиле.</span><span class="sxs-lookup"><span data-stu-id="c1510-129">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="c1510-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1510-130">Property</span></span>|<span data-ttu-id="c1510-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c1510-131">Type</span></span>|<span data-ttu-id="c1510-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c1510-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1510-133">id</span><span class="sxs-lookup"><span data-stu-id="c1510-133">id</span></span>|<span data-ttu-id="c1510-134">String</span><span class="sxs-lookup"><span data-stu-id="c1510-134">String</span></span>|<span data-ttu-id="c1510-135">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="c1510-135">Profile Key</span></span>|
|<span data-ttu-id="c1510-136">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="c1510-136">profileName</span></span>|<span data-ttu-id="c1510-137">String</span><span class="sxs-lookup"><span data-stu-id="c1510-137">String</span></span>|<span data-ttu-id="c1510-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="c1510-138">Name of the profile</span></span>|
|<span data-ttu-id="c1510-139">профиледескриптион</span><span class="sxs-lookup"><span data-stu-id="c1510-139">profileDescription</span></span>|<span data-ttu-id="c1510-140">String</span><span class="sxs-lookup"><span data-stu-id="c1510-140">String</span></span>|<span data-ttu-id="c1510-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="c1510-141">Description of the profile</span></span>|
|<span data-ttu-id="c1510-142">исдефаултпрофиле</span><span class="sxs-lookup"><span data-stu-id="c1510-142">isDefaultProfile</span></span>|<span data-ttu-id="c1510-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1510-143">Boolean</span></span>|<span data-ttu-id="c1510-144">Логическое значение, указывающее, используется ли профиль по умолчанию или нет</span><span class="sxs-lookup"><span data-stu-id="c1510-144">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="c1510-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1510-145">createdDateTime</span></span>|<span data-ttu-id="c1510-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1510-146">DateTimeOffset</span></span>|<span data-ttu-id="c1510-147">Время создания Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="c1510-147">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="c1510-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1510-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c1510-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1510-149">DateTimeOffset</span></span>|<span data-ttu-id="c1510-150">Время последнего изменения Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="c1510-150">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="c1510-151">displayName</span><span class="sxs-lookup"><span data-stu-id="c1510-151">displayName</span></span>|<span data-ttu-id="c1510-152">String</span><span class="sxs-lookup"><span data-stu-id="c1510-152">String</span></span>|<span data-ttu-id="c1510-153">Название компании или организации, которое отображается для конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="c1510-153">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="c1510-154">themeColor</span><span class="sxs-lookup"><span data-stu-id="c1510-154">themeColor</span></span>|[<span data-ttu-id="c1510-155">rgbColor</span><span class="sxs-lookup"><span data-stu-id="c1510-155">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="c1510-156">Основной цвет темы, используемый в приложениях портала компании и на веб-портале</span><span class="sxs-lookup"><span data-stu-id="c1510-156">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="c1510-157">showLogo</span><span class="sxs-lookup"><span data-stu-id="c1510-157">showLogo</span></span>|<span data-ttu-id="c1510-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1510-158">Boolean</span></span>|<span data-ttu-id="c1510-159">Логическое значение, указывающее, отображаются ли изображения логотипа, предоставленные администратором.</span><span class="sxs-lookup"><span data-stu-id="c1510-159">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="c1510-160">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="c1510-160">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="c1510-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1510-161">Boolean</span></span>|<span data-ttu-id="c1510-162">Логическое значение, указывающее, будет ли отображаться отображаемое имя, предоставленное администратором, рядом с изображением логотипа.</span><span class="sxs-lookup"><span data-stu-id="c1510-162">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="c1510-163">семеколорлого</span><span class="sxs-lookup"><span data-stu-id="c1510-163">themeColorLogo</span></span>|<span data-ttu-id="c1510-164">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="c1510-164">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="c1510-165">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть фоновый цвет темы позади логотипа</span><span class="sxs-lookup"><span data-stu-id="c1510-165">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="c1510-166">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="c1510-166">lightBackgroundLogo</span></span>|[<span data-ttu-id="c1510-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c1510-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c1510-168">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть светлый фон позади логотипа</span><span class="sxs-lookup"><span data-stu-id="c1510-168">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="c1510-169">ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="c1510-169">landingPageCustomizedImage</span></span>|<span data-ttu-id="c1510-170">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="c1510-170">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="c1510-171">Настраиваемое изображение, отображаемое на начальной странице "приложения корпоративного портала"</span><span class="sxs-lookup"><span data-stu-id="c1510-171">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="c1510-172">contactITName</span><span class="sxs-lookup"><span data-stu-id="c1510-172">contactITName</span></span>|<span data-ttu-id="c1510-173">String</span><span class="sxs-lookup"><span data-stu-id="c1510-173">String</span></span>|<span data-ttu-id="c1510-174">Имя пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="c1510-174">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="c1510-175">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="c1510-175">contactITPhoneNumber</span></span>|<span data-ttu-id="c1510-176">String</span><span class="sxs-lookup"><span data-stu-id="c1510-176">String</span></span>|<span data-ttu-id="c1510-177">Номер телефона пользователя или организации, ответственного за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="c1510-177">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="c1510-178">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c1510-178">contactITEmailAddress</span></span>|<span data-ttu-id="c1510-179">String</span><span class="sxs-lookup"><span data-stu-id="c1510-179">String</span></span>|<span data-ttu-id="c1510-180">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="c1510-180">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="c1510-181">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="c1510-181">contactITNotes</span></span>|<span data-ttu-id="c1510-182">String</span><span class="sxs-lookup"><span data-stu-id="c1510-182">String</span></span>|<span data-ttu-id="c1510-183">Текстовые комментарии о лице или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="c1510-183">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="c1510-184">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="c1510-184">onlineSupportSiteUrl</span></span>|<span data-ttu-id="c1510-185">String</span><span class="sxs-lookup"><span data-stu-id="c1510-185">String</span></span>|<span data-ttu-id="c1510-186">URL-адрес сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="c1510-186">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="c1510-187">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="c1510-187">onlineSupportSiteName</span></span>|<span data-ttu-id="c1510-188">String</span><span class="sxs-lookup"><span data-stu-id="c1510-188">String</span></span>|<span data-ttu-id="c1510-189">Отображаемое имя сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="c1510-189">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="c1510-190">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="c1510-190">privacyUrl</span></span>|<span data-ttu-id="c1510-191">String</span><span class="sxs-lookup"><span data-stu-id="c1510-191">String</span></span>|<span data-ttu-id="c1510-192">URL-адрес политики конфиденциальности компании или Организации</span><span class="sxs-lookup"><span data-stu-id="c1510-192">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="c1510-193">кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="c1510-193">customPrivacyMessage</span></span>|<span data-ttu-id="c1510-194">String</span><span class="sxs-lookup"><span data-stu-id="c1510-194">String</span></span>|<span data-ttu-id="c1510-195">Текстовые комментарии относительно того, что у администратора нет доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="c1510-195">Text comments regarding what the admin doesn't have access to on the device</span></span>|
|<span data-ttu-id="c1510-196">кустомкансипривацимессаже</span><span class="sxs-lookup"><span data-stu-id="c1510-196">customCanSeePrivacyMessage</span></span>|<span data-ttu-id="c1510-197">String</span><span class="sxs-lookup"><span data-stu-id="c1510-197">String</span></span>|<span data-ttu-id="c1510-198">Текстовые комментарии относительно того, что у администратора есть доступ к устройству.</span><span class="sxs-lookup"><span data-stu-id="c1510-198">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="c1510-199">кустомкантсипривацимессаже</span><span class="sxs-lookup"><span data-stu-id="c1510-199">customCantSeePrivacyMessage</span></span>|<span data-ttu-id="c1510-200">String</span><span class="sxs-lookup"><span data-stu-id="c1510-200">String</span></span>|<span data-ttu-id="c1510-201">Текстовые комментарии относительно того, что у администратора нет доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="c1510-201">Text comments regarding what the admin doesn't have access to on the device</span></span>|
|<span data-ttu-id="c1510-202">исремоведевицедисаблед</span><span class="sxs-lookup"><span data-stu-id="c1510-202">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="c1510-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1510-203">Boolean</span></span>|<span data-ttu-id="c1510-204">Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="c1510-204">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="c1510-205">исфакториресетдисаблед</span><span class="sxs-lookup"><span data-stu-id="c1510-205">isFactoryResetDisabled</span></span>|<span data-ttu-id="c1510-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1510-206">Boolean</span></span>|<span data-ttu-id="c1510-207">Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="c1510-207">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="c1510-208">компанипорталблоккедактионс</span><span class="sxs-lookup"><span data-stu-id="c1510-208">companyPortalBlockedActions</span></span>|<span data-ttu-id="c1510-209">Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="c1510-209">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="c1510-210">Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="c1510-210">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="c1510-211">шовазуреадентерприсеаппс</span><span class="sxs-lookup"><span data-stu-id="c1510-211">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="c1510-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1510-212">Boolean</span></span>|<span data-ttu-id="c1510-213">Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.</span><span class="sxs-lookup"><span data-stu-id="c1510-213">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="c1510-214">шовоффицевебаппс</span><span class="sxs-lookup"><span data-stu-id="c1510-214">showOfficeWebApps</span></span>|<span data-ttu-id="c1510-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1510-215">Boolean</span></span>|<span data-ttu-id="c1510-216">Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.</span><span class="sxs-lookup"><span data-stu-id="c1510-216">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="c1510-217">сенддевицеовнершипчанжепушнотификатион</span><span class="sxs-lookup"><span data-stu-id="c1510-217">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="c1510-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1510-218">Boolean</span></span>|<span data-ttu-id="c1510-219">Логическое значение, указывающее, отправляются ли пользователям push-уведомления, если их тип собственности изменяется от персонального к корпоративному.</span><span class="sxs-lookup"><span data-stu-id="c1510-219">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="c1510-220">енроллментаваилабилити</span><span class="sxs-lookup"><span data-stu-id="c1510-220">enrollmentAvailability</span></span>|[<span data-ttu-id="c1510-221">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="c1510-221">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="c1510-222">Настраиваемый процесс регистрации устройства, отображаемый для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1510-222">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="c1510-223">Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="c1510-223">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="c1510-224">дисаблеклиенттелеметри</span><span class="sxs-lookup"><span data-stu-id="c1510-224">disableClientTelemetry</span></span>|<span data-ttu-id="c1510-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1510-225">Boolean</span></span>|<span data-ttu-id="c1510-226">Применяется к телеметрии, отправляемой со всех клиентов в службу Intune.</span><span class="sxs-lookup"><span data-stu-id="c1510-226">Applies to telemetry sent from all clients to the Intune service.</span></span> <span data-ttu-id="c1510-227">Если этот параметр отключен, все предупреждения об устранении неполадок и неполадки в клиенте отключаются, и параметры телеметрии отображаются как неактивные или скрытые для пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="c1510-227">When disabled, all proactive troubleshooting and issue warnings within the client are turned off, and telemetry settings appear inactive or hidden to the device user.</span></span>|
|<span data-ttu-id="c1510-228">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1510-228">roleScopeTagIds</span></span>|<span data-ttu-id="c1510-229">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c1510-229">String collection</span></span>|<span data-ttu-id="c1510-230">Список тегов области, назначенных профилю фирменной символики</span><span class="sxs-lookup"><span data-stu-id="c1510-230">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="c1510-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1510-231">Response</span></span>
<span data-ttu-id="c1510-232">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1510-232">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1510-233">Пример</span><span class="sxs-lookup"><span data-stu-id="c1510-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1510-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1510-234">Request</span></span>
<span data-ttu-id="c1510-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1510-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1975

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
  "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
  "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
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
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="c1510-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1510-236">Response</span></span>
<span data-ttu-id="c1510-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1510-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2147

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
  "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
  "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
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
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





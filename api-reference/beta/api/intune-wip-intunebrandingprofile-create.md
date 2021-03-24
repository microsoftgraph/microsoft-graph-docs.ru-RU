---
title: Создание intuneBrandingProfile
description: Создайте новый объект intuneBrandingProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e6b8d89b2575402cc38b5f86ecd8a872fd666b3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133854"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="2bfbf-103">Создание intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="2bfbf-103">Create intuneBrandingProfile</span></span>

<span data-ttu-id="2bfbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bfbf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bfbf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bfbf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bfbf-107">Создайте новый [объект intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2bfbf-107">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bfbf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2bfbf-108">Prerequisites</span></span>
<span data-ttu-id="2bfbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bfbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bfbf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bfbf-111">Permission type</span></span>|<span data-ttu-id="2bfbf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bfbf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bfbf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bfbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2bfbf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bfbf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2bfbf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bfbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bfbf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-116">Not supported.</span></span>|
|<span data-ttu-id="2bfbf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2bfbf-117">Application</span></span>|<span data-ttu-id="2bfbf-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bfbf-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bfbf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bfbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="2bfbf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2bfbf-120">Request headers</span></span>
|<span data-ttu-id="2bfbf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2bfbf-121">Header</span></span>|<span data-ttu-id="2bfbf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2bfbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bfbf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bfbf-123">Authorization</span></span>|<span data-ttu-id="2bfbf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bfbf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2bfbf-125">Accept</span></span>|<span data-ttu-id="2bfbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2bfbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bfbf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2bfbf-127">Request body</span></span>
<span data-ttu-id="2bfbf-128">В теле запроса поставляем представление JSON для объекта intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-128">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="2bfbf-129">В следующей таблице показаны свойства, необходимые при создании intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-129">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="2bfbf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bfbf-130">Property</span></span>|<span data-ttu-id="2bfbf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2bfbf-131">Type</span></span>|<span data-ttu-id="2bfbf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2bfbf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bfbf-133">id</span><span class="sxs-lookup"><span data-stu-id="2bfbf-133">id</span></span>|<span data-ttu-id="2bfbf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2bfbf-134">String</span></span>|<span data-ttu-id="2bfbf-135">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="2bfbf-135">Profile Key</span></span>|
|<span data-ttu-id="2bfbf-136">имя профиля</span><span class="sxs-lookup"><span data-stu-id="2bfbf-136">profileName</span></span>|<span data-ttu-id="2bfbf-137">Строка</span><span class="sxs-lookup"><span data-stu-id="2bfbf-137">String</span></span>|<span data-ttu-id="2bfbf-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="2bfbf-138">Name of the profile</span></span>|
|<span data-ttu-id="2bfbf-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="2bfbf-139">profileDescription</span></span>|<span data-ttu-id="2bfbf-140">Строка</span><span class="sxs-lookup"><span data-stu-id="2bfbf-140">String</span></span>|<span data-ttu-id="2bfbf-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="2bfbf-141">Description of the profile</span></span>|
|<span data-ttu-id="2bfbf-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="2bfbf-142">isDefaultProfile</span></span>|<span data-ttu-id="2bfbf-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfbf-143">Boolean</span></span>|<span data-ttu-id="2bfbf-144">Boolean, который представляет, используется ли профиль как по умолчанию или нет</span><span class="sxs-lookup"><span data-stu-id="2bfbf-144">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="2bfbf-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2bfbf-145">createdDateTime</span></span>|<span data-ttu-id="2bfbf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bfbf-146">DateTimeOffset</span></span>|<span data-ttu-id="2bfbf-147">Время создания BrandingProfile</span><span class="sxs-lookup"><span data-stu-id="2bfbf-147">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="2bfbf-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bfbf-148">lastModifiedDateTime</span></span>|<span data-ttu-id="2bfbf-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bfbf-149">DateTimeOffset</span></span>|<span data-ttu-id="2bfbf-150">Время последнего изменения BrandingProfile</span><span class="sxs-lookup"><span data-stu-id="2bfbf-150">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="2bfbf-151">displayName</span><span class="sxs-lookup"><span data-stu-id="2bfbf-151">displayName</span></span>|<span data-ttu-id="2bfbf-152">Строка</span><span class="sxs-lookup"><span data-stu-id="2bfbf-152">String</span></span>|<span data-ttu-id="2bfbf-153">Имя компании или организации, отображаемая конечным пользователям</span><span class="sxs-lookup"><span data-stu-id="2bfbf-153">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="2bfbf-154">themeColor</span><span class="sxs-lookup"><span data-stu-id="2bfbf-154">themeColor</span></span>|[<span data-ttu-id="2bfbf-155">rgbColor</span><span class="sxs-lookup"><span data-stu-id="2bfbf-155">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="2bfbf-156">Основной цвет темы, используемый в приложениях портала компании и веб-портале</span><span class="sxs-lookup"><span data-stu-id="2bfbf-156">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="2bfbf-157">showLogo</span><span class="sxs-lookup"><span data-stu-id="2bfbf-157">showLogo</span></span>|<span data-ttu-id="2bfbf-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfbf-158">Boolean</span></span>|<span data-ttu-id="2bfbf-159">Boolean, который представляет, показаны ли изображения логотипа, предоставленные администратором, или нет.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-159">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="2bfbf-160">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="2bfbf-160">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="2bfbf-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfbf-161">Boolean</span></span>|<span data-ttu-id="2bfbf-162">Boolean, который представляет, будет ли отображаться имя дисплея, предоставленное администратором, рядом с изображением логотипа или нет.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-162">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="2bfbf-163">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="2bfbf-163">themeColorLogo</span></span>|<span data-ttu-id="2bfbf-164">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="2bfbf-164">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="2bfbf-165">Изображение логотипа, отображаемого в приложениях портала компании, которые имеют фон цвета темы за логотипом</span><span class="sxs-lookup"><span data-stu-id="2bfbf-165">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="2bfbf-166">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="2bfbf-166">lightBackgroundLogo</span></span>|[<span data-ttu-id="2bfbf-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2bfbf-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2bfbf-168">Изображение логотипа, отображаемого в приложениях портала компании, которые имеют светлый фон за логотипом</span><span class="sxs-lookup"><span data-stu-id="2bfbf-168">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="2bfbf-169">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="2bfbf-169">landingPageCustomizedImage</span></span>|<span data-ttu-id="2bfbf-170">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="2bfbf-170">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="2bfbf-171">Настраиваемые изображения, отображаемые на странице посадки приложений портала компании</span><span class="sxs-lookup"><span data-stu-id="2bfbf-171">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="2bfbf-172">contactITName</span><span class="sxs-lookup"><span data-stu-id="2bfbf-172">contactITName</span></span>|<span data-ttu-id="2bfbf-173">String</span><span class="sxs-lookup"><span data-stu-id="2bfbf-173">String</span></span>|<span data-ttu-id="2bfbf-174">Имя лица или организации, ответственной за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="2bfbf-174">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="2bfbf-175">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="2bfbf-175">contactITPhoneNumber</span></span>|<span data-ttu-id="2bfbf-176">String</span><span class="sxs-lookup"><span data-stu-id="2bfbf-176">String</span></span>|<span data-ttu-id="2bfbf-177">Номер телефона лица или организации, ответственной за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="2bfbf-177">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="2bfbf-178">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2bfbf-178">contactITEmailAddress</span></span>|<span data-ttu-id="2bfbf-179">String</span><span class="sxs-lookup"><span data-stu-id="2bfbf-179">String</span></span>|<span data-ttu-id="2bfbf-180">Адрес электронной почты лица или организации, ответственной за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="2bfbf-180">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="2bfbf-181">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="2bfbf-181">contactITNotes</span></span>|<span data-ttu-id="2bfbf-182">String</span><span class="sxs-lookup"><span data-stu-id="2bfbf-182">String</span></span>|<span data-ttu-id="2bfbf-183">Текстовые комментарии в отношении лица или организации, ответственной за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="2bfbf-183">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="2bfbf-184">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="2bfbf-184">onlineSupportSiteUrl</span></span>|<span data-ttu-id="2bfbf-185">String</span><span class="sxs-lookup"><span data-stu-id="2bfbf-185">String</span></span>|<span data-ttu-id="2bfbf-186">URL-адрес сайта it-справки компании/организации</span><span class="sxs-lookup"><span data-stu-id="2bfbf-186">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="2bfbf-187">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="2bfbf-187">onlineSupportSiteName</span></span>|<span data-ttu-id="2bfbf-188">String</span><span class="sxs-lookup"><span data-stu-id="2bfbf-188">String</span></span>|<span data-ttu-id="2bfbf-189">Отображение имени сайта it-справки компании/организации</span><span class="sxs-lookup"><span data-stu-id="2bfbf-189">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="2bfbf-190">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="2bfbf-190">privacyUrl</span></span>|<span data-ttu-id="2bfbf-191">String</span><span class="sxs-lookup"><span data-stu-id="2bfbf-191">String</span></span>|<span data-ttu-id="2bfbf-192">URL-адрес политики конфиденциальности компании и организации</span><span class="sxs-lookup"><span data-stu-id="2bfbf-192">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="2bfbf-193">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="2bfbf-193">customPrivacyMessage</span></span>|<span data-ttu-id="2bfbf-194">Строка</span><span class="sxs-lookup"><span data-stu-id="2bfbf-194">String</span></span>|<span data-ttu-id="2bfbf-195">Текстовые комментарии относительно того, к чему администратор не имеет доступа на устройстве</span><span class="sxs-lookup"><span data-stu-id="2bfbf-195">Text comments regarding what the admin doesn't have access to on the device</span></span>|
|<span data-ttu-id="2bfbf-196">customCanSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="2bfbf-196">customCanSeePrivacyMessage</span></span>|<span data-ttu-id="2bfbf-197">Строка</span><span class="sxs-lookup"><span data-stu-id="2bfbf-197">String</span></span>|<span data-ttu-id="2bfbf-198">Текстовые комментарии относительно доступа администратора к устройству</span><span class="sxs-lookup"><span data-stu-id="2bfbf-198">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="2bfbf-199">customCantSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="2bfbf-199">customCantSeePrivacyMessage</span></span>|<span data-ttu-id="2bfbf-200">Строка</span><span class="sxs-lookup"><span data-stu-id="2bfbf-200">String</span></span>|<span data-ttu-id="2bfbf-201">Текстовые комментарии относительно того, к чему администратор не имеет доступа на устройстве</span><span class="sxs-lookup"><span data-stu-id="2bfbf-201">Text comments regarding what the admin doesn't have access to on the device</span></span>|
|<span data-ttu-id="2bfbf-202">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="2bfbf-202">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="2bfbf-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfbf-203">Boolean</span></span>|<span data-ttu-id="2bfbf-204">Boolean, который представляет, отключил ли администратор действие "Удалить устройство" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-204">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="2bfbf-205">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="2bfbf-205">isFactoryResetDisabled</span></span>|<span data-ttu-id="2bfbf-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfbf-206">Boolean</span></span>|<span data-ttu-id="2bfbf-207">Boolean, который представляет, отключил ли администратор действие "Сброс фабрики" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-207">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="2bfbf-208">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="2bfbf-208">companyPortalBlockedActions</span></span>|<span data-ttu-id="2bfbf-209">[коллекция companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="2bfbf-209">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="2bfbf-210">Коллекция заблокированных действий на портале компании в зависимости от типов владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-210">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="2bfbf-211">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="2bfbf-211">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="2bfbf-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfbf-212">Boolean</span></span>|<span data-ttu-id="2bfbf-213">Boolean, который указывает, будут ли корпоративные приложения AzureAD показаны на портале компании</span><span class="sxs-lookup"><span data-stu-id="2bfbf-213">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="2bfbf-214">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="2bfbf-214">showOfficeWebApps</span></span>|<span data-ttu-id="2bfbf-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfbf-215">Boolean</span></span>|<span data-ttu-id="2bfbf-216">Boolean, который указывает, будут ли веб-приложения Office показаны на портале компании</span><span class="sxs-lookup"><span data-stu-id="2bfbf-216">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="2bfbf-217">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="2bfbf-217">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="2bfbf-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfbf-218">Boolean</span></span>|<span data-ttu-id="2bfbf-219">Boolean, который указывает, отправляется ли пользователям push-уведомление при смене типа владения устройствами с личного на корпоративный.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-219">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="2bfbf-220">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="2bfbf-220">enrollmentAvailability</span></span>|[<span data-ttu-id="2bfbf-221">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="2bfbf-221">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="2bfbf-222">Настраиваемый поток регистрации устройств, отображаемый конечному пользователю.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-222">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="2bfbf-223">Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-223">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="2bfbf-224">отключениеClientTelemetry</span><span class="sxs-lookup"><span data-stu-id="2bfbf-224">disableClientTelemetry</span></span>|<span data-ttu-id="2bfbf-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfbf-225">Boolean</span></span>|<span data-ttu-id="2bfbf-226">Применяется к телеметрии, отправленной от всех клиентов в службу Intune.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-226">Applies to telemetry sent from all clients to the Intune service.</span></span> <span data-ttu-id="2bfbf-227">При отключении все упреждающие предупреждения о неполадок в клиенте отключаются, а параметры телеметрии отображаются неактивными или скрытыми для пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-227">When disabled, all proactive troubleshooting and issue warnings within the client are turned off, and telemetry settings appear inactive or hidden to the device user.</span></span>|
|<span data-ttu-id="2bfbf-228">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2bfbf-228">roleScopeTagIds</span></span>|<span data-ttu-id="2bfbf-229">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2bfbf-229">String collection</span></span>|<span data-ttu-id="2bfbf-230">Список тегов области, присвоенных профилю брендинга</span><span class="sxs-lookup"><span data-stu-id="2bfbf-230">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="2bfbf-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bfbf-231">Response</span></span>
<span data-ttu-id="2bfbf-232">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-232">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bfbf-233">Пример</span><span class="sxs-lookup"><span data-stu-id="2bfbf-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bfbf-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bfbf-234">Request</span></span>
<span data-ttu-id="2bfbf-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2bfbf-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bfbf-236">Response</span></span>
<span data-ttu-id="2bfbf-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2bfbf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





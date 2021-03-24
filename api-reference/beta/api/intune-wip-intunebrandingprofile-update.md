---
title: Обновление intuneBrandingProfile
description: Обновление свойств объекта intuneBrandingProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 190a53a273c2ed919d767bd6098a03e135a4effc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133817"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="27a4c-103">Обновление intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="27a4c-103">Update intuneBrandingProfile</span></span>

<span data-ttu-id="27a4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27a4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27a4c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27a4c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27a4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27a4c-107">Обновление свойств объекта [intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="27a4c-107">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27a4c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="27a4c-108">Prerequisites</span></span>
<span data-ttu-id="27a4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27a4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27a4c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27a4c-111">Permission type</span></span>|<span data-ttu-id="27a4c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27a4c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27a4c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27a4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27a4c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27a4c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="27a4c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27a4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27a4c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a4c-116">Not supported.</span></span>|
|<span data-ttu-id="27a4c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="27a4c-117">Application</span></span>|<span data-ttu-id="27a4c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27a4c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27a4c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27a4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="27a4c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="27a4c-120">Request headers</span></span>
|<span data-ttu-id="27a4c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27a4c-121">Header</span></span>|<span data-ttu-id="27a4c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="27a4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27a4c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27a4c-123">Authorization</span></span>|<span data-ttu-id="27a4c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27a4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27a4c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="27a4c-125">Accept</span></span>|<span data-ttu-id="27a4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27a4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27a4c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27a4c-127">Request body</span></span>
<span data-ttu-id="27a4c-128">В теле запроса поставляем представление JSON для [объекта intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="27a4c-128">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="27a4c-129">В следующей таблице показаны свойства, необходимые при создании [intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="27a4c-129">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="27a4c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="27a4c-130">Property</span></span>|<span data-ttu-id="27a4c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="27a4c-131">Type</span></span>|<span data-ttu-id="27a4c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="27a4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27a4c-133">id</span><span class="sxs-lookup"><span data-stu-id="27a4c-133">id</span></span>|<span data-ttu-id="27a4c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="27a4c-134">String</span></span>|<span data-ttu-id="27a4c-135">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="27a4c-135">Profile Key</span></span>|
|<span data-ttu-id="27a4c-136">имя профиля</span><span class="sxs-lookup"><span data-stu-id="27a4c-136">profileName</span></span>|<span data-ttu-id="27a4c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="27a4c-137">String</span></span>|<span data-ttu-id="27a4c-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="27a4c-138">Name of the profile</span></span>|
|<span data-ttu-id="27a4c-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="27a4c-139">profileDescription</span></span>|<span data-ttu-id="27a4c-140">Строка</span><span class="sxs-lookup"><span data-stu-id="27a4c-140">String</span></span>|<span data-ttu-id="27a4c-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="27a4c-141">Description of the profile</span></span>|
|<span data-ttu-id="27a4c-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="27a4c-142">isDefaultProfile</span></span>|<span data-ttu-id="27a4c-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a4c-143">Boolean</span></span>|<span data-ttu-id="27a4c-144">Boolean, который представляет, используется ли профиль как по умолчанию или нет</span><span class="sxs-lookup"><span data-stu-id="27a4c-144">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="27a4c-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27a4c-145">createdDateTime</span></span>|<span data-ttu-id="27a4c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27a4c-146">DateTimeOffset</span></span>|<span data-ttu-id="27a4c-147">Время создания BrandingProfile</span><span class="sxs-lookup"><span data-stu-id="27a4c-147">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="27a4c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27a4c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="27a4c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27a4c-149">DateTimeOffset</span></span>|<span data-ttu-id="27a4c-150">Время последнего изменения BrandingProfile</span><span class="sxs-lookup"><span data-stu-id="27a4c-150">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="27a4c-151">displayName</span><span class="sxs-lookup"><span data-stu-id="27a4c-151">displayName</span></span>|<span data-ttu-id="27a4c-152">Строка</span><span class="sxs-lookup"><span data-stu-id="27a4c-152">String</span></span>|<span data-ttu-id="27a4c-153">Имя компании или организации, отображаемая конечным пользователям</span><span class="sxs-lookup"><span data-stu-id="27a4c-153">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="27a4c-154">themeColor</span><span class="sxs-lookup"><span data-stu-id="27a4c-154">themeColor</span></span>|[<span data-ttu-id="27a4c-155">rgbColor</span><span class="sxs-lookup"><span data-stu-id="27a4c-155">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="27a4c-156">Основной цвет темы, используемый в приложениях портала компании и веб-портале</span><span class="sxs-lookup"><span data-stu-id="27a4c-156">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="27a4c-157">showLogo</span><span class="sxs-lookup"><span data-stu-id="27a4c-157">showLogo</span></span>|<span data-ttu-id="27a4c-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a4c-158">Boolean</span></span>|<span data-ttu-id="27a4c-159">Boolean, который представляет, показаны ли изображения логотипа, предоставленные администратором, или нет.</span><span class="sxs-lookup"><span data-stu-id="27a4c-159">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="27a4c-160">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="27a4c-160">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="27a4c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a4c-161">Boolean</span></span>|<span data-ttu-id="27a4c-162">Boolean, который представляет, будет ли отображаться имя дисплея, предоставленное администратором, рядом с изображением логотипа или нет.</span><span class="sxs-lookup"><span data-stu-id="27a4c-162">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="27a4c-163">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="27a4c-163">themeColorLogo</span></span>|<span data-ttu-id="27a4c-164">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="27a4c-164">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="27a4c-165">Изображение логотипа, отображаемого в приложениях портала компании, которые имеют фон цвета темы за логотипом</span><span class="sxs-lookup"><span data-stu-id="27a4c-165">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="27a4c-166">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="27a4c-166">lightBackgroundLogo</span></span>|[<span data-ttu-id="27a4c-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="27a4c-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="27a4c-168">Изображение логотипа, отображаемого в приложениях портала компании, которые имеют светлый фон за логотипом</span><span class="sxs-lookup"><span data-stu-id="27a4c-168">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="27a4c-169">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="27a4c-169">landingPageCustomizedImage</span></span>|<span data-ttu-id="27a4c-170">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="27a4c-170">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="27a4c-171">Настраиваемые изображения, отображаемые на странице посадки приложений портала компании</span><span class="sxs-lookup"><span data-stu-id="27a4c-171">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="27a4c-172">contactITName</span><span class="sxs-lookup"><span data-stu-id="27a4c-172">contactITName</span></span>|<span data-ttu-id="27a4c-173">String</span><span class="sxs-lookup"><span data-stu-id="27a4c-173">String</span></span>|<span data-ttu-id="27a4c-174">Имя лица или организации, ответственной за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="27a4c-174">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="27a4c-175">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="27a4c-175">contactITPhoneNumber</span></span>|<span data-ttu-id="27a4c-176">String</span><span class="sxs-lookup"><span data-stu-id="27a4c-176">String</span></span>|<span data-ttu-id="27a4c-177">Номер телефона лица или организации, ответственной за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="27a4c-177">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="27a4c-178">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="27a4c-178">contactITEmailAddress</span></span>|<span data-ttu-id="27a4c-179">String</span><span class="sxs-lookup"><span data-stu-id="27a4c-179">String</span></span>|<span data-ttu-id="27a4c-180">Адрес электронной почты лица или организации, ответственной за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="27a4c-180">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="27a4c-181">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="27a4c-181">contactITNotes</span></span>|<span data-ttu-id="27a4c-182">String</span><span class="sxs-lookup"><span data-stu-id="27a4c-182">String</span></span>|<span data-ttu-id="27a4c-183">Текстовые комментарии в отношении лица или организации, ответственной за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="27a4c-183">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="27a4c-184">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="27a4c-184">onlineSupportSiteUrl</span></span>|<span data-ttu-id="27a4c-185">String</span><span class="sxs-lookup"><span data-stu-id="27a4c-185">String</span></span>|<span data-ttu-id="27a4c-186">URL-адрес сайта it-справки компании/организации</span><span class="sxs-lookup"><span data-stu-id="27a4c-186">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="27a4c-187">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="27a4c-187">onlineSupportSiteName</span></span>|<span data-ttu-id="27a4c-188">String</span><span class="sxs-lookup"><span data-stu-id="27a4c-188">String</span></span>|<span data-ttu-id="27a4c-189">Отображение имени сайта it-справки компании/организации</span><span class="sxs-lookup"><span data-stu-id="27a4c-189">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="27a4c-190">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="27a4c-190">privacyUrl</span></span>|<span data-ttu-id="27a4c-191">String</span><span class="sxs-lookup"><span data-stu-id="27a4c-191">String</span></span>|<span data-ttu-id="27a4c-192">URL-адрес политики конфиденциальности компании и организации</span><span class="sxs-lookup"><span data-stu-id="27a4c-192">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="27a4c-193">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="27a4c-193">customPrivacyMessage</span></span>|<span data-ttu-id="27a4c-194">Строка</span><span class="sxs-lookup"><span data-stu-id="27a4c-194">String</span></span>|<span data-ttu-id="27a4c-195">Текстовые комментарии относительно того, к чему администратор не имеет доступа на устройстве</span><span class="sxs-lookup"><span data-stu-id="27a4c-195">Text comments regarding what the admin doesn't have access to on the device</span></span>|
|<span data-ttu-id="27a4c-196">customCanSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="27a4c-196">customCanSeePrivacyMessage</span></span>|<span data-ttu-id="27a4c-197">Строка</span><span class="sxs-lookup"><span data-stu-id="27a4c-197">String</span></span>|<span data-ttu-id="27a4c-198">Текстовые комментарии относительно доступа администратора к устройству</span><span class="sxs-lookup"><span data-stu-id="27a4c-198">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="27a4c-199">customCantSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="27a4c-199">customCantSeePrivacyMessage</span></span>|<span data-ttu-id="27a4c-200">Строка</span><span class="sxs-lookup"><span data-stu-id="27a4c-200">String</span></span>|<span data-ttu-id="27a4c-201">Текстовые комментарии относительно того, к чему администратор не имеет доступа на устройстве</span><span class="sxs-lookup"><span data-stu-id="27a4c-201">Text comments regarding what the admin doesn't have access to on the device</span></span>|
|<span data-ttu-id="27a4c-202">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="27a4c-202">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="27a4c-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a4c-203">Boolean</span></span>|<span data-ttu-id="27a4c-204">Boolean, который представляет, отключил ли администратор действие "Удалить устройство" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="27a4c-204">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="27a4c-205">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="27a4c-205">isFactoryResetDisabled</span></span>|<span data-ttu-id="27a4c-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a4c-206">Boolean</span></span>|<span data-ttu-id="27a4c-207">Boolean, который представляет, отключил ли администратор действие "Сброс фабрики" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="27a4c-207">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="27a4c-208">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="27a4c-208">companyPortalBlockedActions</span></span>|<span data-ttu-id="27a4c-209">[коллекция companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="27a4c-209">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="27a4c-210">Коллекция заблокированных действий на портале компании в зависимости от типов владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="27a4c-210">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="27a4c-211">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="27a4c-211">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="27a4c-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a4c-212">Boolean</span></span>|<span data-ttu-id="27a4c-213">Boolean, который указывает, будут ли корпоративные приложения AzureAD показаны на портале компании</span><span class="sxs-lookup"><span data-stu-id="27a4c-213">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="27a4c-214">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="27a4c-214">showOfficeWebApps</span></span>|<span data-ttu-id="27a4c-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a4c-215">Boolean</span></span>|<span data-ttu-id="27a4c-216">Boolean, который указывает, будут ли веб-приложения Office показаны на портале компании</span><span class="sxs-lookup"><span data-stu-id="27a4c-216">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="27a4c-217">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="27a4c-217">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="27a4c-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a4c-218">Boolean</span></span>|<span data-ttu-id="27a4c-219">Boolean, который указывает, отправляется ли пользователям push-уведомление при смене типа владения устройствами с личного на корпоративный.</span><span class="sxs-lookup"><span data-stu-id="27a4c-219">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="27a4c-220">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="27a4c-220">enrollmentAvailability</span></span>|[<span data-ttu-id="27a4c-221">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="27a4c-221">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="27a4c-222">Настраиваемый поток регистрации устройств, отображаемый конечному пользователю.</span><span class="sxs-lookup"><span data-stu-id="27a4c-222">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="27a4c-223">Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="27a4c-223">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="27a4c-224">отключениеClientTelemetry</span><span class="sxs-lookup"><span data-stu-id="27a4c-224">disableClientTelemetry</span></span>|<span data-ttu-id="27a4c-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a4c-225">Boolean</span></span>|<span data-ttu-id="27a4c-226">Применяется к телеметрии, отправленной от всех клиентов в службу Intune.</span><span class="sxs-lookup"><span data-stu-id="27a4c-226">Applies to telemetry sent from all clients to the Intune service.</span></span> <span data-ttu-id="27a4c-227">При отключении все упреждающие предупреждения о неполадок в клиенте отключаются, а параметры телеметрии отображаются неактивными или скрытыми для пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="27a4c-227">When disabled, all proactive troubleshooting and issue warnings within the client are turned off, and telemetry settings appear inactive or hidden to the device user.</span></span>|
|<span data-ttu-id="27a4c-228">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="27a4c-228">roleScopeTagIds</span></span>|<span data-ttu-id="27a4c-229">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="27a4c-229">String collection</span></span>|<span data-ttu-id="27a4c-230">Список тегов области, присвоенных профилю брендинга</span><span class="sxs-lookup"><span data-stu-id="27a4c-230">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="27a4c-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="27a4c-231">Response</span></span>
<span data-ttu-id="27a4c-232">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="27a4c-232">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27a4c-233">Пример</span><span class="sxs-lookup"><span data-stu-id="27a4c-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="27a4c-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="27a4c-234">Request</span></span>
<span data-ttu-id="27a4c-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27a4c-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
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

### <a name="response"></a><span data-ttu-id="27a4c-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="27a4c-236">Response</span></span>
<span data-ttu-id="27a4c-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27a4c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





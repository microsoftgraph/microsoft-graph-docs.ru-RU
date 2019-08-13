---
title: Создание Интунебрандингпрофиле
description: Создание нового объекта Интунебрандингпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 98245e618ef6c821502109164e2c726657477b91
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350183"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="10ab1-103">Создание Интунебрандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="10ab1-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="10ab1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ab1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10ab1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10ab1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10ab1-106">Создание нового объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="10ab1-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10ab1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="10ab1-107">Prerequisites</span></span>
<span data-ttu-id="10ab1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10ab1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10ab1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10ab1-110">Permission type</span></span>|<span data-ttu-id="10ab1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10ab1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10ab1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10ab1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10ab1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10ab1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="10ab1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10ab1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10ab1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ab1-115">Not supported.</span></span>|
|<span data-ttu-id="10ab1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10ab1-116">Application</span></span>|<span data-ttu-id="10ab1-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10ab1-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10ab1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10ab1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="10ab1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10ab1-119">Request headers</span></span>
|<span data-ttu-id="10ab1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10ab1-120">Header</span></span>|<span data-ttu-id="10ab1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="10ab1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10ab1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10ab1-122">Authorization</span></span>|<span data-ttu-id="10ab1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10ab1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10ab1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="10ab1-124">Accept</span></span>|<span data-ttu-id="10ab1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10ab1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10ab1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10ab1-126">Request body</span></span>
<span data-ttu-id="10ab1-127">В тексте запроса добавьте представление объекта Интунебрандингпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10ab1-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="10ab1-128">В следующей таблице приведены свойства, необходимые при создании Интунебрандингпрофиле.</span><span class="sxs-lookup"><span data-stu-id="10ab1-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="10ab1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="10ab1-129">Property</span></span>|<span data-ttu-id="10ab1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="10ab1-130">Type</span></span>|<span data-ttu-id="10ab1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="10ab1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10ab1-132">id</span><span class="sxs-lookup"><span data-stu-id="10ab1-132">id</span></span>|<span data-ttu-id="10ab1-133">String</span><span class="sxs-lookup"><span data-stu-id="10ab1-133">String</span></span>|<span data-ttu-id="10ab1-134">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="10ab1-134">Profile Key</span></span>|
|<span data-ttu-id="10ab1-135">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="10ab1-135">profileName</span></span>|<span data-ttu-id="10ab1-136">String</span><span class="sxs-lookup"><span data-stu-id="10ab1-136">String</span></span>|<span data-ttu-id="10ab1-137">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="10ab1-137">Name of the profile</span></span>|
|<span data-ttu-id="10ab1-138">профиледескриптион</span><span class="sxs-lookup"><span data-stu-id="10ab1-138">profileDescription</span></span>|<span data-ttu-id="10ab1-139">String</span><span class="sxs-lookup"><span data-stu-id="10ab1-139">String</span></span>|<span data-ttu-id="10ab1-140">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="10ab1-140">Description of the profile</span></span>|
|<span data-ttu-id="10ab1-141">исдефаултпрофиле</span><span class="sxs-lookup"><span data-stu-id="10ab1-141">isDefaultProfile</span></span>|<span data-ttu-id="10ab1-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="10ab1-142">Boolean</span></span>|<span data-ttu-id="10ab1-143">Логическое значение, указывающее, используется ли профиль по умолчанию или нет</span><span class="sxs-lookup"><span data-stu-id="10ab1-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="10ab1-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10ab1-144">createdDateTime</span></span>|<span data-ttu-id="10ab1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10ab1-145">DateTimeOffset</span></span>|<span data-ttu-id="10ab1-146">Время создания Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="10ab1-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="10ab1-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10ab1-147">lastModifiedDateTime</span></span>|<span data-ttu-id="10ab1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10ab1-148">DateTimeOffset</span></span>|<span data-ttu-id="10ab1-149">Время последнего изменения Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="10ab1-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="10ab1-150">displayName</span><span class="sxs-lookup"><span data-stu-id="10ab1-150">displayName</span></span>|<span data-ttu-id="10ab1-151">Строка</span><span class="sxs-lookup"><span data-stu-id="10ab1-151">String</span></span>|<span data-ttu-id="10ab1-152">Название компании или организации, которое отображается для конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="10ab1-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="10ab1-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="10ab1-153">contactITName</span></span>|<span data-ttu-id="10ab1-154">String</span><span class="sxs-lookup"><span data-stu-id="10ab1-154">String</span></span>|<span data-ttu-id="10ab1-155">Имя пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="10ab1-155">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="10ab1-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="10ab1-156">contactITPhoneNumber</span></span>|<span data-ttu-id="10ab1-157">String</span><span class="sxs-lookup"><span data-stu-id="10ab1-157">String</span></span>|<span data-ttu-id="10ab1-158">Номер телефона пользователя или организации, ответственного за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="10ab1-158">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="10ab1-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="10ab1-159">contactITEmailAddress</span></span>|<span data-ttu-id="10ab1-160">String</span><span class="sxs-lookup"><span data-stu-id="10ab1-160">String</span></span>|<span data-ttu-id="10ab1-161">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="10ab1-161">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="10ab1-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="10ab1-162">contactITNotes</span></span>|<span data-ttu-id="10ab1-163">String</span><span class="sxs-lookup"><span data-stu-id="10ab1-163">String</span></span>|<span data-ttu-id="10ab1-164">Текстовые комментарии о лице или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="10ab1-164">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="10ab1-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="10ab1-165">privacyUrl</span></span>|<span data-ttu-id="10ab1-166">String</span><span class="sxs-lookup"><span data-stu-id="10ab1-166">String</span></span>|<span data-ttu-id="10ab1-167">URL-адрес политики конфиденциальности компании или Организации</span><span class="sxs-lookup"><span data-stu-id="10ab1-167">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="10ab1-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="10ab1-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="10ab1-169">String</span><span class="sxs-lookup"><span data-stu-id="10ab1-169">String</span></span>|<span data-ttu-id="10ab1-170">URL-адрес сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="10ab1-170">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="10ab1-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="10ab1-171">onlineSupportSiteName</span></span>|<span data-ttu-id="10ab1-172">String</span><span class="sxs-lookup"><span data-stu-id="10ab1-172">String</span></span>|<span data-ttu-id="10ab1-173">Отображаемое имя сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="10ab1-173">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="10ab1-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="10ab1-174">themeColor</span></span>|[<span data-ttu-id="10ab1-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="10ab1-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="10ab1-176">Основной цвет темы, используемый в приложениях портала компании и на веб-портале</span><span class="sxs-lookup"><span data-stu-id="10ab1-176">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="10ab1-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="10ab1-177">showLogo</span></span>|<span data-ttu-id="10ab1-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="10ab1-178">Boolean</span></span>|<span data-ttu-id="10ab1-179">Логическое значение, указывающее, отображаются ли изображения логотипа, предоставленные администратором.</span><span class="sxs-lookup"><span data-stu-id="10ab1-179">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="10ab1-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="10ab1-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="10ab1-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="10ab1-181">Boolean</span></span>|<span data-ttu-id="10ab1-182">Логическое значение, указывающее, будет ли отображаться отображаемое имя, предоставленное администратором, рядом с изображением логотипа.</span><span class="sxs-lookup"><span data-stu-id="10ab1-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="10ab1-183">семеколорлого</span><span class="sxs-lookup"><span data-stu-id="10ab1-183">themeColorLogo</span></span>|<span data-ttu-id="10ab1-184">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="10ab1-184">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="10ab1-185">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть фоновый цвет темы позади логотипа</span><span class="sxs-lookup"><span data-stu-id="10ab1-185">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="10ab1-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="10ab1-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="10ab1-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="10ab1-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="10ab1-188">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть светлый фон позади логотипа</span><span class="sxs-lookup"><span data-stu-id="10ab1-188">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="10ab1-189">ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="10ab1-189">landingPageCustomizedImage</span></span>|<span data-ttu-id="10ab1-190">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="10ab1-190">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="10ab1-191">Настраиваемое изображение, отображаемое на начальной странице "приложения корпоративного портала"</span><span class="sxs-lookup"><span data-stu-id="10ab1-191">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="10ab1-192">кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="10ab1-192">customPrivacyMessage</span></span>|<span data-ttu-id="10ab1-193">String</span><span class="sxs-lookup"><span data-stu-id="10ab1-193">String</span></span>|<span data-ttu-id="10ab1-194">Текстовые комментарии относительно того, что у администратора есть доступ к устройству.</span><span class="sxs-lookup"><span data-stu-id="10ab1-194">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="10ab1-195">исремоведевицедисаблед</span><span class="sxs-lookup"><span data-stu-id="10ab1-195">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="10ab1-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="10ab1-196">Boolean</span></span>|<span data-ttu-id="10ab1-197">Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="10ab1-197">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="10ab1-198">исфакториресетдисаблед</span><span class="sxs-lookup"><span data-stu-id="10ab1-198">isFactoryResetDisabled</span></span>|<span data-ttu-id="10ab1-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="10ab1-199">Boolean</span></span>|<span data-ttu-id="10ab1-200">Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="10ab1-200">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|



## <a name="response"></a><span data-ttu-id="10ab1-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ab1-201">Response</span></span>
<span data-ttu-id="10ab1-202">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10ab1-202">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10ab1-203">Пример</span><span class="sxs-lookup"><span data-stu-id="10ab1-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="10ab1-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="10ab1-204">Request</span></span>
<span data-ttu-id="10ab1-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10ab1-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1334

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
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
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="10ab1-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ab1-206">Response</span></span>
<span data-ttu-id="10ab1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10ab1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1506

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
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
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true
}
```







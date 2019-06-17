---
title: Обновление Интунебрандингпрофиле
description: Обновление свойств объекта Интунебрандингпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b8d5f80610692aa46b52a2e00101a662549dd32a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990583"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="9b831-103">Обновление Интунебрандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="9b831-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="9b831-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b831-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b831-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b831-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b831-106">Обновление свойств объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9b831-106">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b831-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b831-107">Prerequisites</span></span>
<span data-ttu-id="9b831-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b831-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b831-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b831-110">Permission type</span></span>|<span data-ttu-id="9b831-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b831-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b831-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b831-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b831-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b831-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9b831-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b831-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b831-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b831-115">Not supported.</span></span>|
|<span data-ttu-id="9b831-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b831-116">Application</span></span>|<span data-ttu-id="9b831-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b831-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b831-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b831-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="9b831-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b831-119">Request headers</span></span>
|<span data-ttu-id="9b831-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b831-120">Header</span></span>|<span data-ttu-id="9b831-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9b831-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b831-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b831-122">Authorization</span></span>|<span data-ttu-id="9b831-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b831-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b831-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9b831-124">Accept</span></span>|<span data-ttu-id="9b831-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b831-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b831-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9b831-126">Request body</span></span>
<span data-ttu-id="9b831-127">В тексте запроса добавьте представление объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b831-127">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="9b831-128">В следующей таблице приведены свойства, необходимые при создании [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="9b831-128">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="9b831-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b831-129">Property</span></span>|<span data-ttu-id="9b831-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9b831-130">Type</span></span>|<span data-ttu-id="9b831-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9b831-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b831-132">id</span><span class="sxs-lookup"><span data-stu-id="9b831-132">id</span></span>|<span data-ttu-id="9b831-133">String</span><span class="sxs-lookup"><span data-stu-id="9b831-133">String</span></span>|<span data-ttu-id="9b831-134">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="9b831-134">Profile Key</span></span>|
|<span data-ttu-id="9b831-135">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="9b831-135">profileName</span></span>|<span data-ttu-id="9b831-136">String</span><span class="sxs-lookup"><span data-stu-id="9b831-136">String</span></span>|<span data-ttu-id="9b831-137">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="9b831-137">Name of the profile</span></span>|
|<span data-ttu-id="9b831-138">Профиледескриптион</span><span class="sxs-lookup"><span data-stu-id="9b831-138">profileDescription</span></span>|<span data-ttu-id="9b831-139">String</span><span class="sxs-lookup"><span data-stu-id="9b831-139">String</span></span>|<span data-ttu-id="9b831-140">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="9b831-140">Description of the profile</span></span>|
|<span data-ttu-id="9b831-141">Исдефаултпрофиле</span><span class="sxs-lookup"><span data-stu-id="9b831-141">isDefaultProfile</span></span>|<span data-ttu-id="9b831-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b831-142">Boolean</span></span>|<span data-ttu-id="9b831-143">Логическое значение, указывающее, используется ли профиль по умолчанию или нет</span><span class="sxs-lookup"><span data-stu-id="9b831-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="9b831-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b831-144">createdDateTime</span></span>|<span data-ttu-id="9b831-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b831-145">DateTimeOffset</span></span>|<span data-ttu-id="9b831-146">Время создания Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="9b831-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="9b831-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b831-147">lastModifiedDateTime</span></span>|<span data-ttu-id="9b831-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b831-148">DateTimeOffset</span></span>|<span data-ttu-id="9b831-149">Время последнего изменения Брандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="9b831-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="9b831-150">displayName</span><span class="sxs-lookup"><span data-stu-id="9b831-150">displayName</span></span>|<span data-ttu-id="9b831-151">Строка</span><span class="sxs-lookup"><span data-stu-id="9b831-151">String</span></span>|<span data-ttu-id="9b831-152">Название компании или организации, которое отображается для конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="9b831-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="9b831-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="9b831-153">contactITName</span></span>|<span data-ttu-id="9b831-154">String</span><span class="sxs-lookup"><span data-stu-id="9b831-154">String</span></span>|<span data-ttu-id="9b831-155">Имя пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="9b831-155">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="9b831-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="9b831-156">contactITPhoneNumber</span></span>|<span data-ttu-id="9b831-157">String</span><span class="sxs-lookup"><span data-stu-id="9b831-157">String</span></span>|<span data-ttu-id="9b831-158">Номер телефона пользователя или организации, ответственного за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="9b831-158">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="9b831-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="9b831-159">contactITEmailAddress</span></span>|<span data-ttu-id="9b831-160">String</span><span class="sxs-lookup"><span data-stu-id="9b831-160">String</span></span>|<span data-ttu-id="9b831-161">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="9b831-161">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="9b831-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="9b831-162">contactITNotes</span></span>|<span data-ttu-id="9b831-163">String</span><span class="sxs-lookup"><span data-stu-id="9b831-163">String</span></span>|<span data-ttu-id="9b831-164">Текстовые комментарии о лице или организации, ответственных за ИТ-поддержку</span><span class="sxs-lookup"><span data-stu-id="9b831-164">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="9b831-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="9b831-165">privacyUrl</span></span>|<span data-ttu-id="9b831-166">String</span><span class="sxs-lookup"><span data-stu-id="9b831-166">String</span></span>|<span data-ttu-id="9b831-167">URL-адрес политики конфиденциальности компании или Организации</span><span class="sxs-lookup"><span data-stu-id="9b831-167">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="9b831-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="9b831-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="9b831-169">String</span><span class="sxs-lookup"><span data-stu-id="9b831-169">String</span></span>|<span data-ttu-id="9b831-170">URL-адрес сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="9b831-170">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="9b831-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="9b831-171">onlineSupportSiteName</span></span>|<span data-ttu-id="9b831-172">String</span><span class="sxs-lookup"><span data-stu-id="9b831-172">String</span></span>|<span data-ttu-id="9b831-173">Отображаемое имя сайта ИТ-службы технической поддержки компании или Организации</span><span class="sxs-lookup"><span data-stu-id="9b831-173">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="9b831-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="9b831-174">themeColor</span></span>|[<span data-ttu-id="9b831-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="9b831-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="9b831-176">Основной цвет темы, используемый в приложениях портала компании и на веб-портале</span><span class="sxs-lookup"><span data-stu-id="9b831-176">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="9b831-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="9b831-177">showLogo</span></span>|<span data-ttu-id="9b831-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b831-178">Boolean</span></span>|<span data-ttu-id="9b831-179">Логическое значение, указывающее, отображаются ли изображения логотипа, предоставленные администратором.</span><span class="sxs-lookup"><span data-stu-id="9b831-179">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="9b831-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="9b831-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="9b831-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b831-181">Boolean</span></span>|<span data-ttu-id="9b831-182">Логическое значение, указывающее, будет ли отображаться отображаемое имя, предоставленное администратором, рядом с изображением логотипа.</span><span class="sxs-lookup"><span data-stu-id="9b831-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="9b831-183">Семеколорлого</span><span class="sxs-lookup"><span data-stu-id="9b831-183">themeColorLogo</span></span>|<span data-ttu-id="9b831-184">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="9b831-184">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="9b831-185">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть фоновый цвет темы позади логотипа</span><span class="sxs-lookup"><span data-stu-id="9b831-185">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="9b831-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="9b831-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="9b831-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9b831-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9b831-188">Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть светлый фон позади логотипа</span><span class="sxs-lookup"><span data-stu-id="9b831-188">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="9b831-189">Ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="9b831-189">landingPageCustomizedImage</span></span>|<span data-ttu-id="9b831-190">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="9b831-190">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="9b831-191">Настраиваемое изображение, отображаемое на начальной странице "приложения корпоративного портала"</span><span class="sxs-lookup"><span data-stu-id="9b831-191">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="9b831-192">Кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="9b831-192">customPrivacyMessage</span></span>|<span data-ttu-id="9b831-193">String</span><span class="sxs-lookup"><span data-stu-id="9b831-193">String</span></span>|<span data-ttu-id="9b831-194">Текстовые комментарии относительно того, что у администратора есть доступ к устройству.</span><span class="sxs-lookup"><span data-stu-id="9b831-194">Text comments regarding what the admin has access to on the device</span></span>|



## <a name="response"></a><span data-ttu-id="9b831-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b831-195">Response</span></span>
<span data-ttu-id="9b831-196">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b831-196">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b831-197">Пример</span><span class="sxs-lookup"><span data-stu-id="9b831-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b831-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b831-198">Request</span></span>
<span data-ttu-id="9b831-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b831-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1264

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
  "customPrivacyMessage": "Custom Privacy Message value"
}
```

### <a name="response"></a><span data-ttu-id="9b831-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b831-200">Response</span></span>
<span data-ttu-id="9b831-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b831-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1436

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
  "customPrivacyMessage": "Custom Privacy Message value"
}
```






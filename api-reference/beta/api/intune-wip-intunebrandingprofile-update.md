---
title: Обновление intuneBrandingProfile
description: Обновление свойства объекта intuneBrandingProfile.
ms.openlocfilehash: 094de592e0e8d80472f1b0c6ed3d751ac79ba863
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082127"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="4b024-103">Обновление intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="4b024-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="4b024-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b024-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b024-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b024-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b024-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4b024-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b024-107">Обновление свойства объекта [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4b024-107">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b024-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b024-108">Prerequisites</span></span>
<span data-ttu-id="4b024-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b024-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b024-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b024-111">Permission type</span></span>|<span data-ttu-id="4b024-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b024-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b024-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b024-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b024-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b024-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4b024-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b024-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b024-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b024-116">Not supported.</span></span>|
|<span data-ttu-id="4b024-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b024-117">Application</span></span>|<span data-ttu-id="4b024-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b024-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b024-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b024-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="4b024-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b024-120">Request headers</span></span>
|<span data-ttu-id="4b024-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b024-121">Header</span></span>|<span data-ttu-id="4b024-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b024-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b024-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b024-123">Authorization</span></span>|<span data-ttu-id="4b024-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4b024-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b024-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b024-125">Accept</span></span>|<span data-ttu-id="4b024-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b024-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b024-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b024-127">Request body</span></span>
<span data-ttu-id="4b024-128">В тексте запроса укажите представление JSON для объекта [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4b024-128">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="4b024-129">В следующей таблице показаны свойства, которые необходимы для создания [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="4b024-129">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="4b024-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b024-130">Property</span></span>|<span data-ttu-id="4b024-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b024-131">Type</span></span>|<span data-ttu-id="4b024-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b024-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b024-133">id</span><span class="sxs-lookup"><span data-stu-id="4b024-133">id</span></span>|<span data-ttu-id="4b024-134">String</span><span class="sxs-lookup"><span data-stu-id="4b024-134">String</span></span>|<span data-ttu-id="4b024-135">Клавиша профилей</span><span class="sxs-lookup"><span data-stu-id="4b024-135">Profile Key</span></span>|
|<span data-ttu-id="4b024-136">Имя_профиля</span><span class="sxs-lookup"><span data-stu-id="4b024-136">profileName</span></span>|<span data-ttu-id="4b024-137">String</span><span class="sxs-lookup"><span data-stu-id="4b024-137">String</span></span>|<span data-ttu-id="4b024-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="4b024-138">Name of the profile</span></span>|
|<span data-ttu-id="4b024-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="4b024-139">profileDescription</span></span>|<span data-ttu-id="4b024-140">String</span><span class="sxs-lookup"><span data-stu-id="4b024-140">String</span></span>|<span data-ttu-id="4b024-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="4b024-141">Description of the profile</span></span>|
|<span data-ttu-id="4b024-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="4b024-142">isDefaultProfile</span></span>|<span data-ttu-id="4b024-143">Логический</span><span class="sxs-lookup"><span data-stu-id="4b024-143">Boolean</span></span>|<span data-ttu-id="4b024-144">Представляет при использовании профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4b024-144">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="4b024-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b024-145">createdDateTime</span></span>|<span data-ttu-id="4b024-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b024-146">DateTimeOffset</span></span>|<span data-ttu-id="4b024-147">При создании BrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="4b024-147">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="4b024-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b024-148">lastModifiedDateTime</span></span>|<span data-ttu-id="4b024-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b024-149">DateTimeOffset</span></span>|<span data-ttu-id="4b024-150">Время последнего изменения BrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="4b024-150">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="4b024-151">displayName</span><span class="sxs-lookup"><span data-stu-id="4b024-151">displayName</span></span>|<span data-ttu-id="4b024-152">String</span><span class="sxs-lookup"><span data-stu-id="4b024-152">String</span></span>|<span data-ttu-id="4b024-153">Название компании или организации, которое отображается пользователям.</span><span class="sxs-lookup"><span data-stu-id="4b024-153">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="4b024-154">contactITName</span><span class="sxs-lookup"><span data-stu-id="4b024-154">contactITName</span></span>|<span data-ttu-id="4b024-155">String</span><span class="sxs-lookup"><span data-stu-id="4b024-155">String</span></span>|<span data-ttu-id="4b024-156">Имя пользователя или название организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="4b024-156">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="4b024-157">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="4b024-157">contactITPhoneNumber</span></span>|<span data-ttu-id="4b024-158">String</span><span class="sxs-lookup"><span data-stu-id="4b024-158">String</span></span>|<span data-ttu-id="4b024-159">Номер телефона пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="4b024-159">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="4b024-160">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="4b024-160">contactITEmailAddress</span></span>|<span data-ttu-id="4b024-161">String</span><span class="sxs-lookup"><span data-stu-id="4b024-161">String</span></span>|<span data-ttu-id="4b024-162">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="4b024-162">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="4b024-163">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="4b024-163">contactITNotes</span></span>|<span data-ttu-id="4b024-164">String</span><span class="sxs-lookup"><span data-stu-id="4b024-164">String</span></span>|<span data-ttu-id="4b024-165">Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="4b024-165">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="4b024-166">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="4b024-166">privacyUrl</span></span>|<span data-ttu-id="4b024-167">String</span><span class="sxs-lookup"><span data-stu-id="4b024-167">String</span></span>|<span data-ttu-id="4b024-168">URL-адрес страницы с политикой конфиденциальности компании или организации.</span><span class="sxs-lookup"><span data-stu-id="4b024-168">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="4b024-169">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="4b024-169">onlineSupportSiteUrl</span></span>|<span data-ttu-id="4b024-170">String</span><span class="sxs-lookup"><span data-stu-id="4b024-170">String</span></span>|<span data-ttu-id="4b024-171">URL-адрес сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="4b024-171">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="4b024-172">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="4b024-172">onlineSupportSiteName</span></span>|<span data-ttu-id="4b024-173">String</span><span class="sxs-lookup"><span data-stu-id="4b024-173">String</span></span>|<span data-ttu-id="4b024-174">Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="4b024-174">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="4b024-175">themeColor</span><span class="sxs-lookup"><span data-stu-id="4b024-175">themeColor</span></span>|[<span data-ttu-id="4b024-176">rgbColor</span><span class="sxs-lookup"><span data-stu-id="4b024-176">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="4b024-177">Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.</span><span class="sxs-lookup"><span data-stu-id="4b024-177">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="4b024-178">showLogo</span><span class="sxs-lookup"><span data-stu-id="4b024-178">showLogo</span></span>|<span data-ttu-id="4b024-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b024-179">Boolean</span></span>|<span data-ttu-id="4b024-180">Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.</span><span class="sxs-lookup"><span data-stu-id="4b024-180">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="4b024-181">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="4b024-181">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="4b024-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b024-182">Boolean</span></span>|<span data-ttu-id="4b024-183">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="4b024-183">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="4b024-184">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="4b024-184">themeColorLogo</span></span>|<span data-ttu-id="4b024-185">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="4b024-185">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="4b024-186">Изображения эмблемы, отображаемые в приложениях портала компании на темы цвет фона.</span><span class="sxs-lookup"><span data-stu-id="4b024-186">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="4b024-187">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="4b024-187">lightBackgroundLogo</span></span>|[<span data-ttu-id="4b024-188">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4b024-188">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4b024-189">Изображения эмблемы, отображаемые в приложениях портала компании на светлый фон.</span><span class="sxs-lookup"><span data-stu-id="4b024-189">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="4b024-190">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="4b024-190">landingPageCustomizedImage</span></span>|<span data-ttu-id="4b024-191">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="4b024-191">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="4b024-192">Настраиваемая изображение, отображаемое в приложениях портал "Компания" Главная страница</span><span class="sxs-lookup"><span data-stu-id="4b024-192">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="4b024-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b024-193">Response</span></span>
<span data-ttu-id="4b024-194">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4b024-194">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b024-195">Пример</span><span class="sxs-lookup"><span data-stu-id="4b024-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b024-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b024-196">Request</span></span>
<span data-ttu-id="4b024-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b024-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1209

{
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
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
  }
}
```

### <a name="response"></a><span data-ttu-id="4b024-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b024-198">Response</span></span>
<span data-ttu-id="4b024-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4b024-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1377

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
  }
}
```






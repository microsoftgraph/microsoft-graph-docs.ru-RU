---
title: Создание intuneBrandingProfile
description: Создание нового объекта intuneBrandingProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5e8ec4990b333d18dd761772627665c5ecb04179
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862022"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="c9482-103">Создание intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="c9482-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="c9482-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9482-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9482-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9482-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9482-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c9482-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9482-107">Создание нового объекта [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c9482-107">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9482-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c9482-108">Prerequisites</span></span>
<span data-ttu-id="c9482-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9482-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9482-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9482-111">Permission type</span></span>|<span data-ttu-id="c9482-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9482-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9482-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9482-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9482-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9482-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c9482-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9482-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9482-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9482-116">Not supported.</span></span>|
|<span data-ttu-id="c9482-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9482-117">Application</span></span>|<span data-ttu-id="c9482-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9482-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9482-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9482-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c9482-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9482-120">Request headers</span></span>
|<span data-ttu-id="c9482-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9482-121">Header</span></span>|<span data-ttu-id="c9482-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c9482-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9482-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9482-123">Authorization</span></span>|<span data-ttu-id="c9482-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c9482-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9482-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9482-125">Accept</span></span>|<span data-ttu-id="c9482-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9482-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9482-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9482-127">Request body</span></span>
<span data-ttu-id="c9482-128">В тексте запроса укажите представление JSON для объекта intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="c9482-128">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="c9482-129">В следующей таблице показаны свойства, которые необходимы для создания intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="c9482-129">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="c9482-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9482-130">Property</span></span>|<span data-ttu-id="c9482-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c9482-131">Type</span></span>|<span data-ttu-id="c9482-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c9482-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9482-133">id</span><span class="sxs-lookup"><span data-stu-id="c9482-133">id</span></span>|<span data-ttu-id="c9482-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c9482-134">String</span></span>|<span data-ttu-id="c9482-135">Клавиша профилей</span><span class="sxs-lookup"><span data-stu-id="c9482-135">Profile Key</span></span>|
|<span data-ttu-id="c9482-136">Имя_профиля</span><span class="sxs-lookup"><span data-stu-id="c9482-136">profileName</span></span>|<span data-ttu-id="c9482-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c9482-137">String</span></span>|<span data-ttu-id="c9482-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="c9482-138">Name of the profile</span></span>|
|<span data-ttu-id="c9482-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="c9482-139">profileDescription</span></span>|<span data-ttu-id="c9482-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c9482-140">String</span></span>|<span data-ttu-id="c9482-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="c9482-141">Description of the profile</span></span>|
|<span data-ttu-id="c9482-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="c9482-142">isDefaultProfile</span></span>|<span data-ttu-id="c9482-143">Логический</span><span class="sxs-lookup"><span data-stu-id="c9482-143">Boolean</span></span>|<span data-ttu-id="c9482-144">Представляет при использовании профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c9482-144">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="c9482-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9482-145">createdDateTime</span></span>|<span data-ttu-id="c9482-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9482-146">DateTimeOffset</span></span>|<span data-ttu-id="c9482-147">При создании BrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="c9482-147">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="c9482-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9482-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c9482-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9482-149">DateTimeOffset</span></span>|<span data-ttu-id="c9482-150">Время последнего изменения BrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="c9482-150">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="c9482-151">displayName</span><span class="sxs-lookup"><span data-stu-id="c9482-151">displayName</span></span>|<span data-ttu-id="c9482-152">String</span><span class="sxs-lookup"><span data-stu-id="c9482-152">String</span></span>|<span data-ttu-id="c9482-153">Название компании или организации, которое отображается пользователям.</span><span class="sxs-lookup"><span data-stu-id="c9482-153">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="c9482-154">contactITName</span><span class="sxs-lookup"><span data-stu-id="c9482-154">contactITName</span></span>|<span data-ttu-id="c9482-155">String</span><span class="sxs-lookup"><span data-stu-id="c9482-155">String</span></span>|<span data-ttu-id="c9482-156">Имя пользователя или название организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="c9482-156">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c9482-157">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="c9482-157">contactITPhoneNumber</span></span>|<span data-ttu-id="c9482-158">String</span><span class="sxs-lookup"><span data-stu-id="c9482-158">String</span></span>|<span data-ttu-id="c9482-159">Номер телефона пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="c9482-159">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c9482-160">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c9482-160">contactITEmailAddress</span></span>|<span data-ttu-id="c9482-161">String</span><span class="sxs-lookup"><span data-stu-id="c9482-161">String</span></span>|<span data-ttu-id="c9482-162">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="c9482-162">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c9482-163">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="c9482-163">contactITNotes</span></span>|<span data-ttu-id="c9482-164">String</span><span class="sxs-lookup"><span data-stu-id="c9482-164">String</span></span>|<span data-ttu-id="c9482-165">Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="c9482-165">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c9482-166">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="c9482-166">privacyUrl</span></span>|<span data-ttu-id="c9482-167">String</span><span class="sxs-lookup"><span data-stu-id="c9482-167">String</span></span>|<span data-ttu-id="c9482-168">URL-адрес страницы с политикой конфиденциальности компании или организации.</span><span class="sxs-lookup"><span data-stu-id="c9482-168">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="c9482-169">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="c9482-169">onlineSupportSiteUrl</span></span>|<span data-ttu-id="c9482-170">String</span><span class="sxs-lookup"><span data-stu-id="c9482-170">String</span></span>|<span data-ttu-id="c9482-171">URL-адрес сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="c9482-171">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="c9482-172">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="c9482-172">onlineSupportSiteName</span></span>|<span data-ttu-id="c9482-173">String</span><span class="sxs-lookup"><span data-stu-id="c9482-173">String</span></span>|<span data-ttu-id="c9482-174">Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="c9482-174">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="c9482-175">themeColor</span><span class="sxs-lookup"><span data-stu-id="c9482-175">themeColor</span></span>|[<span data-ttu-id="c9482-176">rgbColor</span><span class="sxs-lookup"><span data-stu-id="c9482-176">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="c9482-177">Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.</span><span class="sxs-lookup"><span data-stu-id="c9482-177">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="c9482-178">showLogo</span><span class="sxs-lookup"><span data-stu-id="c9482-178">showLogo</span></span>|<span data-ttu-id="c9482-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9482-179">Boolean</span></span>|<span data-ttu-id="c9482-180">Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.</span><span class="sxs-lookup"><span data-stu-id="c9482-180">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="c9482-181">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="c9482-181">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="c9482-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9482-182">Boolean</span></span>|<span data-ttu-id="c9482-183">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c9482-183">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="c9482-184">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="c9482-184">themeColorLogo</span></span>|<span data-ttu-id="c9482-185">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="c9482-185">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="c9482-186">Изображения эмблемы, отображаемые в приложениях портала компании на темы цвет фона.</span><span class="sxs-lookup"><span data-stu-id="c9482-186">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="c9482-187">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="c9482-187">lightBackgroundLogo</span></span>|[<span data-ttu-id="c9482-188">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c9482-188">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c9482-189">Изображения эмблемы, отображаемые в приложениях портала компании на светлый фон.</span><span class="sxs-lookup"><span data-stu-id="c9482-189">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="c9482-190">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="c9482-190">landingPageCustomizedImage</span></span>|<span data-ttu-id="c9482-191">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="c9482-191">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="c9482-192">Настраиваемая изображение, отображаемое в приложениях портал "Компания" Главная страница</span><span class="sxs-lookup"><span data-stu-id="c9482-192">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="c9482-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9482-193">Response</span></span>
<span data-ttu-id="c9482-194">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c9482-194">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9482-195">Пример</span><span class="sxs-lookup"><span data-stu-id="c9482-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9482-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9482-196">Request</span></span>
<span data-ttu-id="c9482-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9482-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1269

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
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

### <a name="response"></a><span data-ttu-id="c9482-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9482-198">Response</span></span>
<span data-ttu-id="c9482-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c9482-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






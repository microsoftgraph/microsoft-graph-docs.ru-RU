---
title: Создание intuneBrandingProfile
description: Создание нового объекта intuneBrandingProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 755de596da82aa2ef7a8d5bc142f43e6bf2ca4c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964545"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="f0b32-103">Создание intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="f0b32-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="f0b32-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f0b32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0b32-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0b32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0b32-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f0b32-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0b32-107">Создание нового объекта [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f0b32-107">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0b32-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f0b32-108">Prerequisites</span></span>
<span data-ttu-id="f0b32-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0b32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0b32-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0b32-111">Permission type</span></span>|<span data-ttu-id="f0b32-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0b32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0b32-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0b32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0b32-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0b32-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f0b32-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0b32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0b32-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0b32-116">Not supported.</span></span>|
|<span data-ttu-id="f0b32-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0b32-117">Application</span></span>|<span data-ttu-id="f0b32-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0b32-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0b32-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0b32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f0b32-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0b32-120">Request headers</span></span>
|<span data-ttu-id="f0b32-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0b32-121">Header</span></span>|<span data-ttu-id="f0b32-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0b32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0b32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0b32-123">Authorization</span></span>|<span data-ttu-id="f0b32-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f0b32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0b32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0b32-125">Accept</span></span>|<span data-ttu-id="f0b32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0b32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0b32-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f0b32-127">Request body</span></span>
<span data-ttu-id="f0b32-128">В тексте запроса укажите представление JSON для объекта intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="f0b32-128">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="f0b32-129">В следующей таблице показаны свойства, которые необходимы для создания intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="f0b32-129">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="f0b32-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0b32-130">Property</span></span>|<span data-ttu-id="f0b32-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f0b32-131">Type</span></span>|<span data-ttu-id="f0b32-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f0b32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0b32-133">id</span><span class="sxs-lookup"><span data-stu-id="f0b32-133">id</span></span>|<span data-ttu-id="f0b32-134">String</span><span class="sxs-lookup"><span data-stu-id="f0b32-134">String</span></span>|<span data-ttu-id="f0b32-135">Клавиша профилей</span><span class="sxs-lookup"><span data-stu-id="f0b32-135">Profile Key</span></span>|
|<span data-ttu-id="f0b32-136">Имя_профиля</span><span class="sxs-lookup"><span data-stu-id="f0b32-136">profileName</span></span>|<span data-ttu-id="f0b32-137">String</span><span class="sxs-lookup"><span data-stu-id="f0b32-137">String</span></span>|<span data-ttu-id="f0b32-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="f0b32-138">Name of the profile</span></span>|
|<span data-ttu-id="f0b32-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="f0b32-139">profileDescription</span></span>|<span data-ttu-id="f0b32-140">String</span><span class="sxs-lookup"><span data-stu-id="f0b32-140">String</span></span>|<span data-ttu-id="f0b32-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="f0b32-141">Description of the profile</span></span>|
|<span data-ttu-id="f0b32-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="f0b32-142">isDefaultProfile</span></span>|<span data-ttu-id="f0b32-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0b32-143">Boolean</span></span>|<span data-ttu-id="f0b32-144">Представляет при использовании профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f0b32-144">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="f0b32-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0b32-145">createdDateTime</span></span>|<span data-ttu-id="f0b32-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0b32-146">DateTimeOffset</span></span>|<span data-ttu-id="f0b32-147">При создании BrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="f0b32-147">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="f0b32-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0b32-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f0b32-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0b32-149">DateTimeOffset</span></span>|<span data-ttu-id="f0b32-150">Время последнего изменения BrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="f0b32-150">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="f0b32-151">displayName</span><span class="sxs-lookup"><span data-stu-id="f0b32-151">displayName</span></span>|<span data-ttu-id="f0b32-152">String</span><span class="sxs-lookup"><span data-stu-id="f0b32-152">String</span></span>|<span data-ttu-id="f0b32-153">Название компании или организации, которое отображается пользователям.</span><span class="sxs-lookup"><span data-stu-id="f0b32-153">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="f0b32-154">contactITName</span><span class="sxs-lookup"><span data-stu-id="f0b32-154">contactITName</span></span>|<span data-ttu-id="f0b32-155">String</span><span class="sxs-lookup"><span data-stu-id="f0b32-155">String</span></span>|<span data-ttu-id="f0b32-156">Имя пользователя или название организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="f0b32-156">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="f0b32-157">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="f0b32-157">contactITPhoneNumber</span></span>|<span data-ttu-id="f0b32-158">String</span><span class="sxs-lookup"><span data-stu-id="f0b32-158">String</span></span>|<span data-ttu-id="f0b32-159">Номер телефона пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="f0b32-159">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="f0b32-160">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f0b32-160">contactITEmailAddress</span></span>|<span data-ttu-id="f0b32-161">String</span><span class="sxs-lookup"><span data-stu-id="f0b32-161">String</span></span>|<span data-ttu-id="f0b32-162">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="f0b32-162">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="f0b32-163">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="f0b32-163">contactITNotes</span></span>|<span data-ttu-id="f0b32-164">String</span><span class="sxs-lookup"><span data-stu-id="f0b32-164">String</span></span>|<span data-ttu-id="f0b32-165">Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="f0b32-165">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="f0b32-166">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="f0b32-166">privacyUrl</span></span>|<span data-ttu-id="f0b32-167">String</span><span class="sxs-lookup"><span data-stu-id="f0b32-167">String</span></span>|<span data-ttu-id="f0b32-168">URL-адрес страницы с политикой конфиденциальности компании или организации.</span><span class="sxs-lookup"><span data-stu-id="f0b32-168">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="f0b32-169">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="f0b32-169">onlineSupportSiteUrl</span></span>|<span data-ttu-id="f0b32-170">String</span><span class="sxs-lookup"><span data-stu-id="f0b32-170">String</span></span>|<span data-ttu-id="f0b32-171">URL-адрес сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="f0b32-171">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="f0b32-172">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="f0b32-172">onlineSupportSiteName</span></span>|<span data-ttu-id="f0b32-173">String</span><span class="sxs-lookup"><span data-stu-id="f0b32-173">String</span></span>|<span data-ttu-id="f0b32-174">Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="f0b32-174">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="f0b32-175">themeColor</span><span class="sxs-lookup"><span data-stu-id="f0b32-175">themeColor</span></span>|[<span data-ttu-id="f0b32-176">rgbColor</span><span class="sxs-lookup"><span data-stu-id="f0b32-176">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="f0b32-177">Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.</span><span class="sxs-lookup"><span data-stu-id="f0b32-177">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="f0b32-178">showLogo</span><span class="sxs-lookup"><span data-stu-id="f0b32-178">showLogo</span></span>|<span data-ttu-id="f0b32-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0b32-179">Boolean</span></span>|<span data-ttu-id="f0b32-180">Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.</span><span class="sxs-lookup"><span data-stu-id="f0b32-180">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="f0b32-181">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="f0b32-181">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="f0b32-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0b32-182">Boolean</span></span>|<span data-ttu-id="f0b32-183">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="f0b32-183">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="f0b32-184">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="f0b32-184">themeColorLogo</span></span>|<span data-ttu-id="f0b32-185">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="f0b32-185">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="f0b32-186">Изображения эмблемы, отображаемые в приложениях портала компании на темы цвет фона.</span><span class="sxs-lookup"><span data-stu-id="f0b32-186">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="f0b32-187">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="f0b32-187">lightBackgroundLogo</span></span>|[<span data-ttu-id="f0b32-188">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f0b32-188">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f0b32-189">Изображения эмблемы, отображаемые в приложениях портала компании на светлый фон.</span><span class="sxs-lookup"><span data-stu-id="f0b32-189">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="f0b32-190">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="f0b32-190">landingPageCustomizedImage</span></span>|<span data-ttu-id="f0b32-191">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="f0b32-191">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="f0b32-192">Настраиваемая изображение, отображаемое в приложениях портал "Компания" Главная страница</span><span class="sxs-lookup"><span data-stu-id="f0b32-192">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="f0b32-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0b32-193">Response</span></span>
<span data-ttu-id="f0b32-194">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f0b32-194">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0b32-195">Пример</span><span class="sxs-lookup"><span data-stu-id="f0b32-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0b32-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0b32-196">Request</span></span>
<span data-ttu-id="f0b32-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0b32-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f0b32-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0b32-198">Response</span></span>
<span data-ttu-id="f0b32-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f0b32-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






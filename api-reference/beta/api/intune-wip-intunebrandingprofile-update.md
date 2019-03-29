---
title: Обновление Интунебрандингпрофиле
description: Обновление свойств объекта Интунебрандингпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8a805e8878dbd41493c550647ed9e038c320b13
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976661"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="284ef-103">Обновление Интунебрандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="284ef-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="284ef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="284ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="284ef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="284ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="284ef-106">Обновление свойств объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="284ef-106">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="284ef-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="284ef-107">Prerequisites</span></span>
<span data-ttu-id="284ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="284ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="284ef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="284ef-110">Permission type</span></span>|<span data-ttu-id="284ef-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="284ef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="284ef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="284ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="284ef-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="284ef-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="284ef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="284ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="284ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="284ef-115">Not supported.</span></span>|
|<span data-ttu-id="284ef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="284ef-116">Application</span></span>|<span data-ttu-id="284ef-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="284ef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="284ef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="284ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="284ef-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="284ef-119">Request headers</span></span>
|<span data-ttu-id="284ef-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="284ef-120">Header</span></span>|<span data-ttu-id="284ef-121">Значение</span><span class="sxs-lookup"><span data-stu-id="284ef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="284ef-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="284ef-122">Authorization</span></span>|<span data-ttu-id="284ef-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="284ef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="284ef-124">Accept</span><span class="sxs-lookup"><span data-stu-id="284ef-124">Accept</span></span>|<span data-ttu-id="284ef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="284ef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="284ef-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="284ef-126">Request body</span></span>
<span data-ttu-id="284ef-127">В тексте запроса добавьте представление объекта [Интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="284ef-127">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="284ef-128">В следующей таблице приведены свойства, необходимые при создании [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="284ef-128">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="284ef-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="284ef-129">Property</span></span>|<span data-ttu-id="284ef-130">Тип</span><span class="sxs-lookup"><span data-stu-id="284ef-130">Type</span></span>|<span data-ttu-id="284ef-131">Описание</span><span class="sxs-lookup"><span data-stu-id="284ef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="284ef-132">id</span><span class="sxs-lookup"><span data-stu-id="284ef-132">id</span></span>|<span data-ttu-id="284ef-133">String</span><span class="sxs-lookup"><span data-stu-id="284ef-133">String</span></span>|<span data-ttu-id="284ef-134">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="284ef-134">Profile Key</span></span>|
|<span data-ttu-id="284ef-135">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="284ef-135">profileName</span></span>|<span data-ttu-id="284ef-136">String</span><span class="sxs-lookup"><span data-stu-id="284ef-136">String</span></span>|<span data-ttu-id="284ef-137">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="284ef-137">Name of the profile</span></span>|
|<span data-ttu-id="284ef-138">Профиледескриптион</span><span class="sxs-lookup"><span data-stu-id="284ef-138">profileDescription</span></span>|<span data-ttu-id="284ef-139">String</span><span class="sxs-lookup"><span data-stu-id="284ef-139">String</span></span>|<span data-ttu-id="284ef-140">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="284ef-140">Description of the profile</span></span>|
|<span data-ttu-id="284ef-141">Исдефаултпрофиле</span><span class="sxs-lookup"><span data-stu-id="284ef-141">isDefaultProfile</span></span>|<span data-ttu-id="284ef-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="284ef-142">Boolean</span></span>|<span data-ttu-id="284ef-143">Показывает, используется ли профиль по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="284ef-143">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="284ef-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="284ef-144">createdDateTime</span></span>|<span data-ttu-id="284ef-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="284ef-145">DateTimeOffset</span></span>|<span data-ttu-id="284ef-146">При создании Брандингпрофиле.</span><span class="sxs-lookup"><span data-stu-id="284ef-146">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="284ef-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="284ef-147">lastModifiedDateTime</span></span>|<span data-ttu-id="284ef-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="284ef-148">DateTimeOffset</span></span>|<span data-ttu-id="284ef-149">При последнем изменении Брандингпрофиле.</span><span class="sxs-lookup"><span data-stu-id="284ef-149">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="284ef-150">displayName</span><span class="sxs-lookup"><span data-stu-id="284ef-150">displayName</span></span>|<span data-ttu-id="284ef-151">Строка</span><span class="sxs-lookup"><span data-stu-id="284ef-151">String</span></span>|<span data-ttu-id="284ef-152">Название компании или организации, которое отображается пользователям.</span><span class="sxs-lookup"><span data-stu-id="284ef-152">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="284ef-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="284ef-153">contactITName</span></span>|<span data-ttu-id="284ef-154">String</span><span class="sxs-lookup"><span data-stu-id="284ef-154">String</span></span>|<span data-ttu-id="284ef-155">Имя пользователя или название организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="284ef-155">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="284ef-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="284ef-156">contactITPhoneNumber</span></span>|<span data-ttu-id="284ef-157">String</span><span class="sxs-lookup"><span data-stu-id="284ef-157">String</span></span>|<span data-ttu-id="284ef-158">Номер телефона пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="284ef-158">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="284ef-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="284ef-159">contactITEmailAddress</span></span>|<span data-ttu-id="284ef-160">String</span><span class="sxs-lookup"><span data-stu-id="284ef-160">String</span></span>|<span data-ttu-id="284ef-161">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="284ef-161">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="284ef-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="284ef-162">contactITNotes</span></span>|<span data-ttu-id="284ef-163">String</span><span class="sxs-lookup"><span data-stu-id="284ef-163">String</span></span>|<span data-ttu-id="284ef-164">Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="284ef-164">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="284ef-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="284ef-165">privacyUrl</span></span>|<span data-ttu-id="284ef-166">String</span><span class="sxs-lookup"><span data-stu-id="284ef-166">String</span></span>|<span data-ttu-id="284ef-167">URL-адрес страницы с политикой конфиденциальности компании или организации.</span><span class="sxs-lookup"><span data-stu-id="284ef-167">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="284ef-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="284ef-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="284ef-169">String</span><span class="sxs-lookup"><span data-stu-id="284ef-169">String</span></span>|<span data-ttu-id="284ef-170">URL-адрес сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="284ef-170">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="284ef-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="284ef-171">onlineSupportSiteName</span></span>|<span data-ttu-id="284ef-172">String</span><span class="sxs-lookup"><span data-stu-id="284ef-172">String</span></span>|<span data-ttu-id="284ef-173">Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="284ef-173">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="284ef-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="284ef-174">themeColor</span></span>|[<span data-ttu-id="284ef-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="284ef-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="284ef-176">Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.</span><span class="sxs-lookup"><span data-stu-id="284ef-176">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="284ef-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="284ef-177">showLogo</span></span>|<span data-ttu-id="284ef-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="284ef-178">Boolean</span></span>|<span data-ttu-id="284ef-179">Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.</span><span class="sxs-lookup"><span data-stu-id="284ef-179">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="284ef-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="284ef-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="284ef-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="284ef-181">Boolean</span></span>|<span data-ttu-id="284ef-182">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="284ef-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="284ef-183">Семеколорлого</span><span class="sxs-lookup"><span data-stu-id="284ef-183">themeColorLogo</span></span>|<span data-ttu-id="284ef-184">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="284ef-184">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="284ef-185">Изображение логотипа, отображаемое в приложениях корпоративного портала на фоновом фоне цвета темы.</span><span class="sxs-lookup"><span data-stu-id="284ef-185">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="284ef-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="284ef-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="284ef-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="284ef-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="284ef-188">Изображение логотипа, отображаемое в приложениях корпоративного портала на светлом фоне.</span><span class="sxs-lookup"><span data-stu-id="284ef-188">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="284ef-189">Ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="284ef-189">landingPageCustomizedImage</span></span>|<span data-ttu-id="284ef-190">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="284ef-190">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="284ef-191">Настраиваемое изображение, отображаемое на начальной странице "приложения корпоративного портала"</span><span class="sxs-lookup"><span data-stu-id="284ef-191">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="284ef-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="284ef-192">Response</span></span>
<span data-ttu-id="284ef-193">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="284ef-193">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="284ef-194">Пример</span><span class="sxs-lookup"><span data-stu-id="284ef-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="284ef-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="284ef-195">Request</span></span>
<span data-ttu-id="284ef-196">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="284ef-196">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1205

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
  }
}
```

### <a name="response"></a><span data-ttu-id="284ef-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="284ef-197">Response</span></span>
<span data-ttu-id="284ef-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="284ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





---
title: Тип ресурса intuneBrand
description: Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 478f087b4a7998a8c90bd429e0a0d3173d9b8e3c
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088037"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="69c80-103">Тип ресурса intuneBrand</span><span class="sxs-lookup"><span data-stu-id="69c80-103">intuneBrand resource type</span></span>

> <span data-ttu-id="69c80-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69c80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69c80-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69c80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69c80-106">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="69c80-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="69c80-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="69c80-107">Properties</span></span>
|<span data-ttu-id="69c80-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="69c80-108">Property</span></span>|<span data-ttu-id="69c80-109">Тип</span><span class="sxs-lookup"><span data-stu-id="69c80-109">Type</span></span>|<span data-ttu-id="69c80-110">Описание</span><span class="sxs-lookup"><span data-stu-id="69c80-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69c80-111">displayName</span><span class="sxs-lookup"><span data-stu-id="69c80-111">displayName</span></span>|<span data-ttu-id="69c80-112">String</span><span class="sxs-lookup"><span data-stu-id="69c80-112">String</span></span>|<span data-ttu-id="69c80-113">Название компании или организации, которое отображается пользователям.</span><span class="sxs-lookup"><span data-stu-id="69c80-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="69c80-114">themeColor</span><span class="sxs-lookup"><span data-stu-id="69c80-114">themeColor</span></span>|[<span data-ttu-id="69c80-115">rgbColor</span><span class="sxs-lookup"><span data-stu-id="69c80-115">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="69c80-116">Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.</span><span class="sxs-lookup"><span data-stu-id="69c80-116">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="69c80-117">showLogo</span><span class="sxs-lookup"><span data-stu-id="69c80-117">showLogo</span></span>|<span data-ttu-id="69c80-118">Логический</span><span class="sxs-lookup"><span data-stu-id="69c80-118">Boolean</span></span>|<span data-ttu-id="69c80-119">Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.</span><span class="sxs-lookup"><span data-stu-id="69c80-119">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="69c80-120">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="69c80-120">lightBackgroundLogo</span></span>|<span data-ttu-id="69c80-121">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="69c80-121">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="69c80-122">Изображение с логотипом на светлом фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="69c80-122">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="69c80-123">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="69c80-123">darkBackgroundLogo</span></span>|[<span data-ttu-id="69c80-124">mimeContent</span><span class="sxs-lookup"><span data-stu-id="69c80-124">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="69c80-125">Изображение с логотипом на темном фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="69c80-125">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="69c80-126">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="69c80-126">showNameNextToLogo</span></span>|<span data-ttu-id="69c80-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="69c80-127">Boolean</span></span>|<span data-ttu-id="69c80-128">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="69c80-128">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="69c80-129">ландингпажекустомизедимаже</span><span class="sxs-lookup"><span data-stu-id="69c80-129">landingPageCustomizedImage</span></span>|<span data-ttu-id="69c80-130">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="69c80-130">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="69c80-131">Настраиваемое изображение, отображаемое на начальной странице приложения корпоративного портала</span><span class="sxs-lookup"><span data-stu-id="69c80-131">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="69c80-132">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="69c80-132">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="69c80-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="69c80-133">Boolean</span></span>|<span data-ttu-id="69c80-134">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="69c80-134">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="69c80-135">contactITName</span><span class="sxs-lookup"><span data-stu-id="69c80-135">contactITName</span></span>|<span data-ttu-id="69c80-136">String</span><span class="sxs-lookup"><span data-stu-id="69c80-136">String</span></span>|<span data-ttu-id="69c80-137">Имя пользователя или название организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="69c80-137">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="69c80-138">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="69c80-138">contactITPhoneNumber</span></span>|<span data-ttu-id="69c80-139">String</span><span class="sxs-lookup"><span data-stu-id="69c80-139">String</span></span>|<span data-ttu-id="69c80-140">Номер телефона пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="69c80-140">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="69c80-141">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="69c80-141">contactITEmailAddress</span></span>|<span data-ttu-id="69c80-142">String</span><span class="sxs-lookup"><span data-stu-id="69c80-142">String</span></span>|<span data-ttu-id="69c80-143">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="69c80-143">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="69c80-144">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="69c80-144">contactITNotes</span></span>|<span data-ttu-id="69c80-145">String</span><span class="sxs-lookup"><span data-stu-id="69c80-145">String</span></span>|<span data-ttu-id="69c80-146">Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="69c80-146">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="69c80-147">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="69c80-147">onlineSupportSiteUrl</span></span>|<span data-ttu-id="69c80-148">String</span><span class="sxs-lookup"><span data-stu-id="69c80-148">String</span></span>|<span data-ttu-id="69c80-149">URL-адрес сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="69c80-149">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="69c80-150">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="69c80-150">onlineSupportSiteName</span></span>|<span data-ttu-id="69c80-151">String</span><span class="sxs-lookup"><span data-stu-id="69c80-151">String</span></span>|<span data-ttu-id="69c80-152">Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="69c80-152">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="69c80-153">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="69c80-153">privacyUrl</span></span>|<span data-ttu-id="69c80-154">String</span><span class="sxs-lookup"><span data-stu-id="69c80-154">String</span></span>|<span data-ttu-id="69c80-155">URL-адрес страницы с политикой конфиденциальности компании или организации.</span><span class="sxs-lookup"><span data-stu-id="69c80-155">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="69c80-156">кустомпривацимессаже</span><span class="sxs-lookup"><span data-stu-id="69c80-156">customPrivacyMessage</span></span>|<span data-ttu-id="69c80-157">String</span><span class="sxs-lookup"><span data-stu-id="69c80-157">String</span></span>|<span data-ttu-id="69c80-158">Пользовательское сообщение о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="69c80-158">Custom privacy message.</span></span>|
|<span data-ttu-id="69c80-159">исремоведевицедисаблед</span><span class="sxs-lookup"><span data-stu-id="69c80-159">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="69c80-160">Логический</span><span class="sxs-lookup"><span data-stu-id="69c80-160">Boolean</span></span>|<span data-ttu-id="69c80-161">Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="69c80-161">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="69c80-162">исфакториресетдисаблед</span><span class="sxs-lookup"><span data-stu-id="69c80-162">isFactoryResetDisabled</span></span>|<span data-ttu-id="69c80-163">Логический</span><span class="sxs-lookup"><span data-stu-id="69c80-163">Boolean</span></span>|<span data-ttu-id="69c80-164">Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="69c80-164">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="69c80-165">компанипорталблоккедактионс</span><span class="sxs-lookup"><span data-stu-id="69c80-165">companyPortalBlockedActions</span></span>|<span data-ttu-id="69c80-166">Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="69c80-166">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="69c80-167">Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.</span><span class="sxs-lookup"><span data-stu-id="69c80-167">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="69c80-168">шовазуреадентерприсеаппс</span><span class="sxs-lookup"><span data-stu-id="69c80-168">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="69c80-169">Логический</span><span class="sxs-lookup"><span data-stu-id="69c80-169">Boolean</span></span>|<span data-ttu-id="69c80-170">Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.</span><span class="sxs-lookup"><span data-stu-id="69c80-170">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="69c80-171">шовоффицевебаппс</span><span class="sxs-lookup"><span data-stu-id="69c80-171">showOfficeWebApps</span></span>|<span data-ttu-id="69c80-172">Логический</span><span class="sxs-lookup"><span data-stu-id="69c80-172">Boolean</span></span>|<span data-ttu-id="69c80-173">Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.</span><span class="sxs-lookup"><span data-stu-id="69c80-173">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|

## <a name="relationships"></a><span data-ttu-id="69c80-174">Связи</span><span class="sxs-lookup"><span data-stu-id="69c80-174">Relationships</span></span>
<span data-ttu-id="69c80-175">Нет</span><span class="sxs-lookup"><span data-stu-id="69c80-175">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69c80-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69c80-176">JSON Representation</span></span>
<span data-ttu-id="69c80-177">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69c80-177">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showDisplayNameNextToLogo": true,
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String",
  "customPrivacyMessage": "String",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "String",
      "ownerType": "String",
      "action": "String"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true
}
```




---
title: Тип ресурса intuneBrand
description: Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ab8465390b6b0a9e4f35e8a713f082dfb9325eb3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957685"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="eef5c-103">Тип ресурса intuneBrand</span><span class="sxs-lookup"><span data-stu-id="eef5c-103">intuneBrand resource type</span></span>

> <span data-ttu-id="eef5c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eef5c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eef5c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eef5c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eef5c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eef5c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eef5c-107">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="eef5c-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>
## <a name="properties"></a><span data-ttu-id="eef5c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eef5c-108">Properties</span></span>
|<span data-ttu-id="eef5c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eef5c-109">Property</span></span>|<span data-ttu-id="eef5c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eef5c-110">Type</span></span>|<span data-ttu-id="eef5c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eef5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eef5c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="eef5c-112">displayName</span></span>|<span data-ttu-id="eef5c-113">String</span><span class="sxs-lookup"><span data-stu-id="eef5c-113">String</span></span>|<span data-ttu-id="eef5c-114">Название компании или организации, которое отображается пользователям.</span><span class="sxs-lookup"><span data-stu-id="eef5c-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="eef5c-115">contactITName</span><span class="sxs-lookup"><span data-stu-id="eef5c-115">contactITName</span></span>|<span data-ttu-id="eef5c-116">String</span><span class="sxs-lookup"><span data-stu-id="eef5c-116">String</span></span>|<span data-ttu-id="eef5c-117">Имя пользователя или название организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="eef5c-117">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="eef5c-118">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="eef5c-118">contactITPhoneNumber</span></span>|<span data-ttu-id="eef5c-119">String</span><span class="sxs-lookup"><span data-stu-id="eef5c-119">String</span></span>|<span data-ttu-id="eef5c-120">Номер телефона пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="eef5c-120">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="eef5c-121">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="eef5c-121">contactITEmailAddress</span></span>|<span data-ttu-id="eef5c-122">String</span><span class="sxs-lookup"><span data-stu-id="eef5c-122">String</span></span>|<span data-ttu-id="eef5c-123">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="eef5c-123">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="eef5c-124">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="eef5c-124">contactITNotes</span></span>|<span data-ttu-id="eef5c-125">String</span><span class="sxs-lookup"><span data-stu-id="eef5c-125">String</span></span>|<span data-ttu-id="eef5c-126">Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="eef5c-126">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="eef5c-127">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="eef5c-127">privacyUrl</span></span>|<span data-ttu-id="eef5c-128">String</span><span class="sxs-lookup"><span data-stu-id="eef5c-128">String</span></span>|<span data-ttu-id="eef5c-129">URL-адрес страницы с политикой конфиденциальности компании или организации.</span><span class="sxs-lookup"><span data-stu-id="eef5c-129">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="eef5c-130">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="eef5c-130">onlineSupportSiteUrl</span></span>|<span data-ttu-id="eef5c-131">String</span><span class="sxs-lookup"><span data-stu-id="eef5c-131">String</span></span>|<span data-ttu-id="eef5c-132">URL-адрес сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="eef5c-132">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="eef5c-133">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="eef5c-133">onlineSupportSiteName</span></span>|<span data-ttu-id="eef5c-134">String</span><span class="sxs-lookup"><span data-stu-id="eef5c-134">String</span></span>|<span data-ttu-id="eef5c-135">Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="eef5c-135">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="eef5c-136">themeColor</span><span class="sxs-lookup"><span data-stu-id="eef5c-136">themeColor</span></span>|[<span data-ttu-id="eef5c-137">rgbColor</span><span class="sxs-lookup"><span data-stu-id="eef5c-137">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="eef5c-138">Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.</span><span class="sxs-lookup"><span data-stu-id="eef5c-138">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="eef5c-139">showLogo</span><span class="sxs-lookup"><span data-stu-id="eef5c-139">showLogo</span></span>|<span data-ttu-id="eef5c-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="eef5c-140">Boolean</span></span>|<span data-ttu-id="eef5c-141">Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.</span><span class="sxs-lookup"><span data-stu-id="eef5c-141">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="eef5c-142">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="eef5c-142">lightBackgroundLogo</span></span>|[<span data-ttu-id="eef5c-143">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eef5c-143">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eef5c-144">Изображение с логотипом на светлом фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="eef5c-144">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="eef5c-145">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="eef5c-145">darkBackgroundLogo</span></span>|[<span data-ttu-id="eef5c-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eef5c-146">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eef5c-147">Изображение с логотипом на темном фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="eef5c-147">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="eef5c-148">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="eef5c-148">showNameNextToLogo</span></span>|<span data-ttu-id="eef5c-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="eef5c-149">Boolean</span></span>|<span data-ttu-id="eef5c-150">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="eef5c-150">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="eef5c-151">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="eef5c-151">landingPageCustomizedImage</span></span>|<span data-ttu-id="eef5c-152">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="eef5c-152">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="eef5c-153">Настраиваемая изображение, отображаемое на странице приложения портала компании</span><span class="sxs-lookup"><span data-stu-id="eef5c-153">Customized image displayed in Compnay Portal app landing page</span></span>|
|<span data-ttu-id="eef5c-154">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="eef5c-154">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="eef5c-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="eef5c-155">Boolean</span></span>|<span data-ttu-id="eef5c-156">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="eef5c-156">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eef5c-157">Связи</span><span class="sxs-lookup"><span data-stu-id="eef5c-157">Relationships</span></span>
<span data-ttu-id="eef5c-158">Нет</span><span class="sxs-lookup"><span data-stu-id="eef5c-158">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eef5c-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eef5c-159">JSON Representation</span></span>
<span data-ttu-id="eef5c-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eef5c-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
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
  "showDisplayNameNextToLogo": true
}
```






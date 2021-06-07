---
title: Тип ресурса intuneBrand
description: Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 346966fdcb3cfc8b3c4c24e55f4a07e46c97a612
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751274"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="54a82-103">Тип ресурса intuneBrand</span><span class="sxs-lookup"><span data-stu-id="54a82-103">intuneBrand resource type</span></span>

<span data-ttu-id="54a82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54a82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54a82-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54a82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54a82-106">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="54a82-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="54a82-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="54a82-107">Properties</span></span>
|<span data-ttu-id="54a82-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="54a82-108">Property</span></span>|<span data-ttu-id="54a82-109">Тип</span><span class="sxs-lookup"><span data-stu-id="54a82-109">Type</span></span>|<span data-ttu-id="54a82-110">Описание</span><span class="sxs-lookup"><span data-stu-id="54a82-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54a82-111">displayName</span><span class="sxs-lookup"><span data-stu-id="54a82-111">displayName</span></span>|<span data-ttu-id="54a82-112">String</span><span class="sxs-lookup"><span data-stu-id="54a82-112">String</span></span>|<span data-ttu-id="54a82-113">Название компании или организации, которое отображается пользователям.</span><span class="sxs-lookup"><span data-stu-id="54a82-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="54a82-114">themeColor</span><span class="sxs-lookup"><span data-stu-id="54a82-114">themeColor</span></span>|[<span data-ttu-id="54a82-115">rgbColor</span><span class="sxs-lookup"><span data-stu-id="54a82-115">rgbColor</span></span>](../resources/intune-onboarding-rgbcolor.md)|<span data-ttu-id="54a82-116">Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.</span><span class="sxs-lookup"><span data-stu-id="54a82-116">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="54a82-117">showLogo</span><span class="sxs-lookup"><span data-stu-id="54a82-117">showLogo</span></span>|<span data-ttu-id="54a82-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="54a82-118">Boolean</span></span>|<span data-ttu-id="54a82-119">Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.</span><span class="sxs-lookup"><span data-stu-id="54a82-119">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="54a82-120">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="54a82-120">lightBackgroundLogo</span></span>|[<span data-ttu-id="54a82-121">mimeContent</span><span class="sxs-lookup"><span data-stu-id="54a82-121">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="54a82-122">Изображение с логотипом на светлом фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="54a82-122">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="54a82-123">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="54a82-123">darkBackgroundLogo</span></span>|[<span data-ttu-id="54a82-124">mimeContent</span><span class="sxs-lookup"><span data-stu-id="54a82-124">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="54a82-125">Изображение с логотипом на темном фоне, которое отображается в приложениях "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="54a82-125">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="54a82-126">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="54a82-126">showNameNextToLogo</span></span>|<span data-ttu-id="54a82-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="54a82-127">Boolean</span></span>|<span data-ttu-id="54a82-128">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="54a82-128">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="54a82-129">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="54a82-129">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="54a82-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="54a82-130">Boolean</span></span>|<span data-ttu-id="54a82-131">Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="54a82-131">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="54a82-132">contactITName</span><span class="sxs-lookup"><span data-stu-id="54a82-132">contactITName</span></span>|<span data-ttu-id="54a82-133">String</span><span class="sxs-lookup"><span data-stu-id="54a82-133">String</span></span>|<span data-ttu-id="54a82-134">Имя пользователя или название организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="54a82-134">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="54a82-135">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="54a82-135">contactITPhoneNumber</span></span>|<span data-ttu-id="54a82-136">String</span><span class="sxs-lookup"><span data-stu-id="54a82-136">String</span></span>|<span data-ttu-id="54a82-137">Номер телефона пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="54a82-137">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="54a82-138">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="54a82-138">contactITEmailAddress</span></span>|<span data-ttu-id="54a82-139">String</span><span class="sxs-lookup"><span data-stu-id="54a82-139">String</span></span>|<span data-ttu-id="54a82-140">Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="54a82-140">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="54a82-141">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="54a82-141">contactITNotes</span></span>|<span data-ttu-id="54a82-142">String</span><span class="sxs-lookup"><span data-stu-id="54a82-142">String</span></span>|<span data-ttu-id="54a82-143">Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.</span><span class="sxs-lookup"><span data-stu-id="54a82-143">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="54a82-144">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="54a82-144">onlineSupportSiteUrl</span></span>|<span data-ttu-id="54a82-145">String</span><span class="sxs-lookup"><span data-stu-id="54a82-145">String</span></span>|<span data-ttu-id="54a82-146">URL-адрес сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="54a82-146">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="54a82-147">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="54a82-147">onlineSupportSiteName</span></span>|<span data-ttu-id="54a82-148">String</span><span class="sxs-lookup"><span data-stu-id="54a82-148">String</span></span>|<span data-ttu-id="54a82-149">Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.</span><span class="sxs-lookup"><span data-stu-id="54a82-149">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="54a82-150">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="54a82-150">privacyUrl</span></span>|<span data-ttu-id="54a82-151">String</span><span class="sxs-lookup"><span data-stu-id="54a82-151">String</span></span>|<span data-ttu-id="54a82-152">URL-адрес страницы с политикой конфиденциальности компании или организации.</span><span class="sxs-lookup"><span data-stu-id="54a82-152">URL to the company/organization’s privacy policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54a82-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="54a82-153">Relationships</span></span>
<span data-ttu-id="54a82-154">Нет</span><span class="sxs-lookup"><span data-stu-id="54a82-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54a82-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54a82-155">JSON Representation</span></span>
<span data-ttu-id="54a82-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54a82-156">Here is a JSON representation of the resource.</span></span>
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
  "showDisplayNameNextToLogo": true,
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String"
}
```





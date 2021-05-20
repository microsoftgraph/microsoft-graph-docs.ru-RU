---
title: тип ресурса userFlowLanguageConfiguration
description: Объект userFlowsLanguageConfiguration позволяет потоку пользователей поддерживать настройку нескольких языков.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: aa83d85725cbef54229cdc92246fb83888697166
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547150"
---
# <a name="userflowlanguageconfiguration-resource-type"></a><span data-ttu-id="ddbf5-103">тип ресурса userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="ddbf5-103">userFlowLanguageConfiguration resource type</span></span>

<span data-ttu-id="ddbf5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddbf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddbf5-105">Настройка языка потоков пользователей — это функция, которая позволяет заданный поток пользователей поддерживать настройку нескольких языков, от всех встроенных языков до настраиваемого языка.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-105">User flows language customization is a feature that allows a given user flow to support customization of multiple languages, from all the built-in languages to a custom language.</span></span>

<span data-ttu-id="ddbf5-106">Для Azure Active Directory потоки пользователей [B2C](/azure/active-directory-b2c/user-flow-language-customization#supported-languages)можно использовать встроенные языки или предоставить языковые настройки для языка, который в настоящее время не встроен по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-106">For [Azure Active Directory B2C user flows](/azure/active-directory-b2c/user-flow-language-customization#supported-languages), you can leverage the built-in languages or provide the language customizations for a language that is not currently built-in by default.</span></span> <span data-ttu-id="ddbf5-107">Для [Azure Active Directory](/azure/active-directory/external-identities/user-flow-customize-language)потоков пользователей можно использовать только встроенные языки, предоставляемые Корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-107">For [Azure Active Directory user flows](/azure/active-directory/external-identities/user-flow-customize-language), you can only leverage the built-in languages provided by Microsoft.</span></span> <span data-ttu-id="ddbf5-108">Потоки пользователей Azure Active Directory B2C и Azure Active Directory поддерживают настройку языка и строк, показанных пользователям во время поездок, настроенных с потоками пользователей.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-108">Both user flows for Azure Active Directory B2C and Azure Active Directory support customizing the language and strings shown to users as they go through the journeys you configure with your user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="ddbf5-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ddbf5-109">Methods</span></span>

|<span data-ttu-id="ddbf5-110">Метод</span><span class="sxs-lookup"><span data-stu-id="ddbf5-110">Method</span></span>|<span data-ttu-id="ddbf5-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="ddbf5-111">Return type</span></span>|<span data-ttu-id="ddbf5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ddbf5-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ddbf5-113">Get userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="ddbf5-113">Get userFlowLanguageConfiguration</span></span>](../api/userflowlanguageconfiguration-get.md)|[<span data-ttu-id="ddbf5-114">userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="ddbf5-114">userFlowLanguageConfiguration</span></span>](../resources/userflowlanguageconfiguration.md)|<span data-ttu-id="ddbf5-115">Ознакомьтесь с свойствами и отношениями [объекта userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddbf5-115">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="ddbf5-116">Эти объекты представляют язык, доступный в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-116">These objects represent a language available in a user flow.</span></span>|
|[<span data-ttu-id="ddbf5-117">Удаление userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="ddbf5-117">Delete userFlowLanguageConfiguration</span></span>](../api/userflowlanguageconfiguration-delete.md)|<span data-ttu-id="ddbf5-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ddbf5-118">None</span></span>|<span data-ttu-id="ddbf5-119">Удаляет настраиваемый [объект userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddbf5-119">Deletes a custom [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="ddbf5-120">Эти объекты представляют язык, доступный в потоке пользователей, и из потока пользователей Azure AD B2C можно удалить только настраиваемый язык.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-120">These objects represent a language available in a user flow and only a custom language can be deleted from an Azure AD B2C user flow.</span></span>|
|[<span data-ttu-id="ddbf5-121">Список defaultPages</span><span class="sxs-lookup"><span data-stu-id="ddbf5-121">List defaultPages</span></span>](../api/userflowlanguageconfiguration-list-defaultpages.md)|<span data-ttu-id="ddbf5-122">[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="ddbf5-122">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="ddbf5-123">Получите ресурсы userFlowLanguagePage из свойства навигации defaultPages.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-123">Get the userFlowLanguagePage resources from the defaultPages navigation property.</span></span> <span data-ttu-id="ddbf5-124">Представляет путь пользователя по умолчанию в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-124">Represents the default user journey in a user flow.</span></span>|
|[<span data-ttu-id="ddbf5-125">Переопределения списка</span><span class="sxs-lookup"><span data-stu-id="ddbf5-125">List overridesPages</span></span>](../api/userflowlanguageconfiguration-list-overridespages.md)|<span data-ttu-id="ddbf5-126">[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="ddbf5-126">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="ddbf5-127">Получите ресурсы userFlowLanguagePage из свойства навигации overridesPages.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-127">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="ddbf5-128">Представляет настраиваемый интерфейс для пользовательского путешествия в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-128">Represents a custom experience for a user journey in a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="ddbf5-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="ddbf5-129">Properties</span></span>

|<span data-ttu-id="ddbf5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddbf5-130">Property</span></span>|<span data-ttu-id="ddbf5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ddbf5-131">Type</span></span>|<span data-ttu-id="ddbf5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ddbf5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddbf5-133">id</span><span class="sxs-lookup"><span data-stu-id="ddbf5-133">id</span></span>|<span data-ttu-id="ddbf5-134">String</span><span class="sxs-lookup"><span data-stu-id="ddbf5-134">String</span></span>|<span data-ttu-id="ddbf5-135">Идентификатор языка.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-135">The identifier of the language.</span></span> <span data-ttu-id="ddbf5-136">Это поле — тег языкового [ID RFC 5646,](https://tools.ietf.org/html/rfc5646) который должен быть документированным языковым ИД.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-136">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span>|
|<span data-ttu-id="ddbf5-137">isEnabled</span><span class="sxs-lookup"><span data-stu-id="ddbf5-137">isEnabled</span></span>|<span data-ttu-id="ddbf5-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddbf5-138">Boolean</span></span>|<span data-ttu-id="ddbf5-139">Указывает, включен ли язык в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-139">Indicates whether the language is enabled within the user flow.</span></span>|
|<span data-ttu-id="ddbf5-140">displayName</span><span class="sxs-lookup"><span data-stu-id="ddbf5-140">displayName</span></span>|<span data-ttu-id="ddbf5-141">String</span><span class="sxs-lookup"><span data-stu-id="ddbf5-141">String</span></span>|<span data-ttu-id="ddbf5-142">Отображаемая языковая фамилия.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-142">The language name to display.</span></span> <span data-ttu-id="ddbf5-143">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-143">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddbf5-144">Связи</span><span class="sxs-lookup"><span data-stu-id="ddbf5-144">Relationships</span></span>

|<span data-ttu-id="ddbf5-145">Связь</span><span class="sxs-lookup"><span data-stu-id="ddbf5-145">Relationship</span></span>|<span data-ttu-id="ddbf5-146">Тип</span><span class="sxs-lookup"><span data-stu-id="ddbf5-146">Type</span></span>|<span data-ttu-id="ddbf5-147">Описание</span><span class="sxs-lookup"><span data-stu-id="ddbf5-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddbf5-148">defaultPages</span><span class="sxs-lookup"><span data-stu-id="ddbf5-148">defaultPages</span></span>|<span data-ttu-id="ddbf5-149">[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="ddbf5-149">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="ddbf5-150">Коллекция страниц с контентом по умолчанию, отображаемым в потоке пользователей для указанного языка.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-150">Collection of pages with the default content to display in a user flow for a specified language.</span></span> <span data-ttu-id="ddbf5-151">Эта коллекция не позволяет вносить какие-либо изменения.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-151">This collection does not allow any kind of modification.</span></span>|
|<span data-ttu-id="ddbf5-152">overridesPages</span><span class="sxs-lookup"><span data-stu-id="ddbf5-152">overridesPages</span></span>|<span data-ttu-id="ddbf5-153">[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="ddbf5-153">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="ddbf5-154">Коллекция страниц с переопределениями сообщений для отображения в потоке пользователей для указанного языка.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-154">Collection of pages with the overrides messages to display in a user flow for a specified language.</span></span> <span data-ttu-id="ddbf5-155">Эта коллекция позволяет изменять только содержимое страницы, любые другие изменения не допускаются (создание или удаление страниц).</span><span class="sxs-lookup"><span data-stu-id="ddbf5-155">This collection only allows to modify the content of the page, any other modification is not allowed (creation or deletion of pages).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ddbf5-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ddbf5-156">JSON representation</span></span>

<span data-ttu-id="ddbf5-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddbf5-157">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguageConfiguration",
  "id": "String (identifier)",
  "isEnabled": "Boolean",
  "displayName": "String"
}
```

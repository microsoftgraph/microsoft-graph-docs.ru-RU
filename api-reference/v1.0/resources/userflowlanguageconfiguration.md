---
title: тип ресурса userFlowLanguageConfiguration
description: Позволяет потоку пользователей поддерживать несколько языков.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 556860eb77c4707f1d180b7924ae3126958a4799
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547206"
---
# <a name="userflowlanguageconfiguration-resource-type"></a><span data-ttu-id="f9efc-103">тип ресурса userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9efc-103">userFlowLanguageConfiguration resource type</span></span>

<span data-ttu-id="f9efc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9efc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9efc-105">Позволяет потоку пользователей поддерживать использование нескольких языков.</span><span class="sxs-lookup"><span data-stu-id="f9efc-105">Allows a user flow to support the use of multiple languages.</span></span>

<span data-ttu-id="f9efc-106">Для [Azure Active Directory](/azure/active-directory/external-identities/user-flow-customize-language)потоков пользователей можно использовать только встроенные языки, предоставляемые Корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="f9efc-106">For [Azure Active Directory user flows](/azure/active-directory/external-identities/user-flow-customize-language), you can only leverage the built-in languages provided by Microsoft.</span></span> <span data-ttu-id="f9efc-107">Потоки пользователей Azure Active Directory, определяющие язык и строки, показанные пользователям во время поездок, которые вы настраивали с помощью пользовательских потоков.</span><span class="sxs-lookup"><span data-stu-id="f9efc-107">User flows for Azure Active Directory support defining the language and strings shown to users as they go through the journeys you configure with your user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="f9efc-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f9efc-108">Methods</span></span>

|<span data-ttu-id="f9efc-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f9efc-109">Method</span></span>|<span data-ttu-id="f9efc-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="f9efc-110">Return type</span></span>|<span data-ttu-id="f9efc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f9efc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f9efc-112">Get userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9efc-112">Get userFlowLanguageConfiguration</span></span>](../api/userflowlanguageconfiguration-get.md)|[<span data-ttu-id="f9efc-113">userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9efc-113">userFlowLanguageConfiguration</span></span>](../resources/userflowlanguageconfiguration.md)|<span data-ttu-id="f9efc-114">Ознакомьтесь с свойствами и отношениями [объекта userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9efc-114">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="f9efc-115">Эти объекты представляют язык, доступный в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="f9efc-115">These objects represent a language available in a user flow.</span></span>|
|[<span data-ttu-id="f9efc-116">Список defaultPages</span><span class="sxs-lookup"><span data-stu-id="f9efc-116">List defaultPages</span></span>](../api/userflowlanguageconfiguration-list-defaultpages.md)|<span data-ttu-id="f9efc-117">[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="f9efc-117">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="f9efc-118">Получите ресурсы userFlowLanguagePage из свойства навигации defaultPages.</span><span class="sxs-lookup"><span data-stu-id="f9efc-118">Get the userFlowLanguagePage resources from the defaultPages navigation property.</span></span> <span data-ttu-id="f9efc-119">Представляет путь пользователя по умолчанию в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="f9efc-119">Represents the default user journey in a user flow.</span></span>|
|[<span data-ttu-id="f9efc-120">Переопределения списка</span><span class="sxs-lookup"><span data-stu-id="f9efc-120">List overridesPages</span></span>](../api/userflowlanguageconfiguration-list-overridespages.md)|<span data-ttu-id="f9efc-121">[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="f9efc-121">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="f9efc-122">Получите ресурсы userFlowLanguagePage из свойства навигации overridesPages.</span><span class="sxs-lookup"><span data-stu-id="f9efc-122">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="f9efc-123">Представляет настраиваемый интерфейс для пользовательского путешествия в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="f9efc-123">Represents a custom experience for a user journey in a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="f9efc-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9efc-124">Properties</span></span>

|<span data-ttu-id="f9efc-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9efc-125">Property</span></span>|<span data-ttu-id="f9efc-126">Тип</span><span class="sxs-lookup"><span data-stu-id="f9efc-126">Type</span></span>|<span data-ttu-id="f9efc-127">Описание</span><span class="sxs-lookup"><span data-stu-id="f9efc-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9efc-128">id</span><span class="sxs-lookup"><span data-stu-id="f9efc-128">id</span></span>|<span data-ttu-id="f9efc-129">Строка</span><span class="sxs-lookup"><span data-stu-id="f9efc-129">String</span></span>|<span data-ttu-id="f9efc-130">Идентификатор языка.</span><span class="sxs-lookup"><span data-stu-id="f9efc-130">The identifier of the language.</span></span> <span data-ttu-id="f9efc-131">Это поле — тег языкового [ID RFC 5646,](https://tools.ietf.org/html/rfc5646) который должен быть документированным языковым ИД.</span><span class="sxs-lookup"><span data-stu-id="f9efc-131">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span>|
|<span data-ttu-id="f9efc-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f9efc-132">isEnabled</span></span>|<span data-ttu-id="f9efc-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9efc-133">Boolean</span></span>|<span data-ttu-id="f9efc-134">Указывает, включен ли язык в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="f9efc-134">Indicates whether the language is enabled within the user flow.</span></span>|
|<span data-ttu-id="f9efc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f9efc-135">displayName</span></span>|<span data-ttu-id="f9efc-136">Строка</span><span class="sxs-lookup"><span data-stu-id="f9efc-136">String</span></span>|<span data-ttu-id="f9efc-137">Отображаемая языковая фамилия.</span><span class="sxs-lookup"><span data-stu-id="f9efc-137">The language name to display.</span></span> <span data-ttu-id="f9efc-138">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9efc-138">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9efc-139">Связи</span><span class="sxs-lookup"><span data-stu-id="f9efc-139">Relationships</span></span>

|<span data-ttu-id="f9efc-140">Связь</span><span class="sxs-lookup"><span data-stu-id="f9efc-140">Relationship</span></span>|<span data-ttu-id="f9efc-141">Тип</span><span class="sxs-lookup"><span data-stu-id="f9efc-141">Type</span></span>|<span data-ttu-id="f9efc-142">Описание</span><span class="sxs-lookup"><span data-stu-id="f9efc-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9efc-143">defaultPages</span><span class="sxs-lookup"><span data-stu-id="f9efc-143">defaultPages</span></span>|<span data-ttu-id="f9efc-144">[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="f9efc-144">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="f9efc-145">Коллекция страниц с контентом по умолчанию, отображаемым в потоке пользователей для указанного языка.</span><span class="sxs-lookup"><span data-stu-id="f9efc-145">Collection of pages with the default content to display in a user flow for a specified language.</span></span> <span data-ttu-id="f9efc-146">Эта коллекция не позволяет вносить какие-либо изменения.</span><span class="sxs-lookup"><span data-stu-id="f9efc-146">This collection does not allow any kind of modification.</span></span>|
|<span data-ttu-id="f9efc-147">overridesPages</span><span class="sxs-lookup"><span data-stu-id="f9efc-147">overridesPages</span></span>|<span data-ttu-id="f9efc-148">[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="f9efc-148">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="f9efc-149">Коллекция страниц с переопределениями сообщений для отображения в потоке пользователей для указанного языка.</span><span class="sxs-lookup"><span data-stu-id="f9efc-149">Collection of pages with the overrides messages to display in a user flow for a specified language.</span></span> <span data-ttu-id="f9efc-150">Эта коллекция позволяет изменять только содержимое страницы, любые другие изменения не допускаются (создание или удаление страниц).</span><span class="sxs-lookup"><span data-stu-id="f9efc-150">This collection only allows to modify the content of the page, any other modification is not allowed (creation or deletion of pages).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9efc-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9efc-151">JSON representation</span></span>

<span data-ttu-id="f9efc-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9efc-152">The following is a JSON representation of the resource.</span></span>
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

---
title: тип ресурса userFlowLanguageConfiguration
description: Позволяет потоку пользователей поддерживать несколько языков.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a3291309537ea914587e0491f9340bb626e88a68
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883310"
---
# <a name="userflowlanguageconfiguration-resource-type"></a><span data-ttu-id="6347a-103">тип ресурса userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="6347a-103">userFlowLanguageConfiguration resource type</span></span>

<span data-ttu-id="6347a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6347a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6347a-105">Позволяет потоку пользователей поддерживать использование нескольких языков.</span><span class="sxs-lookup"><span data-stu-id="6347a-105">Allows a user flow to support the use of multiple languages.</span></span>

<span data-ttu-id="6347a-106">Для [потоков пользователей Azure Active Directory](https://docs.microsoft.com/azure/active-directory/external-identities/user-flow-customize-language)можно использовать только встроенные языки, предоставляемые Корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6347a-106">For [Azure Active Directory user flows](https://docs.microsoft.com/azure/active-directory/external-identities/user-flow-customize-language), you can only leverage the built-in languages provided by Microsoft.</span></span> <span data-ttu-id="6347a-107">Потоки пользователей для поддержки Azure Active Directory, определяющие язык и строки, показанные пользователям во время поездок, настроенных с потоками пользователей.</span><span class="sxs-lookup"><span data-stu-id="6347a-107">User flows for Azure Active Directory support defining the language and strings shown to users as they go through the journeys you configure with your user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="6347a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6347a-108">Methods</span></span>

|<span data-ttu-id="6347a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6347a-109">Method</span></span>|<span data-ttu-id="6347a-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="6347a-110">Return type</span></span>|<span data-ttu-id="6347a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6347a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6347a-112">Get userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="6347a-112">Get userFlowLanguageConfiguration</span></span>](../api/userflowlanguageconfiguration-get.md)|[<span data-ttu-id="6347a-113">userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="6347a-113">userFlowLanguageConfiguration</span></span>](../resources/userflowlanguageconfiguration.md)|<span data-ttu-id="6347a-114">Ознакомьтесь с свойствами и отношениями [объекта userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6347a-114">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="6347a-115">Эти объекты представляют язык, доступный в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="6347a-115">These objects represent a language available in a user flow.</span></span>|
|[<span data-ttu-id="6347a-116">Список defaultPages</span><span class="sxs-lookup"><span data-stu-id="6347a-116">List defaultPages</span></span>](../api/userflowlanguageconfiguration-list-defaultpages.md)|<span data-ttu-id="6347a-117">[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="6347a-117">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="6347a-118">Получите ресурсы userFlowLanguagePage из свойства навигации defaultPages.</span><span class="sxs-lookup"><span data-stu-id="6347a-118">Get the userFlowLanguagePage resources from the defaultPages navigation property.</span></span> <span data-ttu-id="6347a-119">Представляет путь пользователя по умолчанию в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="6347a-119">Represents the default user journey in a user flow.</span></span>|
|[<span data-ttu-id="6347a-120">Переопределения списка</span><span class="sxs-lookup"><span data-stu-id="6347a-120">List overridesPages</span></span>](../api/userflowlanguageconfiguration-list-overridespages.md)|<span data-ttu-id="6347a-121">[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="6347a-121">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="6347a-122">Получите ресурсы userFlowLanguagePage из свойства навигации overridesPages.</span><span class="sxs-lookup"><span data-stu-id="6347a-122">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="6347a-123">Представляет настраиваемый интерфейс для пользовательского путешествия в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="6347a-123">Represents a custom experience for a user journey in a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="6347a-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="6347a-124">Properties</span></span>

|<span data-ttu-id="6347a-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="6347a-125">Property</span></span>|<span data-ttu-id="6347a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="6347a-126">Type</span></span>|<span data-ttu-id="6347a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="6347a-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6347a-128">id</span><span class="sxs-lookup"><span data-stu-id="6347a-128">id</span></span>|<span data-ttu-id="6347a-129">Строка</span><span class="sxs-lookup"><span data-stu-id="6347a-129">String</span></span>|<span data-ttu-id="6347a-130">Идентификатор языка.</span><span class="sxs-lookup"><span data-stu-id="6347a-130">The identifier of the language.</span></span> <span data-ttu-id="6347a-131">Это поле — тег языкового [ID RFC 5646,](https://tools.ietf.org/html/rfc5646) который должен быть документированным языковым ИД.</span><span class="sxs-lookup"><span data-stu-id="6347a-131">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span>|
|<span data-ttu-id="6347a-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6347a-132">isEnabled</span></span>|<span data-ttu-id="6347a-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="6347a-133">Boolean</span></span>|<span data-ttu-id="6347a-134">Указывает, включен ли язык в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="6347a-134">Indicates whether the language is enabled within the user flow.</span></span>|
|<span data-ttu-id="6347a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6347a-135">displayName</span></span>|<span data-ttu-id="6347a-136">Строка</span><span class="sxs-lookup"><span data-stu-id="6347a-136">String</span></span>|<span data-ttu-id="6347a-137">Отображаемая языковая фамилия.</span><span class="sxs-lookup"><span data-stu-id="6347a-137">The language name to display.</span></span> <span data-ttu-id="6347a-138">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6347a-138">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6347a-139">Связи</span><span class="sxs-lookup"><span data-stu-id="6347a-139">Relationships</span></span>

|<span data-ttu-id="6347a-140">Связь</span><span class="sxs-lookup"><span data-stu-id="6347a-140">Relationship</span></span>|<span data-ttu-id="6347a-141">Тип</span><span class="sxs-lookup"><span data-stu-id="6347a-141">Type</span></span>|<span data-ttu-id="6347a-142">Описание</span><span class="sxs-lookup"><span data-stu-id="6347a-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6347a-143">defaultPages</span><span class="sxs-lookup"><span data-stu-id="6347a-143">defaultPages</span></span>|<span data-ttu-id="6347a-144">[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="6347a-144">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="6347a-145">Коллекция страниц с контентом по умолчанию, отображаемым в потоке пользователей для указанного языка.</span><span class="sxs-lookup"><span data-stu-id="6347a-145">Collection of pages with the default content to display in a user flow for a specified language.</span></span> <span data-ttu-id="6347a-146">Эта коллекция не позволяет вносить какие-либо изменения.</span><span class="sxs-lookup"><span data-stu-id="6347a-146">This collection does not allow any kind of modification.</span></span>|
|<span data-ttu-id="6347a-147">overridesPages</span><span class="sxs-lookup"><span data-stu-id="6347a-147">overridesPages</span></span>|<span data-ttu-id="6347a-148">[коллекция userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="6347a-148">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="6347a-149">Коллекция страниц с переопределениями сообщений для отображения в потоке пользователей для указанного языка.</span><span class="sxs-lookup"><span data-stu-id="6347a-149">Collection of pages with the overrides messages to display in a user flow for a specified language.</span></span> <span data-ttu-id="6347a-150">Эта коллекция позволяет изменять только содержимое страницы, любые другие изменения не допускаются (создание или удаление страниц).</span><span class="sxs-lookup"><span data-stu-id="6347a-150">This collection only allows to modify the content of the page, any other modification is not allowed (creation or deletion of pages).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6347a-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6347a-151">JSON representation</span></span>

<span data-ttu-id="6347a-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6347a-152">The following is a JSON representation of the resource.</span></span>
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

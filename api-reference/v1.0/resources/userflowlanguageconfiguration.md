---
title: пользовательFlowLanguageКонфигурация типа ресурса
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
# <a name="userflowlanguageconfiguration-resource-type"></a><span data-ttu-id="88dd6-103">пользовательFlowLanguageКонфигурация типа ресурса</span><span class="sxs-lookup"><span data-stu-id="88dd6-103">userFlowLanguageConfiguration resource type</span></span>

<span data-ttu-id="88dd6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88dd6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88dd6-105">Позволяет потоку пользователей поддерживать использование нескольких языков.</span><span class="sxs-lookup"><span data-stu-id="88dd6-105">Allows a user flow to support the use of multiple languages.</span></span>

<span data-ttu-id="88dd6-106">Для [Azure Active Directory потоков пользователей,](/azure/active-directory/external-identities/user-flow-customize-language)вы можете использовать только встроенные языки, предоставляемые корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="88dd6-106">For [Azure Active Directory user flows](/azure/active-directory/external-identities/user-flow-customize-language), you can only leverage the built-in languages provided by Microsoft.</span></span> <span data-ttu-id="88dd6-107">Потоки пользователей для Azure Active Directory поддержки, определяющей язык и строки, показанные пользователям по мере их настройки с потоками пользователей.</span><span class="sxs-lookup"><span data-stu-id="88dd6-107">User flows for Azure Active Directory support defining the language and strings shown to users as they go through the journeys you configure with your user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="88dd6-108">Методы</span><span class="sxs-lookup"><span data-stu-id="88dd6-108">Methods</span></span>

|<span data-ttu-id="88dd6-109">Метод</span><span class="sxs-lookup"><span data-stu-id="88dd6-109">Method</span></span>|<span data-ttu-id="88dd6-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="88dd6-110">Return type</span></span>|<span data-ttu-id="88dd6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="88dd6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88dd6-112">Получить userFlowLanguageКонфигурация</span><span class="sxs-lookup"><span data-stu-id="88dd6-112">Get userFlowLanguageConfiguration</span></span>](../api/userflowlanguageconfiguration-get.md)|[<span data-ttu-id="88dd6-113">userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="88dd6-113">userFlowLanguageConfiguration</span></span>](../resources/userflowlanguageconfiguration.md)|<span data-ttu-id="88dd6-114">Прочитайте свойства и отношения объекта [пользователяFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88dd6-114">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="88dd6-115">Эти объекты представляют собой язык, доступный в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="88dd6-115">These objects represent a language available in a user flow.</span></span>|
|[<span data-ttu-id="88dd6-116">Список по умолчаниюВеся</span><span class="sxs-lookup"><span data-stu-id="88dd6-116">List defaultPages</span></span>](../api/userflowlanguageconfiguration-list-defaultpages.md)|<span data-ttu-id="88dd6-117">[userFlowLanguagePage](../resources/userflowlanguagepage.md) коллекция</span><span class="sxs-lookup"><span data-stu-id="88dd6-117">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="88dd6-118">Получите ресурсы userFlowLanguagePage из навигационного свойства defaultPages.</span><span class="sxs-lookup"><span data-stu-id="88dd6-118">Get the userFlowLanguagePage resources from the defaultPages navigation property.</span></span> <span data-ttu-id="88dd6-119">Представляет путешествие пользователя по умолчанию в потоке пользователя.</span><span class="sxs-lookup"><span data-stu-id="88dd6-119">Represents the default user journey in a user flow.</span></span>|
|[<span data-ttu-id="88dd6-120">Список переопределяетВит Страницы</span><span class="sxs-lookup"><span data-stu-id="88dd6-120">List overridesPages</span></span>](../api/userflowlanguageconfiguration-list-overridespages.md)|<span data-ttu-id="88dd6-121">[userFlowLanguagePage](../resources/userflowlanguagepage.md) коллекция</span><span class="sxs-lookup"><span data-stu-id="88dd6-121">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="88dd6-122">Получите ресурсы userFlowLanguagePage из свойства навигации overridesPages.</span><span class="sxs-lookup"><span data-stu-id="88dd6-122">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="88dd6-123">Представляет собой пользовательский интерфейс для путешествия пользователя в потоке пользователя.</span><span class="sxs-lookup"><span data-stu-id="88dd6-123">Represents a custom experience for a user journey in a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="88dd6-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="88dd6-124">Properties</span></span>

|<span data-ttu-id="88dd6-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="88dd6-125">Property</span></span>|<span data-ttu-id="88dd6-126">Тип</span><span class="sxs-lookup"><span data-stu-id="88dd6-126">Type</span></span>|<span data-ttu-id="88dd6-127">Описание</span><span class="sxs-lookup"><span data-stu-id="88dd6-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88dd6-128">id</span><span class="sxs-lookup"><span data-stu-id="88dd6-128">id</span></span>|<span data-ttu-id="88dd6-129">String</span><span class="sxs-lookup"><span data-stu-id="88dd6-129">String</span></span>|<span data-ttu-id="88dd6-130">Идентификатор языка.</span><span class="sxs-lookup"><span data-stu-id="88dd6-130">The identifier of the language.</span></span> <span data-ttu-id="88dd6-131">Это поле соответствует тегу Language ID [RFC 5646](https://tools.ietf.org/html/rfc5646) и должно быть задокументированным идентификатором языка.</span><span class="sxs-lookup"><span data-stu-id="88dd6-131">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span>|
|<span data-ttu-id="88dd6-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="88dd6-132">isEnabled</span></span>|<span data-ttu-id="88dd6-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="88dd6-133">Boolean</span></span>|<span data-ttu-id="88dd6-134">Указывает, включен ли язык в потоке пользователя.</span><span class="sxs-lookup"><span data-stu-id="88dd6-134">Indicates whether the language is enabled within the user flow.</span></span>|
|<span data-ttu-id="88dd6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="88dd6-135">displayName</span></span>|<span data-ttu-id="88dd6-136">String</span><span class="sxs-lookup"><span data-stu-id="88dd6-136">String</span></span>|<span data-ttu-id="88dd6-137">Название языка для отображения.</span><span class="sxs-lookup"><span data-stu-id="88dd6-137">The language name to display.</span></span> <span data-ttu-id="88dd6-138">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88dd6-138">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88dd6-139">Связи</span><span class="sxs-lookup"><span data-stu-id="88dd6-139">Relationships</span></span>

|<span data-ttu-id="88dd6-140">Связь</span><span class="sxs-lookup"><span data-stu-id="88dd6-140">Relationship</span></span>|<span data-ttu-id="88dd6-141">Тип</span><span class="sxs-lookup"><span data-stu-id="88dd6-141">Type</span></span>|<span data-ttu-id="88dd6-142">Описание</span><span class="sxs-lookup"><span data-stu-id="88dd6-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88dd6-143">по умолчаниюВееся</span><span class="sxs-lookup"><span data-stu-id="88dd6-143">defaultPages</span></span>|<span data-ttu-id="88dd6-144">[userFlowLanguagePage](../resources/userflowlanguagepage.md) коллекция</span><span class="sxs-lookup"><span data-stu-id="88dd6-144">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="88dd6-145">Сбор страниц с содержимым по умолчанию для отображения в пользовательском потоке для определенного языка.</span><span class="sxs-lookup"><span data-stu-id="88dd6-145">Collection of pages with the default content to display in a user flow for a specified language.</span></span> <span data-ttu-id="88dd6-146">Эта коллекция не допускает каких-либо изменений.</span><span class="sxs-lookup"><span data-stu-id="88dd6-146">This collection does not allow any kind of modification.</span></span>|
|<span data-ttu-id="88dd6-147">переопределяет Страницы</span><span class="sxs-lookup"><span data-stu-id="88dd6-147">overridesPages</span></span>|<span data-ttu-id="88dd6-148">[userFlowLanguagePage](../resources/userflowlanguagepage.md) коллекция</span><span class="sxs-lookup"><span data-stu-id="88dd6-148">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="88dd6-149">Сбор страниц с переопределениями сообщений для отображения в пользовательском потоке для определенного языка.</span><span class="sxs-lookup"><span data-stu-id="88dd6-149">Collection of pages with the overrides messages to display in a user flow for a specified language.</span></span> <span data-ttu-id="88dd6-150">Эта коллекция позволяет изменять только содержимое страницы, любая другая модификация не допускается (создание или удаление страниц).</span><span class="sxs-lookup"><span data-stu-id="88dd6-150">This collection only allows to modify the content of the page, any other modification is not allowed (creation or deletion of pages).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88dd6-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88dd6-151">JSON representation</span></span>

<span data-ttu-id="88dd6-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88dd6-152">The following is a JSON representation of the resource.</span></span>
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

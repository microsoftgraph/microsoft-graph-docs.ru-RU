---
title: тип ресурса translationPreferences
description: Ресурс, представляющий параметры параметров перевода пользователя.
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: b2e45f797709067e52f142c3de3f2be566b55201
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518169"
---
# <a name="translationpreferences-resource-type"></a><span data-ttu-id="547bc-103">тип ресурса translationPreferences</span><span class="sxs-lookup"><span data-stu-id="547bc-103">translationPreferences resource type</span></span>

<span data-ttu-id="547bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="547bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="547bc-105">Представляет запись в переопределяемом списке языка перевода пользователя.</span><span class="sxs-lookup"><span data-stu-id="547bc-105">Represents an entry in a user's translation language override list.</span></span>

## <a name="properties"></a><span data-ttu-id="547bc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="547bc-106">Properties</span></span>

|<span data-ttu-id="547bc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="547bc-107">Property</span></span>             |<span data-ttu-id="547bc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="547bc-108">Type</span></span>                                         |<span data-ttu-id="547bc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="547bc-109">Description</span></span>                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|<span data-ttu-id="547bc-110">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="547bc-110">translationBehavior</span></span>  |[<span data-ttu-id="547bc-111">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="547bc-111">translationBehavior</span></span>](#translationbehavior-values)       |<span data-ttu-id="547bc-112">Предпочтительное поведение пользователя для перевода.</span><span class="sxs-lookup"><span data-stu-id="547bc-112">The user's preferred translation behavior.</span></span><br><br><span data-ttu-id="547bc-113">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="547bc-113">Returned by default.</span></span> <span data-ttu-id="547bc-114">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="547bc-114">Not nullable.</span></span> |                   
|<span data-ttu-id="547bc-115">LanguageOverrides</span><span class="sxs-lookup"><span data-stu-id="547bc-115">languageOverrides</span></span>    |<span data-ttu-id="547bc-116">[коллекция translationLanguageOverride](translationLanguageOverride.md)</span><span class="sxs-lookup"><span data-stu-id="547bc-116">[translationLanguageOverride](translationLanguageOverride.md) collection</span></span>                | <span data-ttu-id="547bc-117">Переопределять поведение для языков, если таково.</span><span class="sxs-lookup"><span data-stu-id="547bc-117">Translation override behavior for languages, if any.</span></span><br><br><span data-ttu-id="547bc-118">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="547bc-118">Returned by default.</span></span>|
|<span data-ttu-id="547bc-119">untranslatedLanguages</span><span class="sxs-lookup"><span data-stu-id="547bc-119">untranslatedLanguages</span></span>|<span data-ttu-id="547bc-120">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="547bc-120">String collection</span></span>| <span data-ttu-id="547bc-121">Список языков, которые пользователю не нужно переводить.</span><span class="sxs-lookup"><span data-stu-id="547bc-121">The list of languages the user does not need translated.</span></span> <span data-ttu-id="547bc-122">Это вычисляется из коллекции **authoringLanguages** в [regionalAndLanguageSettings](regionalandlanguagesettings.md)и **коллекции languageOverrides** в **translationPreferences.**</span><span class="sxs-lookup"><span data-stu-id="547bc-122">This is computed from the **authoringLanguages** collection in [regionalAndLanguageSettings](regionalandlanguagesettings.md), and the **languageOverrides** collection in **translationPreferences**.</span></span> <span data-ttu-id="547bc-123">В списке указаны нейтральные культурные значения, которые включают языковый код без какой-либо страны или региона.</span><span class="sxs-lookup"><span data-stu-id="547bc-123">The list specifies neutral culture values that include the language code without any country or region association.</span></span> <span data-ttu-id="547bc-124">Например, он указывает "fr" для нейтральной французской культуры, но не "fr-FR" для французской культуры во Франции.</span><span class="sxs-lookup"><span data-stu-id="547bc-124">For example, it would specify "fr" for the neutral French culture, but not "fr-FR" for the French culture in France.</span></span> <br><br><span data-ttu-id="547bc-125">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="547bc-125">Returned by default.</span></span> <span data-ttu-id="547bc-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="547bc-126">Read only.</span></span>| 

### <a name="translationbehavior-values"></a><span data-ttu-id="547bc-127">значения translationBehavior</span><span class="sxs-lookup"><span data-stu-id="547bc-127">translationBehavior values</span></span>

|<span data-ttu-id="547bc-128">Member</span><span class="sxs-lookup"><span data-stu-id="547bc-128">Member</span></span> |<span data-ttu-id="547bc-129">Описание</span><span class="sxs-lookup"><span data-stu-id="547bc-129">Description</span></span>                                                                  |
|-------|-----------------------------------------------------------------------------|
|<span data-ttu-id="547bc-130">Спросите</span><span class="sxs-lookup"><span data-stu-id="547bc-130">Ask</span></span>    |<span data-ttu-id="547bc-131">Запрос пользователя перед переводом сообщений/чатов/веб-страниц для пользователя.</span><span class="sxs-lookup"><span data-stu-id="547bc-131">Prompt the user before translating the messages/chats/web pages for the user.</span></span>|
|<span data-ttu-id="547bc-132">Да</span><span class="sxs-lookup"><span data-stu-id="547bc-132">Yes</span></span>    |<span data-ttu-id="547bc-133">Автоматически перевод сообщений/чатов/веб-страниц для пользователя.</span><span class="sxs-lookup"><span data-stu-id="547bc-133">Automatically translate the messages/chats/web pages for the user.</span></span>           |
|<span data-ttu-id="547bc-134">Нет</span><span class="sxs-lookup"><span data-stu-id="547bc-134">No</span></span>     |<span data-ttu-id="547bc-135">Не предлагай пользователю подсказок или автоматический перевод.</span><span class="sxs-lookup"><span data-stu-id="547bc-135">Do not offer prompted or automatic translation for the user.</span></span>                 |



## <a name="json-representation"></a><span data-ttu-id="547bc-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="547bc-136">JSON representation</span></span>

<span data-ttu-id="547bc-137">Ниже приводится определение ресурса JSON.</span><span class="sxs-lookup"><span data-stu-id="547bc-137">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.translationPreferences"
}-->

```json
{
    "translationBehavior": "string",
    "languageOverrides": [{"@odata.type":"microsoft.graph.translationLanguageOverride"}],
    "untranslatedLanguages": ["string"]
}
```
<!-- {
  "type": "#page.annotation",
  "description": translationPreferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



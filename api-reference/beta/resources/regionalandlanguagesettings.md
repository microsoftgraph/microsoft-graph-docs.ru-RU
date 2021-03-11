---
title: тип ресурса regionalAndLanguageSettings
description: Ресурс, представляющий региональные и языковые предпочтения пользователей
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 25af8de5a93bc67ed774b161ec63c1698434efb2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721315"
---
# <a name="regionalandlanguagesettings-resource-type"></a><span data-ttu-id="6b1e1-103">тип ресурса regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="6b1e1-103">regionalAndLanguageSettings resource type</span></span>

<span data-ttu-id="6b1e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b1e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b1e1-105">Открытый тип, который представляет предпочтения пользователя для языков в различных контекстах, а также для регионального языка и форматирования, который диски календаря по умолчанию, и форматирование для даты и времени.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-105">An open type that represents a user's preferences for languages in various contexts, and for regional locale and formatting that drives the default calendar, and formatting for date and time.</span></span>

## <a name="methods"></a><span data-ttu-id="6b1e1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6b1e1-106">Methods</span></span>

| <span data-ttu-id="6b1e1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6b1e1-107">Method</span></span>                                                 | <span data-ttu-id="6b1e1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6b1e1-108">Return Type</span></span>                                                   | <span data-ttu-id="6b1e1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6b1e1-109">Description</span></span>                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6b1e1-110">[получение](../api/regionalAndLanguageSettings-get.md);</span><span class="sxs-lookup"><span data-stu-id="6b1e1-110">[Get](../api/regionalAndLanguageSettings-get.md)</span></span>       | [<span data-ttu-id="6b1e1-111">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="6b1e1-111">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="6b1e1-112">Чтение свойств объекта **regionalAndLanguageSettings.**</span><span class="sxs-lookup"><span data-stu-id="6b1e1-112">Read properties of a **regionalAndLanguageSettings** object.</span></span>                                       |
| [<span data-ttu-id="6b1e1-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="6b1e1-113">Update</span></span>](../api/regionalandlanguagesettings-update.md) | [<span data-ttu-id="6b1e1-114">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="6b1e1-114">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="6b1e1-115">Обновление всех или подмножества свойств объекта **regionalAndLanguageSettings** для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-115">Update all or a subset of the properties of the **regionalAndLanguageSettings** object for a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="6b1e1-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b1e1-116">Properties</span></span>
| <span data-ttu-id="6b1e1-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b1e1-117">Property</span></span>                   | <span data-ttu-id="6b1e1-118">Тип</span><span class="sxs-lookup"><span data-stu-id="6b1e1-118">Type</span></span>                                                  | <span data-ttu-id="6b1e1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6b1e1-119">Description</span></span>                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6b1e1-120">defaultDisplayLanguage</span><span class="sxs-lookup"><span data-stu-id="6b1e1-120">defaultDisplayLanguage</span></span>     | [<span data-ttu-id="6b1e1-121">localeInfo</span><span class="sxs-lookup"><span data-stu-id="6b1e1-121">localeInfo</span></span>](localeinfo.md)                           | <span data-ttu-id="6b1e1-122">Предпочтительный язык пользовательского интерфейса пользователя (меню, кнопки, ленты, предупреждающие сообщения) для веб-приложений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-122">The  user's preferred user interface language (menus, buttons, ribbons, warning messages) for Microsoft web applications.</span></span><br><br><span data-ttu-id="6b1e1-123">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-123">Returned by default.</span></span> <span data-ttu-id="6b1e1-124">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-124">Not nullable.</span></span> |
| <span data-ttu-id="6b1e1-125">authoringLanguages</span><span class="sxs-lookup"><span data-stu-id="6b1e1-125">authoringLanguages</span></span>         | <span data-ttu-id="6b1e1-126">Коллекция объектов [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="6b1e1-126">[localeInfo](localeinfo.md) collection</span></span>                                 | <span data-ttu-id="6b1e1-127">Приоритизированный список языков, на которые пользователь читает и авторов.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-127">Prioritized list of languages the user reads and authors in.</span></span><br><br><span data-ttu-id="6b1e1-128">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-128">Returned by default.</span></span> <span data-ttu-id="6b1e1-129">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-129">Not nullable.</span></span>                                                              |
| <span data-ttu-id="6b1e1-130">defaultTranslationLanguage</span><span class="sxs-lookup"><span data-stu-id="6b1e1-130">defaultTranslationLanguage</span></span> | [<span data-ttu-id="6b1e1-131">localeInfo</span><span class="sxs-lookup"><span data-stu-id="6b1e1-131">localeInfo</span></span>](localeinfo.md)                 | <span data-ttu-id="6b1e1-132">Язык, на который пользователь ожидает перевода документов, электронной почты и сообщений.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-132">The language a user expects to have documents, emails, and messages translated into.</span></span><br><br><span data-ttu-id="6b1e1-133">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-133">Returned by default.</span></span>                                                    |
| <span data-ttu-id="6b1e1-134">defaultSpeechInputLanguage</span><span class="sxs-lookup"><span data-stu-id="6b1e1-134">defaultSpeechInputLanguage</span></span> | [<span data-ttu-id="6b1e1-135">localeInfo</span><span class="sxs-lookup"><span data-stu-id="6b1e1-135">localeInfo</span></span>](localeinfo.md)                 | <span data-ttu-id="6b1e1-136">Язык, который пользователь должен использовать в качестве ввода для текстовых сценариев речи.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-136">The language a user expected to use as input for text to speech scenarios.</span></span><br><br><span data-ttu-id="6b1e1-137">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-137">Returned by default.</span></span>                                                              |
| <span data-ttu-id="6b1e1-138">defaultRegionalFormat</span><span class="sxs-lookup"><span data-stu-id="6b1e1-138">defaultRegionalFormat</span></span>      | [<span data-ttu-id="6b1e1-139">localeInfo</span><span class="sxs-lookup"><span data-stu-id="6b1e1-139">localeInfo</span></span>](localeinfo.md)            | <span data-ttu-id="6b1e1-140">Локализ, который диски по умолчанию даты, времени и форматирования календаря.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-140">The locale that drives the default date, time, and calendar formatting.</span></span><br><br><span data-ttu-id="6b1e1-141">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-141">Returned by default.</span></span>                                                                 |
| <span data-ttu-id="6b1e1-142">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="6b1e1-142">regionalFormatOverrides</span></span>    | [<span data-ttu-id="6b1e1-143">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="6b1e1-143">regionalFormatOverrides</span></span>](regionalformatoverrides.md) | <span data-ttu-id="6b1e1-144">Позволяет пользователю переопределять значение defaultRegionalFormat с помощью определенных форматов поля.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-144">Allows a user to override their defaultRegionalFormat with field specific formats.</span></span><br><br><span data-ttu-id="6b1e1-145">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-145">Returned by default.</span></span>                                                      |
| <span data-ttu-id="6b1e1-146">translationPreferences</span><span class="sxs-lookup"><span data-stu-id="6b1e1-146">translationPreferences</span></span>     | [<span data-ttu-id="6b1e1-147">translationPreferences</span><span class="sxs-lookup"><span data-stu-id="6b1e1-147">translationPreferences</span></span>](translationPreferences.md)   | <span data-ttu-id="6b1e1-148">Предпочтительные параметры пользователя при потреблении переведенных документов, электронной почты, сообщений и веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-148">The user's preferred settings when consuming translated documents, emails, messages, and websites.</span></span><br><br><span data-ttu-id="6b1e1-149">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-149">Returned by default.</span></span> <span data-ttu-id="6b1e1-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-150">Not nullable.</span></span>                                       |

## <a name="json-representation"></a><span data-ttu-id="6b1e1-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b1e1-151">JSON representation</span></span>

<span data-ttu-id="6b1e1-152">Ниже приводится определение ресурса JSON.</span><span class="sxs-lookup"><span data-stu-id="6b1e1-152">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings"
} -->

```json
{
    "defaultDisplayLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "authoringLanguages": [{"@odata.type":"microsoft.graph.localeInfo"}],
    "defaultTranslationLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultSpeechInputLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultRegionalFormat": {"@odata.type":"microsoft.graph.localeInfo"},
    "regionalFormatOverrides": {"@odata.type":"microsoft.graph.regionalFormatOverrides"},
    "translationPreferences":{"@odata.type":"microsoft.graph.translationPreferences"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



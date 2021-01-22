---
title: Тип ресурса regionalAndLanguageSettings
description: Ресурс, представляющий региональные и языковые параметры пользователей
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 66734cba4c5d0e2997a4bfd5b70c54156821f5da
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934914"
---
# <a name="regionalandlanguagesettings-resource-type"></a><span data-ttu-id="2fdd3-103">Тип ресурса regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="2fdd3-103">regionalAndLanguageSettings resource type</span></span>

<span data-ttu-id="2fdd3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fdd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fdd3-105">Открытый тип, который представляет предпочтения пользователя для языков в различных контекстах, а также региональных стандартов и форматирования, на котором задается календарь по умолчанию, и форматирования для даты и времени.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-105">An open type that represents a user's preferences for languages in various contexts, and for regional locale and formatting that drives the default calendar, and formatting for date and time.</span></span>

## <a name="methods"></a><span data-ttu-id="2fdd3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2fdd3-106">Methods</span></span>

| <span data-ttu-id="2fdd3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2fdd3-107">Method</span></span>                                                 | <span data-ttu-id="2fdd3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2fdd3-108">Return Type</span></span>                                                   | <span data-ttu-id="2fdd3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2fdd3-109">Description</span></span>                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2fdd3-110">[получение](../api/regionalAndLanguageSettings-get.md);</span><span class="sxs-lookup"><span data-stu-id="2fdd3-110">[Get](../api/regionalAndLanguageSettings-get.md)</span></span>       | [<span data-ttu-id="2fdd3-111">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="2fdd3-111">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="2fdd3-112">Чтение свойств объекта **regionalAndLanguageSettings.**</span><span class="sxs-lookup"><span data-stu-id="2fdd3-112">Read properties of a **regionalAndLanguageSettings** object.</span></span>                                       |
| <span data-ttu-id="2fdd3-113">[обновление](../api/regionalandlanguagesettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="2fdd3-113">[Update](../api/regionalandlanguagesettings-update.md)</span></span> | [<span data-ttu-id="2fdd3-114">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="2fdd3-114">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="2fdd3-115">Обновление всех или подмножества свойств объекта **regionalAndLanguageSettings** для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-115">Update all or a subset of the properties of the **regionalAndLanguageSettings** object for a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="2fdd3-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="2fdd3-116">Properties</span></span>
| <span data-ttu-id="2fdd3-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fdd3-117">Property</span></span>                   | <span data-ttu-id="2fdd3-118">Тип</span><span class="sxs-lookup"><span data-stu-id="2fdd3-118">Type</span></span>                                                  | <span data-ttu-id="2fdd3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2fdd3-119">Description</span></span>                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2fdd3-120">defaultDisplayLanguage</span><span class="sxs-lookup"><span data-stu-id="2fdd3-120">defaultDisplayLanguage</span></span>     | [<span data-ttu-id="2fdd3-121">localeInfo</span><span class="sxs-lookup"><span data-stu-id="2fdd3-121">localeInfo</span></span>](localeinfo.md)                           | <span data-ttu-id="2fdd3-122">Предпочитаемый пользователем язык пользовательского интерфейса (меню, кнопки, ленты, предупреждения) для веб-приложений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-122">The  user's preferred user interface language (menus, buttons, ribbons, warning messages) for Microsoft web applications.</span></span><br><br><span data-ttu-id="2fdd3-123">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-123">Returned by default.</span></span> <span data-ttu-id="2fdd3-124">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-124">Not nullable.</span></span> |
| <span data-ttu-id="2fdd3-125">authoringLanguages</span><span class="sxs-lookup"><span data-stu-id="2fdd3-125">authoringLanguages</span></span>         | <span data-ttu-id="2fdd3-126">Коллекция объектов localeInfo</span><span class="sxs-lookup"><span data-stu-id="2fdd3-126">localeInfo collection</span></span>                                 | <span data-ttu-id="2fdd3-127">Приоритетный список языков, на которые пользователь читает и авторов.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-127">Prioritized list of languages the user reads and authors in.</span></span><br><br><span data-ttu-id="2fdd3-128">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-128">Returned by default.</span></span> <span data-ttu-id="2fdd3-129">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-129">Not nullable.</span></span>                                                              |
| <span data-ttu-id="2fdd3-130">defaultTranslationLanguage</span><span class="sxs-lookup"><span data-stu-id="2fdd3-130">defaultTranslationLanguage</span></span> | <span data-ttu-id="2fdd3-131">localeInfo</span><span class="sxs-lookup"><span data-stu-id="2fdd3-131">localeInfo</span></span>                                            | <span data-ttu-id="2fdd3-132">Язык, на который пользователь ожидает перевода документов, сообщений электронной почты и сообщений.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-132">The language a user expects to have documents, emails, and messages translated into.</span></span><br><br><span data-ttu-id="2fdd3-133">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-133">Returned by default.</span></span>                                                    |
| <span data-ttu-id="2fdd3-134">defaultSpeechInputLanguage</span><span class="sxs-lookup"><span data-stu-id="2fdd3-134">defaultSpeechInputLanguage</span></span> | <span data-ttu-id="2fdd3-135">localeInfo</span><span class="sxs-lookup"><span data-stu-id="2fdd3-135">localeInfo</span></span>                                            | <span data-ttu-id="2fdd3-136">Язык, который пользователь должен использовать в качестве входных данных для текста в речевой сценарий.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-136">The language a user expected to use as input for text to speech scenarios.</span></span><br><br><span data-ttu-id="2fdd3-137">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-137">Returned by default.</span></span>                                                              |
| <span data-ttu-id="2fdd3-138">defaultRegionalFormat</span><span class="sxs-lookup"><span data-stu-id="2fdd3-138">defaultRegionalFormat</span></span>      | <span data-ttu-id="2fdd3-139">localeInfo</span><span class="sxs-lookup"><span data-stu-id="2fdd3-139">localeInfo</span></span>                                            | <span data-ttu-id="2fdd3-140">Региональные стандарты, которые будут управлять форматированием даты, времени и календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-140">The locale that drives the default date, time, and calendar formatting.</span></span><br><br><span data-ttu-id="2fdd3-141">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-141">Returned by default.</span></span>                                                                 |
| <span data-ttu-id="2fdd3-142">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="2fdd3-142">regionalFormatOverrides</span></span>    | [<span data-ttu-id="2fdd3-143">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="2fdd3-143">regionalFormatOverrides</span></span>](regionalformatoverrides.md) | <span data-ttu-id="2fdd3-144">Позволяет пользователю переопределять свой defaultRegionalFormat с помощью форматов, определенных для поля.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-144">Allows a user to override their defaultRegionalFormat with field specific formats.</span></span><br><br><span data-ttu-id="2fdd3-145">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-145">Returned by default.</span></span>                                                      |

## <a name="json-representation"></a><span data-ttu-id="2fdd3-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2fdd3-146">JSON representation</span></span>

<span data-ttu-id="2fdd3-147">Ниже приводится определение ресурса в JSON.</span><span class="sxs-lookup"><span data-stu-id="2fdd3-147">The following is a JSON definition of the resource.</span></span>

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
    "regionalFormatOverrides": {"@odata.type":"microsoft.graph.regionalFormatOverrides"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



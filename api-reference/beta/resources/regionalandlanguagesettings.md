---
title: Тип ресурса Регионаландлангуажесеттингс
description: Ресурс, представляющий региональные и языковые параметры пользователей
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 096a59f9e153c7395e1263cc32ec01c2fda01ce2
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744233"
---
# <a name="regionalandlanguagesettings-resource-type"></a><span data-ttu-id="08678-103">Тип ресурса Регионаландлангуажесеттингс</span><span class="sxs-lookup"><span data-stu-id="08678-103">regionalAndLanguageSettings resource type</span></span>

<span data-ttu-id="08678-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08678-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08678-105">Открытый тип, который представляет предпочтения пользователя для языков в различных контекстах, а также для региональных языковых стандартов и форматирования, которые заменяют календарь по умолчанию и форматирование даты и времени.</span><span class="sxs-lookup"><span data-stu-id="08678-105">An open type that represents a user's preferences for languages in various contexts, and for regional locale and formatting that drives the default calendar, and formatting for date and time.</span></span>

## <a name="methods"></a><span data-ttu-id="08678-106">Методы</span><span class="sxs-lookup"><span data-stu-id="08678-106">Methods</span></span>

| <span data-ttu-id="08678-107">Метод</span><span class="sxs-lookup"><span data-stu-id="08678-107">Method</span></span>                                                          | <span data-ttu-id="08678-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="08678-108">Return Type</span></span>                                                    | <span data-ttu-id="08678-109">Описание</span><span class="sxs-lookup"><span data-stu-id="08678-109">Description</span></span>                                                                                  |
| :-------------------------------------------------------------- | :------------------------------------------------------------- | :------------------------------------------------------------------------------------------- |
| <span data-ttu-id="08678-110">[получение](../api/regionalAndLanguageSettings-get.md);</span><span class="sxs-lookup"><span data-stu-id="08678-110">[Get](../api/regionalAndLanguageSettings-get.md)</span></span>        | [<span data-ttu-id="08678-111">регионаландлангуажесеттингс</span><span class="sxs-lookup"><span data-stu-id="08678-111">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md)  | <span data-ttu-id="08678-112">Чтение свойств объекта **регионаландлангуажесеттингс** .</span><span class="sxs-lookup"><span data-stu-id="08678-112">Read properties of a **regionalAndLanguageSettings** object.</span></span>               |                           |
| [<span data-ttu-id="08678-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="08678-113">Update</span></span>](../api/regionalandlanguagesettings-update.md)  | [<span data-ttu-id="08678-114">регионаландлангуажесеттингс</span><span class="sxs-lookup"><span data-stu-id="08678-114">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md)  | <span data-ttu-id="08678-115">Обновление всех или подмножества свойств объекта **регионаландлангуажесеттингс** для пользователя.</span><span class="sxs-lookup"><span data-stu-id="08678-115">Update all or a subset of the properties of the **regionalAndLanguageSettings** object for a user.</span></span>                                |

## <a name="properties"></a><span data-ttu-id="08678-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="08678-116">Properties</span></span>
|<span data-ttu-id="08678-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="08678-117">Property</span></span>                     |<span data-ttu-id="08678-118">Тип</span><span class="sxs-lookup"><span data-stu-id="08678-118">Type</span></span>                 |<span data-ttu-id="08678-119">Описание</span><span class="sxs-lookup"><span data-stu-id="08678-119">Description</span></span>          |
|-----------------------------|---------------------|--------------------|
|<span data-ttu-id="08678-120">дефаултдисплайлангуаже</span><span class="sxs-lookup"><span data-stu-id="08678-120">defaultDisplayLanguage</span></span>             |[<span data-ttu-id="08678-121">localeInfo</span><span class="sxs-lookup"><span data-stu-id="08678-121">localeInfo</span></span>](localeinfo.md)                     |<span data-ttu-id="08678-122">Предпочтительный язык пользовательского интерфейса пользователя (меню, кнопки, ленты, предупреждающие сообщения) для веб-приложений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="08678-122">The  user's preferred user interface language (menus, buttons, ribbons, warning messages) for Microsoft web applications.</span></span><br><br><span data-ttu-id="08678-123">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="08678-123">Returned by default.</span></span> <span data-ttu-id="08678-124">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="08678-124">Not nullable.</span></span>|
|<span data-ttu-id="08678-125">аусоринглангуажес</span><span class="sxs-lookup"><span data-stu-id="08678-125">authoringLanguages</span></span>                 |<span data-ttu-id="08678-126">Коллекция объектов localeInfo</span><span class="sxs-lookup"><span data-stu-id="08678-126">localeInfo collection</span></span>        |<span data-ttu-id="08678-127">Приоритетный список языков, в которых пользователь читает и авторы.</span><span class="sxs-lookup"><span data-stu-id="08678-127">Prioritized list of languages the user reads and authors in.</span></span><br><br><span data-ttu-id="08678-128">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="08678-128">Returned by default.</span></span> <span data-ttu-id="08678-129">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="08678-129">Not nullable.</span></span>|
|<span data-ttu-id="08678-130">дефаулттранслатионлангуаже</span><span class="sxs-lookup"><span data-stu-id="08678-130">defaultTranslationLanguage</span></span>         |<span data-ttu-id="08678-131">localeInfo</span><span class="sxs-lookup"><span data-stu-id="08678-131">localeInfo</span></span>                   |<span data-ttu-id="08678-132">Язык, на который пользователь ожидает документы, сообщения электронной почты и сообщения, преобразованные в.</span><span class="sxs-lookup"><span data-stu-id="08678-132">The language a user expects to have documents, emails, and messages translated into.</span></span><br><br><span data-ttu-id="08678-133">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="08678-133">Returned by default.</span></span>|
|<span data-ttu-id="08678-134">дефаултспичинпутлангуаже</span><span class="sxs-lookup"><span data-stu-id="08678-134">defaultSpeechInputLanguage</span></span>         |<span data-ttu-id="08678-135">localeInfo</span><span class="sxs-lookup"><span data-stu-id="08678-135">localeInfo</span></span>                   |<span data-ttu-id="08678-136">Язык, который пользователь должен использовать в качестве входных данных для сценариев преобразования текста в речь.</span><span class="sxs-lookup"><span data-stu-id="08678-136">The language a user expected to use as input for text to speech scenarios.</span></span><br><br><span data-ttu-id="08678-137">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="08678-137">Returned by default.</span></span>|
|<span data-ttu-id="08678-138">дефаултрегионалформат</span><span class="sxs-lookup"><span data-stu-id="08678-138">defaultRegionalFormat</span></span>              |<span data-ttu-id="08678-139">localeInfo</span><span class="sxs-lookup"><span data-stu-id="08678-139">localeInfo</span></span>                     |<span data-ttu-id="08678-140">Языковой стандарт, который управляет форматированием даты, времени и календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="08678-140">The locale that drives the default date, time, and calendar formatting.</span></span><br><br><span data-ttu-id="08678-141">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="08678-141">Returned by default.</span></span>|
|<span data-ttu-id="08678-142">регионалформатоверридес</span><span class="sxs-lookup"><span data-stu-id="08678-142">regionalFormatOverrides</span></span>            |[<span data-ttu-id="08678-143">регионалформатоверридес</span><span class="sxs-lookup"><span data-stu-id="08678-143">regionalFormatOverrides</span></span>](regionalformatoverrides.md)    |<span data-ttu-id="08678-144">Позволяет пользователю переопределять свои Дефаултрегионалформат с использованием определенных форматов полей.</span><span class="sxs-lookup"><span data-stu-id="08678-144">Allows a user to override their defaultRegionalFormat with field specific formats.</span></span><br><br><span data-ttu-id="08678-145">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="08678-145">Returned by default.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08678-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08678-146">JSON representation</span></span>

<span data-ttu-id="08678-147">Ниже приведено определение ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08678-147">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings"
} -->

```json
{
    "defaultDisplayLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "authoringLanguages":[{"@odata.type":"microsoft.graph.localeInfo"}] ,
    "defaultTranslationLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultSpeechInputLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultRegionalFormat":{"@odata.type":"microsoft.graph.localeInfo"} ,
    "regionalFormatOverrides":{"@odata.type":"microsoft.graph.regionalFormatOverrides"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Тип ресурса Профилекарданнотатион
description: Позволяет администратору настраивать внешний вид выбранных полей в карточке профиля Microsoft 365.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 57b6378c811727676f7b34c1812955639598054b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973732"
---
# <a name="profilecardannotation-resource-type"></a><span data-ttu-id="6b441-103">Тип ресурса Профилекарданнотатион</span><span class="sxs-lookup"><span data-stu-id="6b441-103">profileCardAnnotation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b441-104">Используется для задания настраиваемого отображаемого имени для полей, которые находятся в общей программе Microsoft 365 People експериинце.</span><span class="sxs-lookup"><span data-stu-id="6b441-104">Used to set a custom display name for fields that surface in a shared Microsoft 365 people experieence.</span></span> <span data-ttu-id="6b441-105">Администратор может определить строку отображаемого имени по умолчанию и набор альтернативных переводов для языков, которые они поддерживают в Организации.</span><span class="sxs-lookup"><span data-stu-id="6b441-105">An administrator can define a default display name string and a set of alternative translations for the languages that they support in their organization.</span></span>

## <a name="properties"></a><span data-ttu-id="6b441-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b441-106">Properties</span></span>

| <span data-ttu-id="6b441-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b441-107">Property</span></span>     | <span data-ttu-id="6b441-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6b441-108">Type</span></span>                                                            | <span data-ttu-id="6b441-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6b441-109">Description</span></span>                                                                                                                       |
|:-------------|:----------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="6b441-110">displayName</span><span class="sxs-lookup"><span data-stu-id="6b441-110">displayName</span></span>   |<span data-ttu-id="6b441-111">String</span><span class="sxs-lookup"><span data-stu-id="6b441-111">String</span></span>                                                           | <span data-ttu-id="6b441-112">Если этот параметр задан, значение этого поля используется картой профиля в качестве метки свойства по умолчанию (например, "центр затрат").</span><span class="sxs-lookup"><span data-stu-id="6b441-112">If present, the value of this field is used by the profile card as the default property label in the experience (for example, "Cost Center").</span></span> |
|<span data-ttu-id="6b441-113">Локализация</span><span class="sxs-lookup"><span data-stu-id="6b441-113">localizations</span></span> |<span data-ttu-id="6b441-114">Коллекция [дисплайнамелокализатион](displaynamelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="6b441-114">[displayNameLocalization](displaynamelocalization.md) collection</span></span> | <span data-ttu-id="6b441-115">Каждый ресурс в этой коллекции представляет локализованное значение имени атрибута для определенного языка, используемого в качестве метки по умолчанию для этого языкового стандарта.</span><span class="sxs-lookup"><span data-stu-id="6b441-115">Each resource in this collection represents the localized value of the attribute name for a given language, used as the default label for that locale.</span></span> <span data-ttu-id="6b441-116">Например, пользователь с `no-NB` клиентом получает значение "Костнадс Sent" в качестве метки атрибута, а не "центр затрат".</span><span class="sxs-lookup"><span data-stu-id="6b441-116">For example, a user with a `no-NB` client gets "Kostnads Senter" as the attribute label, rather than "Cost Center."</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b441-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b441-117">JSON representation</span></span>

<span data-ttu-id="6b441-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b441-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardAnnotation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "localizations": [
    {
      "displayName": "String",
      "languageTag": "String"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profileCardAnnotation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



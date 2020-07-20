---
title: Тип ресурса Профилекарданнотатион
description: Позволяет администратору настраивать внешний вид выбранных полей в карточке профиля Microsoft 365.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 973732dc92527dcf3795b8796e1c817ba880836c
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051062"
---
# <a name="profilecardannotation-resource-type"></a><span data-ttu-id="dbc3c-103">Тип ресурса Профилекарданнотатион</span><span class="sxs-lookup"><span data-stu-id="dbc3c-103">profileCardAnnotation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbc3c-104">Используется для задания настраиваемого отображаемого имени для полей, которые находятся в общей программе Microsoft 365 People експериинце.</span><span class="sxs-lookup"><span data-stu-id="dbc3c-104">Used to set a custom display name for fields that surface in a shared Microsoft 365 people experieence.</span></span> <span data-ttu-id="dbc3c-105">Администратор может определить строку отображаемого имени по умолчанию и набор альтернативных переводов для языков, которые они поддерживают в Организации.</span><span class="sxs-lookup"><span data-stu-id="dbc3c-105">An administrator can define a default display name string and a set of alternative translations for the languages that they support in their organization.</span></span>

## <a name="properties"></a><span data-ttu-id="dbc3c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbc3c-106">Properties</span></span>

| <span data-ttu-id="dbc3c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbc3c-107">Property</span></span>     | <span data-ttu-id="dbc3c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="dbc3c-108">Type</span></span>                                                            | <span data-ttu-id="dbc3c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dbc3c-109">Description</span></span>                                                                                                                       |
|:-------------|:----------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="dbc3c-110">displayName</span><span class="sxs-lookup"><span data-stu-id="dbc3c-110">displayName</span></span>   |<span data-ttu-id="dbc3c-111">String</span><span class="sxs-lookup"><span data-stu-id="dbc3c-111">String</span></span>                                                           | <span data-ttu-id="dbc3c-112">Если этот параметр задан, значение этого поля используется картой профиля в качестве метки свойства по умолчанию (например, "центр затрат").</span><span class="sxs-lookup"><span data-stu-id="dbc3c-112">If present, the value of this field is used by the profile card as the default property label in the experience (for example, "Cost Center").</span></span> |
|<span data-ttu-id="dbc3c-113">Локализация</span><span class="sxs-lookup"><span data-stu-id="dbc3c-113">localizations</span></span> |<span data-ttu-id="dbc3c-114">Коллекция [дисплайнамелокализатион](displaynamelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="dbc3c-114">[displayNameLocalization](displaynamelocalization.md) collection</span></span> | <span data-ttu-id="dbc3c-115">Каждый ресурс в этой коллекции представляет локализованное значение имени атрибута для определенного языка, используемого в качестве метки по умолчанию для этого языкового стандарта.</span><span class="sxs-lookup"><span data-stu-id="dbc3c-115">Each resource in this collection represents the localized value of the attribute name for a given language, used as the default label for that locale.</span></span> <span data-ttu-id="dbc3c-116">Например, пользователь с `no-NB` клиентом получает значение "Костнадс Sent" в качестве метки атрибута, а не "центр затрат".</span><span class="sxs-lookup"><span data-stu-id="dbc3c-116">For example, a user with a `no-NB` client gets "Kostnads Senter" as the attribute label, rather than "Cost Center."</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbc3c-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dbc3c-117">JSON representation</span></span>

<span data-ttu-id="dbc3c-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbc3c-118">The following is a JSON representation of the resource.</span></span>

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

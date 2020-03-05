---
title: Тип ресурса ЛангуажепрофиЦиенци
description: Тип ресурса ЛангуажепрофиЦиенци
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0934ea66c15e090a4f9ba9bcaa62a6c7eb900cd5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522997"
---
# <a name="languageproficiency-resource-type"></a><span data-ttu-id="ff4d5-103">Тип ресурса ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="ff4d5-103">languageProficiency resource type</span></span>

<span data-ttu-id="ff4d5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ff4d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff4d5-105">Представляет подробные сведения о языках, добавленных пользователем в свой [профиль](profile.md).</span><span class="sxs-lookup"><span data-stu-id="ff4d5-105">Represents detailed information about languages that a user has added to their [profile](profile.md).</span></span>

<span data-ttu-id="ff4d5-106">Наследуется от [итемфацет](itemFacet.md).</span><span class="sxs-lookup"><span data-stu-id="ff4d5-106">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ff4d5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ff4d5-107">Methods</span></span>

| <span data-ttu-id="ff4d5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ff4d5-108">Method</span></span>                                                       | <span data-ttu-id="ff4d5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ff4d5-109">Return Type</span></span>                                   | <span data-ttu-id="ff4d5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ff4d5-110">Description</span></span>                                                      | 
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="ff4d5-111">Получение ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="ff4d5-111">Get languageProficiency</span></span>](../api/languageproficiency-get.md) | [<span data-ttu-id="ff4d5-112">лангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="ff4d5-112">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="ff4d5-113">Чтение свойств и связей объекта **лангуажепрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="ff4d5-113">Read the properties and relationships of a **languageProficiency** object.</span></span> |
| [<span data-ttu-id="ff4d5-114">Обновление ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="ff4d5-114">Update languageProficiency</span></span>](../api/languageproficiency-update.md)               | [<span data-ttu-id="ff4d5-115">лангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="ff4d5-115">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="ff4d5-116">Обновление объекта **лангуажепрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="ff4d5-116">Update a **languageProficiency** object.</span></span>                               |
| [<span data-ttu-id="ff4d5-117">Удаление ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="ff4d5-117">Delete languageProficiency</span></span>](../api/languageproficiency-delete.md)               | <span data-ttu-id="ff4d5-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ff4d5-118">None</span></span>                                          | <span data-ttu-id="ff4d5-119">Удаление объекта **лангуажепрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="ff4d5-119">Delete a **languageProficiency** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="ff4d5-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff4d5-120">Properties</span></span>

| <span data-ttu-id="ff4d5-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff4d5-121">Property</span></span>     | <span data-ttu-id="ff4d5-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ff4d5-122">Type</span></span>        | <span data-ttu-id="ff4d5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ff4d5-123">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="ff4d5-124">displayName</span><span class="sxs-lookup"><span data-stu-id="ff4d5-124">displayName</span></span>   |<span data-ttu-id="ff4d5-125">String</span><span class="sxs-lookup"><span data-stu-id="ff4d5-125">String</span></span>       | <span data-ttu-id="ff4d5-126">Содержит имя языка в длинном формате.</span><span class="sxs-lookup"><span data-stu-id="ff4d5-126">Contains the long-form name for the language.</span></span>                                                                                                   |
|<span data-ttu-id="ff4d5-127">навыки</span><span class="sxs-lookup"><span data-stu-id="ff4d5-127">proficiency</span></span>   |<span data-ttu-id="ff4d5-128">строка</span><span class="sxs-lookup"><span data-stu-id="ff4d5-128">string</span></span>       | <span data-ttu-id="ff4d5-129">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ff4d5-129">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ff4d5-130">tag</span><span class="sxs-lookup"><span data-stu-id="ff4d5-130">tag</span></span>           |<span data-ttu-id="ff4d5-131">String</span><span class="sxs-lookup"><span data-stu-id="ff4d5-131">String</span></span>       | <span data-ttu-id="ff4d5-132">Содержит четырехзначный BCP47 Name для языка (EN-US, No-NetBIOS, en-AU).</span><span class="sxs-lookup"><span data-stu-id="ff4d5-132">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>                                                                                  |

## <a name="relationships"></a><span data-ttu-id="ff4d5-133">Связи</span><span class="sxs-lookup"><span data-stu-id="ff4d5-133">Relationships</span></span>

<span data-ttu-id="ff4d5-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ff4d5-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff4d5-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ff4d5-135">JSON representation</span></span>

<span data-ttu-id="ff4d5-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff4d5-136">The following is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.languageProficiency",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "proficiency": "string",
  "tag": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "languageProficiency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

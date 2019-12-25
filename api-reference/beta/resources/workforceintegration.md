---
title: Тип ресурса Воркфорцеинтегратион
description: Экземпляр интеграции сотрудников с сменами.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 631f2cc52b9327d77edd6fc5ad48292cf044570f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866492"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="fe5d5-103">Тип ресурса Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="fe5d5-103">workforceIntegration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe5d5-104">Экземпляр интеграции сотрудников с сменами.</span><span class="sxs-lookup"><span data-stu-id="fe5d5-104">An instance of a workforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="fe5d5-105">Методы</span><span class="sxs-lookup"><span data-stu-id="fe5d5-105">Methods</span></span>

| <span data-ttu-id="fe5d5-106">Метод</span><span class="sxs-lookup"><span data-stu-id="fe5d5-106">Method</span></span>       | <span data-ttu-id="fe5d5-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fe5d5-107">Return Type</span></span> | <span data-ttu-id="fe5d5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fe5d5-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fe5d5-109">[получение](../api/workforceintegration-get.md);</span><span class="sxs-lookup"><span data-stu-id="fe5d5-109">[Get](../api/workforceintegration-get.md)</span></span> | [<span data-ttu-id="fe5d5-110">воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="fe5d5-110">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="fe5d5-111">Чтение свойств и связей объекта **воркфорцеинтегратион** .</span><span class="sxs-lookup"><span data-stu-id="fe5d5-111">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| <span data-ttu-id="fe5d5-112">[обновление](../api/workforceintegration-update.md).</span><span class="sxs-lookup"><span data-stu-id="fe5d5-112">[Update](../api/workforceintegration-update.md)</span></span> | [<span data-ttu-id="fe5d5-113">воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="fe5d5-113">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="fe5d5-114">Обновление объекта **воркфорцеинтегратион** .</span><span class="sxs-lookup"><span data-stu-id="fe5d5-114">Update a **workforceIntegration** object.</span></span> |
| <span data-ttu-id="fe5d5-115">[удаление](../api/workforceintegration-delete.md);</span><span class="sxs-lookup"><span data-stu-id="fe5d5-115">[Delete](../api/workforceintegration-delete.md)</span></span> | <span data-ttu-id="fe5d5-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="fe5d5-116">None</span></span> | <span data-ttu-id="fe5d5-117">Удаление объекта **воркфорцеинтегратион** .</span><span class="sxs-lookup"><span data-stu-id="fe5d5-117">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fe5d5-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe5d5-118">Properties</span></span>

| <span data-ttu-id="fe5d5-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe5d5-119">Property</span></span>     | <span data-ttu-id="fe5d5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fe5d5-120">Type</span></span>        | <span data-ttu-id="fe5d5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fe5d5-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fe5d5-122">апиверсион</span><span class="sxs-lookup"><span data-stu-id="fe5d5-122">apiVersion</span></span>|<span data-ttu-id="fe5d5-123">Int32</span><span class="sxs-lookup"><span data-stu-id="fe5d5-123">Int32</span></span>|<span data-ttu-id="fe5d5-124">Версия API для URL-адреса обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="fe5d5-124">API version for the call back URL.</span></span> <span data-ttu-id="fe5d5-125">Начните с 1.</span><span class="sxs-lookup"><span data-stu-id="fe5d5-125">Start with 1.</span></span>|
|<span data-ttu-id="fe5d5-126">displayName</span><span class="sxs-lookup"><span data-stu-id="fe5d5-126">displayName</span></span>|<span data-ttu-id="fe5d5-127">String</span><span class="sxs-lookup"><span data-stu-id="fe5d5-127">String</span></span>|<span data-ttu-id="fe5d5-128">Имя интеграции трудовых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fe5d5-128">Name of the workforce integration.</span></span>|
|<span data-ttu-id="fe5d5-129">шифрования</span><span class="sxs-lookup"><span data-stu-id="fe5d5-129">encryption</span></span>|[<span data-ttu-id="fe5d5-130">воркфорцеинтегратионенкриптион</span><span class="sxs-lookup"><span data-stu-id="fe5d5-130">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="fe5d5-131">Ресурс для шифрования взаимодействия сотрудников.</span><span class="sxs-lookup"><span data-stu-id="fe5d5-131">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="fe5d5-132">isActive</span><span class="sxs-lookup"><span data-stu-id="fe5d5-132">isActive</span></span>|<span data-ttu-id="fe5d5-133">Логический</span><span class="sxs-lookup"><span data-stu-id="fe5d5-133">Boolean</span></span>|<span data-ttu-id="fe5d5-134">Указывает, активна ли эта интеграция сотрудников в настоящее время и доступна ли она.</span><span class="sxs-lookup"><span data-stu-id="fe5d5-134">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="fe5d5-135">имеется</span><span class="sxs-lookup"><span data-stu-id="fe5d5-135">supports</span></span>|<span data-ttu-id="fe5d5-136">string</span><span class="sxs-lookup"><span data-stu-id="fe5d5-136">string</span></span>| <span data-ttu-id="fe5d5-137">Возможные значения: `none`, `shift`, `swapRequest`, `openshift`,, `openShiftRequest``userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="fe5d5-137">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`</span></span>|
|<span data-ttu-id="fe5d5-138">url</span><span class="sxs-lookup"><span data-stu-id="fe5d5-138">url</span></span>|<span data-ttu-id="fe5d5-139">String</span><span class="sxs-lookup"><span data-stu-id="fe5d5-139">String</span></span>| <span data-ttu-id="fe5d5-140">URL-адрес интеграции сотрудников для обратных вызовов из службы смены.</span><span class="sxs-lookup"><span data-stu-id="fe5d5-140">Workforce Integration URL for callbacks from the shift service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe5d5-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="fe5d5-141">Relationships</span></span>

<span data-ttu-id="fe5d5-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fe5d5-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe5d5-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fe5d5-143">JSON representation</span></span>

<span data-ttu-id="fe5d5-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe5d5-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegration",
  "baseType": ""
}-->

```json
{
  "apiVersion": 1024,
  "displayName": "String",
  "encryption": {"@odata.type": "microsoft.graph.workforceIntegrationEncryption"},
  "isActive": true,
  "supports": "string",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

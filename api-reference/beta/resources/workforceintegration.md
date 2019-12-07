---
title: Тип ресурса Воркфорцеинтегратион
description: Экземпляр интеграции сотрудников с сменами.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa604c7d087d3231dd6ed1c6903a87f80298904b
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895842"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="90443-103">Тип ресурса Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="90443-103">workforceIntegration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90443-104">Экземпляр интеграции воркфорцефорце с сменами.</span><span class="sxs-lookup"><span data-stu-id="90443-104">An instance of a workforceforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="90443-105">Методы</span><span class="sxs-lookup"><span data-stu-id="90443-105">Methods</span></span>

| <span data-ttu-id="90443-106">Метод</span><span class="sxs-lookup"><span data-stu-id="90443-106">Method</span></span>       | <span data-ttu-id="90443-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="90443-107">Return Type</span></span> | <span data-ttu-id="90443-108">Описание</span><span class="sxs-lookup"><span data-stu-id="90443-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="90443-109">[получение](../api/workforceintegration-get.md);</span><span class="sxs-lookup"><span data-stu-id="90443-109">[Get](../api/workforceintegration-get.md)</span></span> | [<span data-ttu-id="90443-110">воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="90443-110">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="90443-111">Чтение свойств и связей объекта **воркфорцеинтегратион** .</span><span class="sxs-lookup"><span data-stu-id="90443-111">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| <span data-ttu-id="90443-112">[обновление](../api/workforceintegration-update.md).</span><span class="sxs-lookup"><span data-stu-id="90443-112">[Update](../api/workforceintegration-update.md)</span></span> | [<span data-ttu-id="90443-113">воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="90443-113">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="90443-114">Обновление объекта **воркфорцеинтегратион** .</span><span class="sxs-lookup"><span data-stu-id="90443-114">Update a **workforceIntegration** object.</span></span> |
| <span data-ttu-id="90443-115">[удаление](../api/workforceintegration-delete.md);</span><span class="sxs-lookup"><span data-stu-id="90443-115">[Delete](../api/workforceintegration-delete.md)</span></span> | <span data-ttu-id="90443-116">Нет</span><span class="sxs-lookup"><span data-stu-id="90443-116">None</span></span> | <span data-ttu-id="90443-117">Удаление объекта **воркфорцеинтегратион** .</span><span class="sxs-lookup"><span data-stu-id="90443-117">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="90443-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="90443-118">Properties</span></span>

| <span data-ttu-id="90443-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="90443-119">Property</span></span>     | <span data-ttu-id="90443-120">Тип</span><span class="sxs-lookup"><span data-stu-id="90443-120">Type</span></span>        | <span data-ttu-id="90443-121">Описание</span><span class="sxs-lookup"><span data-stu-id="90443-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90443-122">апиверсион</span><span class="sxs-lookup"><span data-stu-id="90443-122">apiVersion</span></span>|<span data-ttu-id="90443-123">Int32</span><span class="sxs-lookup"><span data-stu-id="90443-123">Int32</span></span>|<span data-ttu-id="90443-124">Версия API для URL-адреса обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="90443-124">API version for the call back URL.</span></span> <span data-ttu-id="90443-125">Начните с 1.</span><span class="sxs-lookup"><span data-stu-id="90443-125">Start with 1.</span></span>|
|<span data-ttu-id="90443-126">displayName</span><span class="sxs-lookup"><span data-stu-id="90443-126">displayName</span></span>|<span data-ttu-id="90443-127">String</span><span class="sxs-lookup"><span data-stu-id="90443-127">String</span></span>|<span data-ttu-id="90443-128">Имя интеграции трудовых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="90443-128">Name of the workforce integration.</span></span>|
|<span data-ttu-id="90443-129">шифрования</span><span class="sxs-lookup"><span data-stu-id="90443-129">encryption</span></span>|[<span data-ttu-id="90443-130">воркфорцеинтегратионенкриптион</span><span class="sxs-lookup"><span data-stu-id="90443-130">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="90443-131">Ресурс для шифрования взаимодействия сотрудников.</span><span class="sxs-lookup"><span data-stu-id="90443-131">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="90443-132">isActive</span><span class="sxs-lookup"><span data-stu-id="90443-132">isActive</span></span>|<span data-ttu-id="90443-133">Логический</span><span class="sxs-lookup"><span data-stu-id="90443-133">Boolean</span></span>|<span data-ttu-id="90443-134">Указывает, активна ли эта интеграция сотрудников в настоящее время и доступна ли она.</span><span class="sxs-lookup"><span data-stu-id="90443-134">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="90443-135">имеется</span><span class="sxs-lookup"><span data-stu-id="90443-135">supports</span></span>|<span data-ttu-id="90443-136">string</span><span class="sxs-lookup"><span data-stu-id="90443-136">string</span></span>| <span data-ttu-id="90443-137">Возможные значения: `none`, `shift`, `swapRequest`, `openshift`,, `openShiftRequest``userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="90443-137">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`</span></span>|
|<span data-ttu-id="90443-138">url</span><span class="sxs-lookup"><span data-stu-id="90443-138">url</span></span>|<span data-ttu-id="90443-139">String</span><span class="sxs-lookup"><span data-stu-id="90443-139">String</span></span>| <span data-ttu-id="90443-140">URL-адрес интеграции сотрудников для обратных вызовов из службы смены.</span><span class="sxs-lookup"><span data-stu-id="90443-140">Workforce Integration URL for callbacks from the shift service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90443-141">Связи</span><span class="sxs-lookup"><span data-stu-id="90443-141">Relationships</span></span>

<span data-ttu-id="90443-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="90443-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="90443-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="90443-143">JSON representation</span></span>

<span data-ttu-id="90443-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90443-144">The following is a JSON representation of the resource.</span></span>

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

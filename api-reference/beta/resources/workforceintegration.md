---
title: Тип ресурса Воркфорцеинтегратион
description: Экземпляр интеграции сотрудников с сменами.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1e836a4346fe5e31f39c1f6383acbf78530ae9e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519087"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="75774-103">Тип ресурса Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="75774-103">workforceIntegration resource type</span></span>

<span data-ttu-id="75774-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75774-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75774-105">Экземпляр интеграции сотрудников с сменами.</span><span class="sxs-lookup"><span data-stu-id="75774-105">An instance of a workforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="75774-106">Методы</span><span class="sxs-lookup"><span data-stu-id="75774-106">Methods</span></span>

| <span data-ttu-id="75774-107">Метод</span><span class="sxs-lookup"><span data-stu-id="75774-107">Method</span></span>       | <span data-ttu-id="75774-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="75774-108">Return Type</span></span> | <span data-ttu-id="75774-109">Описание</span><span class="sxs-lookup"><span data-stu-id="75774-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="75774-110">[получение](../api/workforceintegration-get.md);</span><span class="sxs-lookup"><span data-stu-id="75774-110">[Get](../api/workforceintegration-get.md)</span></span> | [<span data-ttu-id="75774-111">воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="75774-111">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="75774-112">Чтение свойств и связей объекта **воркфорцеинтегратион** .</span><span class="sxs-lookup"><span data-stu-id="75774-112">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| <span data-ttu-id="75774-113">[обновление](../api/workforceintegration-update.md).</span><span class="sxs-lookup"><span data-stu-id="75774-113">[Update](../api/workforceintegration-update.md)</span></span> | [<span data-ttu-id="75774-114">воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="75774-114">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="75774-115">Обновление объекта **воркфорцеинтегратион** .</span><span class="sxs-lookup"><span data-stu-id="75774-115">Update a **workforceIntegration** object.</span></span> |
| <span data-ttu-id="75774-116">[удаление](../api/workforceintegration-delete.md);</span><span class="sxs-lookup"><span data-stu-id="75774-116">[Delete](../api/workforceintegration-delete.md)</span></span> | <span data-ttu-id="75774-117">Нет</span><span class="sxs-lookup"><span data-stu-id="75774-117">None</span></span> | <span data-ttu-id="75774-118">Удаление объекта **воркфорцеинтегратион** .</span><span class="sxs-lookup"><span data-stu-id="75774-118">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="75774-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="75774-119">Properties</span></span>

| <span data-ttu-id="75774-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="75774-120">Property</span></span>     | <span data-ttu-id="75774-121">Тип</span><span class="sxs-lookup"><span data-stu-id="75774-121">Type</span></span>        | <span data-ttu-id="75774-122">Описание</span><span class="sxs-lookup"><span data-stu-id="75774-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="75774-123">апиверсион</span><span class="sxs-lookup"><span data-stu-id="75774-123">apiVersion</span></span>|<span data-ttu-id="75774-124">Int32</span><span class="sxs-lookup"><span data-stu-id="75774-124">Int32</span></span>|<span data-ttu-id="75774-125">Версия API для URL-адреса обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="75774-125">API version for the call back URL.</span></span> <span data-ttu-id="75774-126">Начните с 1.</span><span class="sxs-lookup"><span data-stu-id="75774-126">Start with 1.</span></span>|
|<span data-ttu-id="75774-127">displayName</span><span class="sxs-lookup"><span data-stu-id="75774-127">displayName</span></span>|<span data-ttu-id="75774-128">String</span><span class="sxs-lookup"><span data-stu-id="75774-128">String</span></span>|<span data-ttu-id="75774-129">Имя интеграции трудовых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="75774-129">Name of the workforce integration.</span></span>|
|<span data-ttu-id="75774-130">шифрования</span><span class="sxs-lookup"><span data-stu-id="75774-130">encryption</span></span>|[<span data-ttu-id="75774-131">воркфорцеинтегратионенкриптион</span><span class="sxs-lookup"><span data-stu-id="75774-131">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="75774-132">Ресурс для шифрования взаимодействия сотрудников.</span><span class="sxs-lookup"><span data-stu-id="75774-132">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="75774-133">isActive</span><span class="sxs-lookup"><span data-stu-id="75774-133">isActive</span></span>|<span data-ttu-id="75774-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="75774-134">Boolean</span></span>|<span data-ttu-id="75774-135">Указывает, активна ли эта интеграция сотрудников в настоящее время и доступна ли она.</span><span class="sxs-lookup"><span data-stu-id="75774-135">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="75774-136">имеется</span><span class="sxs-lookup"><span data-stu-id="75774-136">supports</span></span>|<span data-ttu-id="75774-137">string</span><span class="sxs-lookup"><span data-stu-id="75774-137">string</span></span>| <span data-ttu-id="75774-138">Возможные значения: `none`, `shift`, `swapRequest`, `openshift`,, `openShiftRequest``userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="75774-138">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`</span></span>|
|<span data-ttu-id="75774-139">url</span><span class="sxs-lookup"><span data-stu-id="75774-139">url</span></span>|<span data-ttu-id="75774-140">String</span><span class="sxs-lookup"><span data-stu-id="75774-140">String</span></span>| <span data-ttu-id="75774-141">URL-адрес интеграции сотрудников для обратных вызовов из службы смены.</span><span class="sxs-lookup"><span data-stu-id="75774-141">Workforce Integration URL for callbacks from the shift service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75774-142">Связи</span><span class="sxs-lookup"><span data-stu-id="75774-142">Relationships</span></span>

<span data-ttu-id="75774-143">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="75774-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="75774-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="75774-144">JSON representation</span></span>

<span data-ttu-id="75774-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75774-145">The following is a JSON representation of the resource.</span></span>

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

---
title: тип ресурса membershipRuleProcessingStatus
description: Представляет текущее состояние динамической групповой обработки.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 7c86f044517ad7b808db69364413727c8d76f076
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680999"
---
# <a name="membershipruleprocessingstatus-resource-type"></a><span data-ttu-id="e3c13-103">тип ресурса membershipRuleProcessingStatus</span><span class="sxs-lookup"><span data-stu-id="e3c13-103">membershipRuleProcessingStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3c13-104">Представляет текущее состояние динамической групповой обработки.</span><span class="sxs-lookup"><span data-stu-id="e3c13-104">Represents the current status of dynamic group processing.</span></span>

## <a name="properties"></a><span data-ttu-id="e3c13-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3c13-105">Properties</span></span>

| <span data-ttu-id="e3c13-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3c13-106">Property</span></span> | <span data-ttu-id="e3c13-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e3c13-107">Type</span></span> | <span data-ttu-id="e3c13-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e3c13-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="e3c13-109">status</span><span class="sxs-lookup"><span data-stu-id="e3c13-109">status</span></span> | [<span data-ttu-id="e3c13-110">membershipRuleProcessingStatusDetails</span><span class="sxs-lookup"><span data-stu-id="e3c13-110">membershipRuleProcessingStatusDetails</span></span>](#membershipruleprocessingstatusdetails-values) | <span data-ttu-id="e3c13-111">Текущее состояние динамической групповой обработки.</span><span class="sxs-lookup"><span data-stu-id="e3c13-111">Current status of a dynamic group processing.</span></span> <span data-ttu-id="e3c13-112">Возможные значения: `NotStarted` `Running` , , , , `Succeeded` и `Failed` `UnknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="e3c13-112">Possible values are: `NotStarted`, `Running`, `Succeeded`, `Failed`, and `UnknownFutureValue`.</span></span>  <br><br> <span data-ttu-id="e3c13-113">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="e3c13-113">Required.</span></span> <span data-ttu-id="e3c13-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3c13-114">Read-only.</span></span>|
| <span data-ttu-id="e3c13-115">lastMembershipUpdated</span><span class="sxs-lookup"><span data-stu-id="e3c13-115">lastMembershipUpdated</span></span> | <span data-ttu-id="e3c13-116">edm. DateTime</span><span class="sxs-lookup"><span data-stu-id="e3c13-116">edm.DateTime</span></span> | <span data-ttu-id="e3c13-117">Последние даты и время обновления членства в динамической группе.</span><span class="sxs-lookup"><span data-stu-id="e3c13-117">Most recent date and time when membership of a dynamic group was updated.</span></span> <br><br> <span data-ttu-id="e3c13-118">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e3c13-118">Optional.</span></span> <span data-ttu-id="e3c13-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3c13-119">Read-only.</span></span>|
| <span data-ttu-id="e3c13-120">errorMessage</span><span class="sxs-lookup"><span data-stu-id="e3c13-120">errorMessage</span></span> | <span data-ttu-id="e3c13-121">String</span><span class="sxs-lookup"><span data-stu-id="e3c13-121">String</span></span> | <span data-ttu-id="e3c13-122">Подробное сообщение об ошибке, если динамическая обработка группы столкнулась с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="e3c13-122">Detailed error message if dynamic group processing ran into an error.</span></span> <br><br> <span data-ttu-id="e3c13-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e3c13-123">Optional.</span></span> <span data-ttu-id="e3c13-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3c13-124">Read-only.</span></span>|

### <a name="membershipruleprocessingstatusdetails-values"></a><span data-ttu-id="e3c13-125">значения membershipRuleProcessingStatusDetails</span><span class="sxs-lookup"><span data-stu-id="e3c13-125">membershipRuleProcessingStatusDetails values</span></span>

| <span data-ttu-id="e3c13-126">Member</span><span class="sxs-lookup"><span data-stu-id="e3c13-126">Member</span></span> | <span data-ttu-id="e3c13-127">Описание</span><span class="sxs-lookup"><span data-stu-id="e3c13-127">Description</span></span> |
|:-------- |:----------- |
| <span data-ttu-id="e3c13-128">NotStarted</span><span class="sxs-lookup"><span data-stu-id="e3c13-128">NotStarted</span></span> | <span data-ttu-id="e3c13-129">Группа была создана или обновлена и ожидает обработки.</span><span class="sxs-lookup"><span data-stu-id="e3c13-129">Group has been created or updated, and awaiting processing.</span></span>|
| <span data-ttu-id="e3c13-130">Работает</span><span class="sxs-lookup"><span data-stu-id="e3c13-130">Running</span></span> | <span data-ttu-id="e3c13-131">Началась обработка.</span><span class="sxs-lookup"><span data-stu-id="e3c13-131">Processing has started.</span></span>|
| <span data-ttu-id="e3c13-132">Succeeded</span><span class="sxs-lookup"><span data-stu-id="e3c13-132">Succeeded</span></span> | <span data-ttu-id="e3c13-133">Обработка завершена.</span><span class="sxs-lookup"><span data-stu-id="e3c13-133">Processing has completed.</span></span> <span data-ttu-id="e3c13-134">Инкрементные изменения объектов обрабатываются постоянно.</span><span class="sxs-lookup"><span data-stu-id="e3c13-134">Incremental object changes are processed perpetually.</span></span> |
| <span data-ttu-id="e3c13-135">Ошибка</span><span class="sxs-lookup"><span data-stu-id="e3c13-135">Failed</span></span> | <span data-ttu-id="e3c13-136">Обработка столкнулась с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="e3c13-136">Processing ran into an error.</span></span> <span data-ttu-id="e3c13-137">Подробные сведения см. в **странице errorMessage.**</span><span class="sxs-lookup"><span data-stu-id="e3c13-137">See **errorMessage** for details.</span></span> |
| <span data-ttu-id="e3c13-138">UnknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="e3c13-138">UnknownFutureValue</span></span> | <span data-ttu-id="e3c13-139">Поддерживает будущие значения.</span><span class="sxs-lookup"><span data-stu-id="e3c13-139">Supports future values.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e3c13-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3c13-140">JSON representation</span></span>

<span data-ttu-id="e3c13-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3c13-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.membershipRuleProcessingStatus",
  "baseType": null
}-->

```json
{
  "status": "string",
  "lastMembershipUpdated": "DateTime",
  "errorMessage": "string"
}
```

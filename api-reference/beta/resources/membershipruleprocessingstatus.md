---
title: Тип ресурса membershipRuleProcessingStatus
description: Представляет текущее состояние динамической обработки группы.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 864cbd9ea446655c2a0d5f950b28fa6421d2241c
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784890"
---
# <a name="membershipruleprocessingstatus-resource-type"></a><span data-ttu-id="6bbb3-103">Тип ресурса membershipRuleProcessingStatus</span><span class="sxs-lookup"><span data-stu-id="6bbb3-103">membershipRuleProcessingStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bbb3-104">Представляет текущее состояние динамической обработки группы.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-104">Represents the current status of dynamic group processing.</span></span>

## <a name="properties"></a><span data-ttu-id="6bbb3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6bbb3-105">Properties</span></span>

| <span data-ttu-id="6bbb3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bbb3-106">Property</span></span> | <span data-ttu-id="6bbb3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6bbb3-107">Type</span></span> | <span data-ttu-id="6bbb3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6bbb3-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="6bbb3-109">status</span><span class="sxs-lookup"><span data-stu-id="6bbb3-109">status</span></span> | [<span data-ttu-id="6bbb3-110">membershipRuleProcessingStatusDetails</span><span class="sxs-lookup"><span data-stu-id="6bbb3-110">membershipRuleProcessingStatusDetails</span></span>](#membershipruleprocessingstatusdetails-values) | <span data-ttu-id="6bbb3-111">Текущее состояние динамической обработки группы.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-111">Current status of a dynamic group processing.</span></span> <span data-ttu-id="6bbb3-112">Возможные значения: `NotStarted` , , , , и `Running` `Succeeded` `Failed` `UnknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="6bbb3-112">Possible values are: `NotStarted`, `Running`, `Succeeded`, `Failed`, and `UnknownFutureValue`.</span></span>  <br><br> <span data-ttu-id="6bbb3-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-113">Required.</span></span> <span data-ttu-id="6bbb3-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-114">Read-only.</span></span>|
| <span data-ttu-id="6bbb3-115">lastMembershipUpdated</span><span class="sxs-lookup"><span data-stu-id="6bbb3-115">lastMembershipUpdated</span></span> | <span data-ttu-id="6bbb3-116">edm. DateTime</span><span class="sxs-lookup"><span data-stu-id="6bbb3-116">edm.DateTime</span></span> | <span data-ttu-id="6bbb3-117">Самая новая дата и время обновления членства в динамической группе.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-117">Most recent date and time when membership of a dynamic group was updated.</span></span> <br><br> <span data-ttu-id="6bbb3-118">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-118">Optional.</span></span> <span data-ttu-id="6bbb3-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-119">Read-only.</span></span>|
| <span data-ttu-id="6bbb3-120">errorMessage</span><span class="sxs-lookup"><span data-stu-id="6bbb3-120">errorMessage</span></span> | <span data-ttu-id="6bbb3-121">String</span><span class="sxs-lookup"><span data-stu-id="6bbb3-121">String</span></span> | <span data-ttu-id="6bbb3-122">Подробное сообщение об ошибке, если динамическая обработка группы столкнулась с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-122">Detailed error message if dynamic group processing ran into an error.</span></span> <br><br> <span data-ttu-id="6bbb3-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-123">Optional.</span></span> <span data-ttu-id="6bbb3-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-124">Read-only.</span></span>|

### <a name="membershipruleprocessingstatusdetails-values"></a><span data-ttu-id="6bbb3-125">значения membershipRuleProcessingStatusDetails</span><span class="sxs-lookup"><span data-stu-id="6bbb3-125">membershipRuleProcessingStatusDetails values</span></span>

| <span data-ttu-id="6bbb3-126">Member</span><span class="sxs-lookup"><span data-stu-id="6bbb3-126">Member</span></span> | <span data-ttu-id="6bbb3-127">Описание</span><span class="sxs-lookup"><span data-stu-id="6bbb3-127">Description</span></span> |
|:-------- |:----------- |
| <span data-ttu-id="6bbb3-128">NotStarted</span><span class="sxs-lookup"><span data-stu-id="6bbb3-128">NotStarted</span></span> | <span data-ttu-id="6bbb3-129">Группа создана или обновлена и ожидает обработки.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-129">Group has been created or updated, and awaiting processing.</span></span>|
| <span data-ttu-id="6bbb3-130">Выполняется</span><span class="sxs-lookup"><span data-stu-id="6bbb3-130">Running</span></span> | <span data-ttu-id="6bbb3-131">Обработка запущена.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-131">Processing has started.</span></span>|
| <span data-ttu-id="6bbb3-132">Succeeded</span><span class="sxs-lookup"><span data-stu-id="6bbb3-132">Succeeded</span></span> | <span data-ttu-id="6bbb3-133">Обработка завершена.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-133">Processing has completed.</span></span> <span data-ttu-id="6bbb3-134">Добавочные изменения объектов обрабатываются бессрочно.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-134">Incremental object changes are processed perpetually.</span></span> |
| <span data-ttu-id="6bbb3-135">Не выполнено</span><span class="sxs-lookup"><span data-stu-id="6bbb3-135">Failed</span></span> | <span data-ttu-id="6bbb3-136">При обработке произошла ошибка.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-136">Processing ran into an error.</span></span> <span data-ttu-id="6bbb3-137">Подробные **сведения см. в errorMessage.**</span><span class="sxs-lookup"><span data-stu-id="6bbb3-137">See **errorMessage** for details.</span></span> |
| <span data-ttu-id="6bbb3-138">UnknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="6bbb3-138">UnknownFutureValue</span></span> | <span data-ttu-id="6bbb3-139">Поддерживает будущие значения.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-139">Supports future values.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6bbb3-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6bbb3-140">JSON representation</span></span>

<span data-ttu-id="6bbb3-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-141">The following is a JSON representation of the resource.</span></span>

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

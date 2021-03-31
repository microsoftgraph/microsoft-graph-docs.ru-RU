---
title: Тип ресурса approvalStage
description: Объект approvalStage, связанный с userConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d6212553d9364c4352bf1d6796156a4020854bf1
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469624"
---
# <a name="approvalstage-resource-type"></a><span data-ttu-id="04bd5-103">Тип ресурса approvalStage</span><span class="sxs-lookup"><span data-stu-id="04bd5-103">approvalStage resource type</span></span>

<span data-ttu-id="04bd5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04bd5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="04bd5-105">Указывает этапы принятия решений в утверждении.</span><span class="sxs-lookup"><span data-stu-id="04bd5-105">Specifies decision stages in the approval.</span></span>

## <a name="properties"></a><span data-ttu-id="04bd5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="04bd5-106">Properties</span></span>

|<span data-ttu-id="04bd5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="04bd5-107">Property</span></span>|<span data-ttu-id="04bd5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="04bd5-108">Type</span></span>|<span data-ttu-id="04bd5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="04bd5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04bd5-110">assignedToMe</span><span class="sxs-lookup"><span data-stu-id="04bd5-110">assignedToMe</span></span>|<span data-ttu-id="04bd5-111">Логический</span><span class="sxs-lookup"><span data-stu-id="04bd5-111">Boolean</span></span>|<span data-ttu-id="04bd5-112">Указывает, назначен ли этап пользователю вызова для проверки.</span><span class="sxs-lookup"><span data-stu-id="04bd5-112">Indicates whether the stage is assigned to the calling user to review.</span></span> <span data-ttu-id="04bd5-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04bd5-113">Read-only.</span></span>|
|<span data-ttu-id="04bd5-114">displayName</span><span class="sxs-lookup"><span data-stu-id="04bd5-114">displayName</span></span>|<span data-ttu-id="04bd5-115">String</span><span class="sxs-lookup"><span data-stu-id="04bd5-115">String</span></span>|<span data-ttu-id="04bd5-116">Метка, предоставленная создателем политики для определения стадии утверждения.</span><span class="sxs-lookup"><span data-stu-id="04bd5-116">The label provided by the policy creator to identify an approval stage.</span></span> <span data-ttu-id="04bd5-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04bd5-117">Read-only.</span></span>|
|<span data-ttu-id="04bd5-118">id</span><span class="sxs-lookup"><span data-stu-id="04bd5-118">id</span></span>|<span data-ttu-id="04bd5-119">String</span><span class="sxs-lookup"><span data-stu-id="04bd5-119">String</span></span>|<span data-ttu-id="04bd5-120">Идентификатор стадии, связанной с объектом утверждения.</span><span class="sxs-lookup"><span data-stu-id="04bd5-120">The identifier of the stage associated with an approval object.</span></span> <span data-ttu-id="04bd5-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04bd5-121">Read-only.</span></span>|
|<span data-ttu-id="04bd5-122">обоснование</span><span class="sxs-lookup"><span data-stu-id="04bd5-122">justification</span></span>|<span data-ttu-id="04bd5-123">String</span><span class="sxs-lookup"><span data-stu-id="04bd5-123">String</span></span>|<span data-ttu-id="04bd5-124">Обоснование, связанное с решением стадии утверждения.</span><span class="sxs-lookup"><span data-stu-id="04bd5-124">The justification associated with the approval stage decision.</span></span>|
|<span data-ttu-id="04bd5-125">reviewResult</span><span class="sxs-lookup"><span data-stu-id="04bd5-125">reviewResult</span></span>|<span data-ttu-id="04bd5-126">String</span><span class="sxs-lookup"><span data-stu-id="04bd5-126">String</span></span>|<span data-ttu-id="04bd5-127">Результат этой записи утверждения.</span><span class="sxs-lookup"><span data-stu-id="04bd5-127">The result of this approval record.</span></span> <span data-ttu-id="04bd5-128">Возможные значения: `NotReviewed` , `Approved` , `Denied` .</span><span class="sxs-lookup"><span data-stu-id="04bd5-128">Possible values include: `NotReviewed`, `Approved`, `Denied`.</span></span>|
|<span data-ttu-id="04bd5-129">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="04bd5-129">reviewedBy</span></span>|[<span data-ttu-id="04bd5-130">userIdentity</span><span class="sxs-lookup"><span data-stu-id="04bd5-130">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="04bd5-131">Идентификатор рецензента.</span><span class="sxs-lookup"><span data-stu-id="04bd5-131">The identifier of the reviewer.</span></span> <span data-ttu-id="04bd5-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04bd5-132">Read-only.</span></span>|
|<span data-ttu-id="04bd5-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="04bd5-133">reviewedDateTime</span></span>|<span data-ttu-id="04bd5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04bd5-134">DateTimeOffset</span></span>|<span data-ttu-id="04bd5-135">Дата и время записи решения.</span><span class="sxs-lookup"><span data-stu-id="04bd5-135">The date and time when a decision was recorded.</span></span> <span data-ttu-id="04bd5-136">Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="04bd5-136">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="04bd5-137">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="04bd5-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="04bd5-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04bd5-138">Read-only.</span></span>|
|<span data-ttu-id="04bd5-139">status</span><span class="sxs-lookup"><span data-stu-id="04bd5-139">status</span></span>|<span data-ttu-id="04bd5-140">String</span><span class="sxs-lookup"><span data-stu-id="04bd5-140">String</span></span>|<span data-ttu-id="04bd5-141">Состояние сцены.</span><span class="sxs-lookup"><span data-stu-id="04bd5-141">The stage status.</span></span> <span data-ttu-id="04bd5-142">Возможные значения: `InProgress` `Initializing` , , `Completed` `Expired` .</span><span class="sxs-lookup"><span data-stu-id="04bd5-142">Possible values: `InProgress`, `Initializing`, `Completed`, `Expired`.</span></span> <span data-ttu-id="04bd5-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04bd5-143">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04bd5-144">Связи</span><span class="sxs-lookup"><span data-stu-id="04bd5-144">Relationships</span></span>

<span data-ttu-id="04bd5-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="04bd5-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04bd5-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="04bd5-146">JSON representation</span></span>

<span data-ttu-id="04bd5-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04bd5-147">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approvalStage",
  "id": "String (identifier)",
  "displayName": "String",
  "status": "String",
  "assignedToMe": "Boolean",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.identity"
  },
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String"
}
```

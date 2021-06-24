---
title: тип ресурса serviceHealthIssue
description: Представляет проблему со здоровьем службы в службе.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 2436e6d0d5e49155b936cbfb7f7fc98630b7ce57
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109232"
---
# <a name="servicehealthissue-resource-type"></a><span data-ttu-id="aa263-103">тип ресурса serviceHealthIssue</span><span class="sxs-lookup"><span data-stu-id="aa263-103">serviceHealthIssue resource type</span></span>

<span data-ttu-id="aa263-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa263-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa263-105">Представляет проблему со здоровьем службы в службе.</span><span class="sxs-lookup"><span data-stu-id="aa263-105">Represents a service health issue in a service.</span></span>

<span data-ttu-id="aa263-106">Проблема со здоровьем службы может быть инцидентом службы или консультацией по обслуживанию.</span><span class="sxs-lookup"><span data-stu-id="aa263-106">The service health issue can be a service incident or service advisory.</span></span> <span data-ttu-id="aa263-107">Например:</span><span class="sxs-lookup"><span data-stu-id="aa263-107">For example:</span></span>

* <span data-ttu-id="aa263-108">Инцидент службы: "Exchange службы почтовых ящиков не существует".</span><span class="sxs-lookup"><span data-stu-id="aa263-108">Service incident: "Exchange mailbox service is down".</span></span>
* <span data-ttu-id="aa263-109">Рекомендации по обслуживанию: "Пользователи могут испытывать задержки в приеме сообщений электронной почты".</span><span class="sxs-lookup"><span data-stu-id="aa263-109">Service advisory: "Users may experience delays in emails reception".</span></span>

<span data-ttu-id="aa263-110">Наследует от [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="aa263-110">Inherits from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="aa263-111">Методы</span><span class="sxs-lookup"><span data-stu-id="aa263-111">Methods</span></span>
|<span data-ttu-id="aa263-112">Метод</span><span class="sxs-lookup"><span data-stu-id="aa263-112">Method</span></span>|<span data-ttu-id="aa263-113">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="aa263-113">Return type</span></span>|<span data-ttu-id="aa263-114">Описание</span><span class="sxs-lookup"><span data-stu-id="aa263-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa263-115">Get serviceHealthIssue</span><span class="sxs-lookup"><span data-stu-id="aa263-115">Get serviceHealthIssue</span></span>](../api/servicehealthissue-get.md)|[<span data-ttu-id="aa263-116">serviceHealthIssue</span><span class="sxs-lookup"><span data-stu-id="aa263-116">serviceHealthIssue</span></span>](../resources/servicehealthissue.md)|<span data-ttu-id="aa263-117">Извлечение свойств и связей объекта [serviceHealthIssue.](../resources/servicehealthissue.md)</span><span class="sxs-lookup"><span data-stu-id="aa263-117">Retrieve the properties and relationships of a [serviceHealthIssue](../resources/servicehealthissue.md) object.</span></span> |
|[<span data-ttu-id="aa263-118">Получить отчет о проверке после инцидента</span><span class="sxs-lookup"><span data-stu-id="aa263-118">Get post-incident review report</span></span>](../api/servicehealthissue-incidentreport.md)|<span data-ttu-id="aa263-119">Stream</span><span class="sxs-lookup"><span data-stu-id="aa263-119">Stream</span></span>|<span data-ttu-id="aa263-120">Предоставляет отчет о происшествии после публикации (PIR) для указанной проблемы службы для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa263-120">Provides the post incident report (PIR) document of a specified service issue for tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="aa263-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa263-121">Properties</span></span>
|<span data-ttu-id="aa263-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa263-122">Property</span></span>|<span data-ttu-id="aa263-123">Тип</span><span class="sxs-lookup"><span data-stu-id="aa263-123">Type</span></span>|<span data-ttu-id="aa263-124">Описание</span><span class="sxs-lookup"><span data-stu-id="aa263-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa263-125">classification</span><span class="sxs-lookup"><span data-stu-id="aa263-125">classification</span></span>|<span data-ttu-id="aa263-126">serviceHealthClassificationType</span><span class="sxs-lookup"><span data-stu-id="aa263-126">serviceHealthClassificationType</span></span>|<span data-ttu-id="aa263-127">Тип проблемы со здоровьем службы.</span><span class="sxs-lookup"><span data-stu-id="aa263-127">The type of service health issue.</span></span> <span data-ttu-id="aa263-128">Возможные значения: `advisory`, `incident`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="aa263-128">Possible values are: `advisory`, `incident`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="aa263-129">подробности</span><span class="sxs-lookup"><span data-stu-id="aa263-129">details</span></span>|<span data-ttu-id="aa263-130">[Коллекция(keyValuePair)](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="aa263-130">Collection([keyValuePair](../resources/keyvaluepair.md))</span></span>|<span data-ttu-id="aa263-131">Дополнительные сведения о проблеме со здоровьем службы.</span><span class="sxs-lookup"><span data-stu-id="aa263-131">Additional details about service health issue.</span></span> <span data-ttu-id="aa263-132">Это свойство не поддерживает фильтры.</span><span class="sxs-lookup"><span data-stu-id="aa263-132">This property doesn't support filters.</span></span> <span data-ttu-id="aa263-133">Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="aa263-133">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="aa263-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="aa263-134">endDateTime</span></span>|<span data-ttu-id="aa263-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa263-135">DateTimeOffset</span></span>|<span data-ttu-id="aa263-136">Время окончания проблемы службы.</span><span class="sxs-lookup"><span data-stu-id="aa263-136">The end time of the service issue.</span></span> <span data-ttu-id="aa263-137">Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="aa263-137">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="aa263-138">функция</span><span class="sxs-lookup"><span data-stu-id="aa263-138">feature</span></span>|<span data-ttu-id="aa263-139">Строка</span><span class="sxs-lookup"><span data-stu-id="aa263-139">String</span></span>|<span data-ttu-id="aa263-140">Имя функции проблемы службы.</span><span class="sxs-lookup"><span data-stu-id="aa263-140">The feature name of the service issue.</span></span>|
|<span data-ttu-id="aa263-141">featureGroup</span><span class="sxs-lookup"><span data-stu-id="aa263-141">featureGroup</span></span>|<span data-ttu-id="aa263-142">Строка</span><span class="sxs-lookup"><span data-stu-id="aa263-142">String</span></span>|<span data-ttu-id="aa263-143">Имя группы функций проблемы службы.</span><span class="sxs-lookup"><span data-stu-id="aa263-143">The feature group name of the service issue.</span></span>|
|<span data-ttu-id="aa263-144">id</span><span class="sxs-lookup"><span data-stu-id="aa263-144">id</span></span>|<span data-ttu-id="aa263-145">Строка</span><span class="sxs-lookup"><span data-stu-id="aa263-145">String</span></span>|<span data-ttu-id="aa263-146">Id проблемы службы.</span><span class="sxs-lookup"><span data-stu-id="aa263-146">The id of the service issue.</span></span> <span data-ttu-id="aa263-147">Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="aa263-147">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="aa263-148">impactDescription</span><span class="sxs-lookup"><span data-stu-id="aa263-148">impactDescription</span></span>|<span data-ttu-id="aa263-149">Строка</span><span class="sxs-lookup"><span data-stu-id="aa263-149">String</span></span>|<span data-ttu-id="aa263-150">Описание влияния проблемы службы.</span><span class="sxs-lookup"><span data-stu-id="aa263-150">The description of the service issue impact.</span></span>|
|<span data-ttu-id="aa263-151">isResolved</span><span class="sxs-lookup"><span data-stu-id="aa263-151">isResolved</span></span>|<span data-ttu-id="aa263-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa263-152">Boolean</span></span>|<span data-ttu-id="aa263-153">Указывает, устранена ли проблема.</span><span class="sxs-lookup"><span data-stu-id="aa263-153">Indicates whether the issue is resolved.</span></span>|
|<span data-ttu-id="aa263-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa263-154">lastModifiedDateTime</span></span>|<span data-ttu-id="aa263-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa263-155">DateTimeOffset</span></span>|<span data-ttu-id="aa263-156">Последнее измененное время проблемы.</span><span class="sxs-lookup"><span data-stu-id="aa263-156">The last modified time of the issue.</span></span> <span data-ttu-id="aa263-157">Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="aa263-157">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="aa263-158">происхождение</span><span class="sxs-lookup"><span data-stu-id="aa263-158">origin</span></span>|<span data-ttu-id="aa263-159">serviceHealthOrigin</span><span class="sxs-lookup"><span data-stu-id="aa263-159">serviceHealthOrigin</span></span>|<span data-ttu-id="aa263-160">Указывает происхождение проблемы службы.</span><span class="sxs-lookup"><span data-stu-id="aa263-160">Indicates the origin of the service issue.</span></span> <span data-ttu-id="aa263-161">Возможные значения: `microsoft`, `thirdParty`, `customer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="aa263-161">Possible values are: `microsoft`, `thirdParty`, `customer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="aa263-162">posts</span><span class="sxs-lookup"><span data-stu-id="aa263-162">posts</span></span>|<span data-ttu-id="aa263-163">[Collection(serviceHealthIssuePost)](../resources/servicehealthissuepost.md)</span><span class="sxs-lookup"><span data-stu-id="aa263-163">Collection([serviceHealthIssuePost](../resources/servicehealthissuepost.md))</span></span>|<span data-ttu-id="aa263-164">Коллекция исторических сообщений для проблемы службы.</span><span class="sxs-lookup"><span data-stu-id="aa263-164">Collection of historical posts for the service issue.</span></span>|
|<span data-ttu-id="aa263-165">service</span><span class="sxs-lookup"><span data-stu-id="aa263-165">service</span></span>|<span data-ttu-id="aa263-166">String</span><span class="sxs-lookup"><span data-stu-id="aa263-166">String</span></span>|<span data-ttu-id="aa263-167">Указывает службу, затрагиваемую проблемой.</span><span class="sxs-lookup"><span data-stu-id="aa263-167">Indicates the service affected by the issue.</span></span>|
|<span data-ttu-id="aa263-168">startDateTime</span><span class="sxs-lookup"><span data-stu-id="aa263-168">startDateTime</span></span>|<span data-ttu-id="aa263-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa263-169">DateTimeOffset</span></span>|<span data-ttu-id="aa263-170">Время начала выпуска службы.</span><span class="sxs-lookup"><span data-stu-id="aa263-170">The start time of the service issue.</span></span> <span data-ttu-id="aa263-171">Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="aa263-171">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="aa263-172">status</span><span class="sxs-lookup"><span data-stu-id="aa263-172">status</span></span>|<span data-ttu-id="aa263-173">serviceHealthStatus</span><span class="sxs-lookup"><span data-stu-id="aa263-173">serviceHealthStatus</span></span>|<span data-ttu-id="aa263-174">Состояние проблемы службы.</span><span class="sxs-lookup"><span data-stu-id="aa263-174">The status of the service issue.</span></span> <span data-ttu-id="aa263-175">Возможные значения: `serviceOperational` `investigating` , , , , `restoringService` , `verifyingService` , `serviceRestored` `postIncidentReviewPublished` `serviceDegradation` , `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` `reported` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="aa263-175">Possible values are: `serviceOperational`, `investigating`, `restoringService`, `verifyingService`, `serviceRestored`, `postIncidentReviewPublished`, `serviceDegradation`, `serviceInterruption`, `extendedRecovery`, `falsePositive`, `investigationSuspended`, `resolved`, `mitigatedExternal`, `mitigated`, `resolvedExternal`, `confirmed`, `reported`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="aa263-176">title</span><span class="sxs-lookup"><span data-stu-id="aa263-176">title</span></span>|<span data-ttu-id="aa263-177">Строка</span><span class="sxs-lookup"><span data-stu-id="aa263-177">String</span></span>|<span data-ttu-id="aa263-178">Название проблемы службы.</span><span class="sxs-lookup"><span data-stu-id="aa263-178">The title of the service issue.</span></span> <span data-ttu-id="aa263-179">Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="aa263-179">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa263-180">Отношения</span><span class="sxs-lookup"><span data-stu-id="aa263-180">Relationships</span></span>
<span data-ttu-id="aa263-181">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aa263-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa263-182">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aa263-182">JSON representation</span></span>
<span data-ttu-id="aa263-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa263-183">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceHealthIssue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealthIssue",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "id": "String (identifier)",
  "impactDescription": "String",
  "classification": "String",
  "origin": "String",
  "posts": [
    {
      "@odata.type": "microsoft.graph.serviceHealthIssuePost"
    }
  ],
  "status": "String",
  "service": "String",
  "feature": "String",
  "featureGroup": "String",
  "isResolved": "Boolean"
}
```


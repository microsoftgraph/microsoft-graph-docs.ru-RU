---
title: тип ресурса securityAction
description: Принимайте незамедлительные действия по защите от угроз с помощью объекта securityAction Microsoft Graph Security. Если аналитик безопасности обнаруживает новый индикатор, например вредоносный файл, URL-адрес, домен или IP-адрес, можно сразу же включить защиту в решении по обеспечению безопасности от корпорации Майкрософт. Вызывайте действие для определенного поставщика услуг, просматривайте все выполненные действия и отменяйте действие при необходимости. Воспользуйтесь действиями по обеспечению безопасности с помощью ATP в Защитнике Windows (ожидается в ближайшее время), чтобы заблокировать вредоносную активность в конечных точках Windows с использованием свойств, отображаемых в оповещениях или выявленных при изучении.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c1adeb6ee5ab3b3ad2165e854b2812e39b8df5ab
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720636"
---
# <a name="securityaction-resource-type"></a><span data-ttu-id="e583c-106">тип ресурса securityAction</span><span class="sxs-lookup"><span data-stu-id="e583c-106">securityAction resource type</span></span>

<span data-ttu-id="e583c-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e583c-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e583c-108">Принимайте незамедлительные действия по защите от угроз с помощью объекта securityAction Microsoft Graph Security.</span><span class="sxs-lookup"><span data-stu-id="e583c-108">Take immediate action to defend against threats using the Microsoft Graph Security securityAction entity.</span></span> <span data-ttu-id="e583c-109">Если аналитик безопасности обнаруживает новый индикатор, например вредоносный файл, URL-адрес, домен или IP-адрес, можно сразу же включить защиту в решении по обеспечению безопасности от корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e583c-109">When a security analyst discovers a new indicator, such as a malicious file, URL, domain, or IP address, protection can be instantly enabled in your Microsoft security solutions.</span></span> <span data-ttu-id="e583c-110">Вызывайте действие для определенного поставщика услуг, просматривайте все выполненные действия и отменяйте действие при необходимости.</span><span class="sxs-lookup"><span data-stu-id="e583c-110">Invoke an action for a specific provider, see all actions taken, and cancel an action if needed.</span></span> <span data-ttu-id="e583c-111">Воспользуйтесь действиями по обеспечению безопасности с помощью [ATP в Защитнике Windows](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection), чтобы заблокировать вредоносную активность в конечных точках Windows с использованием свойств, отображаемых в оповещениях или выявленных при изучении.</span><span class="sxs-lookup"><span data-stu-id="e583c-111">Try security actions with [Windows Defender ATP](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) to block malicious activity on your Windows endpoints using properties seen in alerts or identified during investigations.</span></span>

  > <span data-ttu-id="e583c-112">**Примечание.** В настоящее время действия по обеспечению безопасности поддерживают только разрешения для приложений.</span><span class="sxs-lookup"><span data-stu-id="e583c-112">**Note:** Currently security actions only support application permissions.</span></span>

## <a name="methods"></a><span data-ttu-id="e583c-113">Методы</span><span class="sxs-lookup"><span data-stu-id="e583c-113">Methods</span></span>

| <span data-ttu-id="e583c-114">Метод</span><span class="sxs-lookup"><span data-stu-id="e583c-114">Method</span></span>       | <span data-ttu-id="e583c-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e583c-115">Return Type</span></span> | <span data-ttu-id="e583c-116">Описание</span><span class="sxs-lookup"><span data-stu-id="e583c-116">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e583c-117">Получение действия по обеспечению безопасности</span><span class="sxs-lookup"><span data-stu-id="e583c-117">Get security action</span></span>](../api/securityaction-get.md) | [<span data-ttu-id="e583c-118">securityAction</span><span class="sxs-lookup"><span data-stu-id="e583c-118">securityAction</span></span>](securityaction.md) | <span data-ttu-id="e583c-119">Чтение свойств и связей объекта securityAction.</span><span class="sxs-lookup"><span data-stu-id="e583c-119">Read properties and relationships of securityAction object.</span></span> |
| [<span data-ttu-id="e583c-120">Создание действия по обеспечению безопасности</span><span class="sxs-lookup"><span data-stu-id="e583c-120">Create security action</span></span>](../api/securityactions-post.md) | [<span data-ttu-id="e583c-121">securityAction</span><span class="sxs-lookup"><span data-stu-id="e583c-121">securityAction</span></span>](securityaction.md) | <span data-ttu-id="e583c-122">Создайте новую службу безопасности, разместив ее в коллекции securityActions.</span><span class="sxs-lookup"><span data-stu-id="e583c-122">Create a new securityAction by posting to the securityActions collection.</span></span> |
| [<span data-ttu-id="e583c-123">Перечисление действий по обеспечению безопасности</span><span class="sxs-lookup"><span data-stu-id="e583c-123">List security actions</span></span>](../api/securityactions-list.md) | <span data-ttu-id="e583c-124">[коллекция securityAction](securityaction.md)</span><span class="sxs-lookup"><span data-stu-id="e583c-124">[securityAction](securityaction.md) collection</span></span> | <span data-ttu-id="e583c-125">Получите коллекцию объектов securityAction.</span><span class="sxs-lookup"><span data-stu-id="e583c-125">Get a securityAction object collection.</span></span> |
|[<span data-ttu-id="e583c-126">Отмена действия по обеспечению безопасности</span><span class="sxs-lookup"><span data-stu-id="e583c-126">Cancel security action</span></span>](../api/securityaction-cancelsecurityaction.md)|<span data-ttu-id="e583c-127">Нет</span><span class="sxs-lookup"><span data-stu-id="e583c-127">None</span></span>|<span data-ttu-id="e583c-128">Отмена операции безопасности.</span><span class="sxs-lookup"><span data-stu-id="e583c-128">Cancel a security operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="e583c-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="e583c-129">Properties</span></span>

| <span data-ttu-id="e583c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e583c-130">Property</span></span>     | <span data-ttu-id="e583c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e583c-131">Type</span></span>        | <span data-ttu-id="e583c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e583c-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e583c-133">actionReason</span><span class="sxs-lookup"><span data-stu-id="e583c-133">actionReason</span></span>|<span data-ttu-id="e583c-134">String</span><span class="sxs-lookup"><span data-stu-id="e583c-134">String</span></span>|<span data-ttu-id="e583c-135">Причина для этого действия.</span><span class="sxs-lookup"><span data-stu-id="e583c-135">Reason for invoking this action.</span></span>|
|<span data-ttu-id="e583c-136">appId</span><span class="sxs-lookup"><span data-stu-id="e583c-136">appId</span></span>|<span data-ttu-id="e583c-137">String</span><span class="sxs-lookup"><span data-stu-id="e583c-137">String</span></span>|<span data-ttu-id="e583c-138">ID приложения вызываемого приложения, которое представило (POST) действие.</span><span class="sxs-lookup"><span data-stu-id="e583c-138">The Application ID of the calling application that submitted (POST) the action.</span></span> <span data-ttu-id="e583c-139">AppId должен быть извлечен из маркера auth и не вошел вручную в вызываемом приложении.</span><span class="sxs-lookup"><span data-stu-id="e583c-139">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="e583c-140">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="e583c-140">azureTenantId</span></span>|<span data-ttu-id="e583c-141">String</span><span class="sxs-lookup"><span data-stu-id="e583c-141">String</span></span>|<span data-ttu-id="e583c-142">ID клиента Azure для субъекта, чтобы определить, к какову клиенту принадлежит объект (поддержка с несколькими арендами).</span><span class="sxs-lookup"><span data-stu-id="e583c-142">Azure tenant ID of the entity to determine which tenant the entity belongs to (multi-tenancy support).</span></span> <span data-ttu-id="e583c-143">AzureTenantId должен быть извлечен из маркера auth и не вошел вручную с помощью вызываемого приложения.</span><span class="sxs-lookup"><span data-stu-id="e583c-143">The azureTenantId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="e583c-144">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="e583c-144">completedDateTime</span></span>|<span data-ttu-id="e583c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e583c-145">DateTimeOffset</span></span>|<span data-ttu-id="e583c-146">Timestamp, когда действие было завершено.</span><span class="sxs-lookup"><span data-stu-id="e583c-146">Timestamp when the action was completed.</span></span> <span data-ttu-id="e583c-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e583c-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e583c-148">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e583c-148">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e583c-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e583c-149">createdDateTime</span></span>|<span data-ttu-id="e583c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e583c-150">DateTimeOffset</span></span>|<span data-ttu-id="e583c-151">Timestamp, когда действие создано.</span><span class="sxs-lookup"><span data-stu-id="e583c-151">Timestamp when the action is created.</span></span> <span data-ttu-id="e583c-152">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e583c-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e583c-153">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e583c-153">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e583c-154">errorInfo</span><span class="sxs-lookup"><span data-stu-id="e583c-154">errorInfo</span></span>|[<span data-ttu-id="e583c-155">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e583c-155">resultInfo</span></span>](resultinfo.md)| <span data-ttu-id="e583c-156">Сведения об ошибках при сбойе действия.</span><span class="sxs-lookup"><span data-stu-id="e583c-156">Error info when the action fails.</span></span>|
|<span data-ttu-id="e583c-157">id</span><span class="sxs-lookup"><span data-stu-id="e583c-157">id</span></span>|<span data-ttu-id="e583c-158">String</span><span class="sxs-lookup"><span data-stu-id="e583c-158">String</span></span>| <span data-ttu-id="e583c-159">Создается системой при прохо-</span><span class="sxs-lookup"><span data-stu-id="e583c-159">Created by the system when the action is ingested.</span></span> <span data-ttu-id="e583c-160">Созданный GUID/уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="e583c-160">Generated GUID/unique identifier.</span></span> <span data-ttu-id="e583c-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e583c-161">Read-only.</span></span>|
|<span data-ttu-id="e583c-162">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="e583c-162">lastActionDateTime</span></span>|<span data-ttu-id="e583c-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e583c-163">DateTimeOffset</span></span>| <span data-ttu-id="e583c-164">Timestamp при последнем обновлении этого действия.</span><span class="sxs-lookup"><span data-stu-id="e583c-164">Timestamp when this action was last updated.</span></span> <span data-ttu-id="e583c-165">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e583c-165">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e583c-166">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e583c-166">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e583c-167">name</span><span class="sxs-lookup"><span data-stu-id="e583c-167">name</span></span>|<span data-ttu-id="e583c-168">String</span><span class="sxs-lookup"><span data-stu-id="e583c-168">String</span></span>| <span data-ttu-id="e583c-169">Имя действия.</span><span class="sxs-lookup"><span data-stu-id="e583c-169">Action name.</span></span>|
|<span data-ttu-id="e583c-170">parameters</span><span class="sxs-lookup"><span data-stu-id="e583c-170">parameters</span></span>|<span data-ttu-id="e583c-171">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e583c-171">[keyValuePair](keyvaluepair.md) collection</span></span>| <span data-ttu-id="e583c-172">Набор параметров (пары значений ключа), необходимых для вызова действия, например URL-адреса или fileHash для блокировки и т.д.).</span><span class="sxs-lookup"><span data-stu-id="e583c-172">Collection of parameters (key-value pairs) necessary to invoke the action, e.g. URL or fileHash to block, etc.).</span></span> <span data-ttu-id="e583c-173">**Required**</span><span class="sxs-lookup"><span data-stu-id="e583c-173">**Required**</span></span>|
|<span data-ttu-id="e583c-174">состояния</span><span class="sxs-lookup"><span data-stu-id="e583c-174">states</span></span>|<span data-ttu-id="e583c-175">[коллекция securityActionState](securityactionstate.md)</span><span class="sxs-lookup"><span data-stu-id="e583c-175">[securityActionState](securityactionstate.md) collection</span></span>|<span data-ttu-id="e583c-176">Коллекция securityActionState для сохраняемой истории действия.</span><span class="sxs-lookup"><span data-stu-id="e583c-176">Collection of securityActionState to keep the history of an action.</span></span>|
|<span data-ttu-id="e583c-177">status</span><span class="sxs-lookup"><span data-stu-id="e583c-177">status</span></span>|<span data-ttu-id="e583c-178">string</span><span class="sxs-lookup"><span data-stu-id="e583c-178">string</span></span>| <span data-ttu-id="e583c-179">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="e583c-179">Status of the action.</span></span> <span data-ttu-id="e583c-180">Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="e583c-180">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="e583c-181">user</span><span class="sxs-lookup"><span data-stu-id="e583c-181">user</span></span>|<span data-ttu-id="e583c-182">String</span><span class="sxs-lookup"><span data-stu-id="e583c-182">String</span></span>| <span data-ttu-id="e583c-183">Основное имя пользователя пользователя, который отправил (POST) действие.</span><span class="sxs-lookup"><span data-stu-id="e583c-183">The user principal name of the signed-in user that submitted  (POST) the action.</span></span> <span data-ttu-id="e583c-184">Пользователь должен быть извлечен из маркера auth и не вошел вручную с помощью вызываемого приложения.</span><span class="sxs-lookup"><span data-stu-id="e583c-184">The user should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="e583c-185">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="e583c-185">vendorInformation</span></span>|[<span data-ttu-id="e583c-186">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="e583c-186">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="e583c-187">Сложный тип, содержащий сведения о поставщике продукта и службы безопасности, поставщике и суб-поставщике (например, поставщик=Microsoft; provider=Защитник Windows ATP; sub-provider=AppLocker).</span><span class="sxs-lookup"><span data-stu-id="e583c-187">Complex Type containing details about the Security product/service vendor, provider, and sub-provider (e.g. vendor=Microsoft; provider=Windows Defender ATP; sub-provider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e583c-188">Связи</span><span class="sxs-lookup"><span data-stu-id="e583c-188">Relationships</span></span>

<span data-ttu-id="e583c-189">Нет</span><span class="sxs-lookup"><span data-stu-id="e583c-189">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e583c-190">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e583c-190">JSON representation</span></span>

<span data-ttu-id="e583c-191">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e583c-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
  "keyProperty": "id"
}-->

```json
{
  "actionReason": "String",
  "appId": "String",
  "azureTenantId": "String",
  "clientContext": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "errorInfo": {"@odata.type": "microsoft.graph.resultInfo"},
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "states": [{"@odata.type": "microsoft.graph.securityActionState"}],
  "status": "string",
  "user": "String",
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
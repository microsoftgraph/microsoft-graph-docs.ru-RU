---
title: Тип ресурса securityAction
description: Принимайте незамедлительные действия по защите от угроз с помощью объекта securityAction Microsoft Graph Security. Если аналитик безопасности обнаруживает новый индикатор, например вредоносный файл, URL-адрес, домен или IP-адрес, можно сразу же включить защиту в решении по обеспечению безопасности от корпорации Майкрософт. Вызывайте действие для определенного поставщика услуг, просматривайте все выполненные действия и отменяйте действие при необходимости. Воспользуйтесь действиями по обеспечению безопасности с помощью ATP в Защитнике Windows (ожидается в ближайшее время), чтобы заблокировать вредоносную активность в конечных точках Windows с использованием свойств, отображаемых в оповещениях или выявленных при изучении.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 48c00d99ade3601e051d074272793d6aa0f2c66b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520831"
---
# <a name="securityaction-resource-type"></a><span data-ttu-id="b1b6c-106">Тип ресурса securityAction</span><span class="sxs-lookup"><span data-stu-id="b1b6c-106">securityAction resource type</span></span>

<span data-ttu-id="b1b6c-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1b6c-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1b6c-108">Принимайте незамедлительные действия по защите от угроз с помощью объекта securityAction Microsoft Graph Security.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-108">Take immediate action to defend against threats using the Microsoft Graph Security securityAction entity.</span></span> <span data-ttu-id="b1b6c-109">Если аналитик безопасности обнаруживает новый индикатор, например вредоносный файл, URL-адрес, домен или IP-адрес, можно сразу же включить защиту в решении по обеспечению безопасности от корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-109">When a security analyst discovers a new indicator, such as a malicious file, URL, domain, or IP address, protection can be instantly enabled in your Microsoft security solutions.</span></span> <span data-ttu-id="b1b6c-110">Вызывайте действие для определенного поставщика услуг, просматривайте все выполненные действия и отменяйте действие при необходимости.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-110">Invoke an action for a specific provider, see all actions taken, and cancel an action if needed.</span></span> <span data-ttu-id="b1b6c-111">Воспользуйтесь действиями по обеспечению безопасности с помощью [ATP в Защитнике Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection), чтобы заблокировать вредоносную активность в конечных точках Windows с использованием свойств, отображаемых в оповещениях или выявленных при изучении.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-111">Try security actions with [Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) to block malicious activity on your Windows endpoints using properties seen in alerts or identified during investigations.</span></span>

  > <span data-ttu-id="b1b6c-112">**Примечание.** В настоящее время действия по обеспечению безопасности поддерживают только разрешения для приложений.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-112">**Note:** Currently security actions only support application permissions.</span></span>

## <a name="methods"></a><span data-ttu-id="b1b6c-113">Методы</span><span class="sxs-lookup"><span data-stu-id="b1b6c-113">Methods</span></span>

| <span data-ttu-id="b1b6c-114">Метод</span><span class="sxs-lookup"><span data-stu-id="b1b6c-114">Method</span></span>       | <span data-ttu-id="b1b6c-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b1b6c-115">Return Type</span></span> | <span data-ttu-id="b1b6c-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b1b6c-116">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b1b6c-117">Получение действия по обеспечению безопасности</span><span class="sxs-lookup"><span data-stu-id="b1b6c-117">Get security action</span></span>](../api/securityaction-get.md) | [<span data-ttu-id="b1b6c-118">securityAction</span><span class="sxs-lookup"><span data-stu-id="b1b6c-118">securityAction</span></span>](securityaction.md) | <span data-ttu-id="b1b6c-119">Чтение свойств и связей объекта securityAction.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-119">Read properties and relationships of securityAction object.</span></span> |
| [<span data-ttu-id="b1b6c-120">Создание действия по обеспечению безопасности</span><span class="sxs-lookup"><span data-stu-id="b1b6c-120">Create security action</span></span>](../api/securityactions-post.md) | [<span data-ttu-id="b1b6c-121">securityAction</span><span class="sxs-lookup"><span data-stu-id="b1b6c-121">securityAction</span></span>](securityaction.md) | <span data-ttu-id="b1b6c-122">Создание нового securityAction путем отправки в коллекцию Секуритяктионс.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-122">Create a new securityAction by posting to the securityActions collection.</span></span> |
| [<span data-ttu-id="b1b6c-123">Перечисление действий по обеспечению безопасности</span><span class="sxs-lookup"><span data-stu-id="b1b6c-123">List security actions</span></span>](../api/securityactions-list.md) | <span data-ttu-id="b1b6c-124">Коллекция [securityAction](securityaction.md)</span><span class="sxs-lookup"><span data-stu-id="b1b6c-124">[securityAction](securityaction.md) collection</span></span> | <span data-ttu-id="b1b6c-125">Получение коллекции объектов securityAction.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-125">Get a securityAction object collection.</span></span> |
|[<span data-ttu-id="b1b6c-126">Отмена действия по обеспечению безопасности</span><span class="sxs-lookup"><span data-stu-id="b1b6c-126">Cancel security action</span></span>](../api/securityaction-cancelsecurityaction.md)|<span data-ttu-id="b1b6c-127">Нет</span><span class="sxs-lookup"><span data-stu-id="b1b6c-127">None</span></span>|<span data-ttu-id="b1b6c-128">Отмена операции безопасности.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-128">Cancel a security operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1b6c-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1b6c-129">Properties</span></span>

| <span data-ttu-id="b1b6c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1b6c-130">Property</span></span>     | <span data-ttu-id="b1b6c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b1b6c-131">Type</span></span>        | <span data-ttu-id="b1b6c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b1b6c-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1b6c-133">актионреасон</span><span class="sxs-lookup"><span data-stu-id="b1b6c-133">actionReason</span></span>|<span data-ttu-id="b1b6c-134">String</span><span class="sxs-lookup"><span data-stu-id="b1b6c-134">String</span></span>|<span data-ttu-id="b1b6c-135">Причина для вызова этого действия.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-135">Reason for invoking this action.</span></span>|
|<span data-ttu-id="b1b6c-136">appId</span><span class="sxs-lookup"><span data-stu-id="b1b6c-136">appId</span></span>|<span data-ttu-id="b1b6c-137">String</span><span class="sxs-lookup"><span data-stu-id="b1b6c-137">String</span></span>|<span data-ttu-id="b1b6c-138">Идентификатор приложения, который передал действие (POST).</span><span class="sxs-lookup"><span data-stu-id="b1b6c-138">The Application ID of the calling application that submitted (POST) the action.</span></span> <span data-ttu-id="b1b6c-139">AppId необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-139">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="b1b6c-140">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="b1b6c-140">azureTenantId</span></span>|<span data-ttu-id="b1b6c-141">String</span><span class="sxs-lookup"><span data-stu-id="b1b6c-141">String</span></span>|<span data-ttu-id="b1b6c-142">Идентификатор клиента Azure объекта, который определяет, к какому клиенту относится данная сущность (поддержка с поддержкой нескольких клиентов).</span><span class="sxs-lookup"><span data-stu-id="b1b6c-142">Azure tenant ID of the entity to determine which tenant the entity belongs to (multi-tenancy support).</span></span> <span data-ttu-id="b1b6c-143">Азуретенантид необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-143">The azureTenantId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="b1b6c-144">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1b6c-144">completedDateTime</span></span>|<span data-ttu-id="b1b6c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1b6c-145">DateTimeOffset</span></span>|<span data-ttu-id="b1b6c-146">Временная метка выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-146">Timestamp when the action was completed.</span></span> <span data-ttu-id="b1b6c-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b1b6c-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b1b6c-148">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-148">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b1b6c-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1b6c-149">createdDateTime</span></span>|<span data-ttu-id="b1b6c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1b6c-150">DateTimeOffset</span></span>|<span data-ttu-id="b1b6c-151">Временная метка при создании действия.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-151">Timestamp when the action is created.</span></span> <span data-ttu-id="b1b6c-152">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b1b6c-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b1b6c-153">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b1b6c-154">errorInfo</span><span class="sxs-lookup"><span data-stu-id="b1b6c-154">errorInfo</span></span>|[<span data-ttu-id="b1b6c-155">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b1b6c-155">resultInfo</span></span>](resultinfo.md)| <span data-ttu-id="b1b6c-156">Сведения об ошибке при сбое действия.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-156">Error info when the action fails.</span></span>|
|<span data-ttu-id="b1b6c-157">id</span><span class="sxs-lookup"><span data-stu-id="b1b6c-157">id</span></span>|<span data-ttu-id="b1b6c-158">Строка</span><span class="sxs-lookup"><span data-stu-id="b1b6c-158">String</span></span>| <span data-ttu-id="b1b6c-159">Создается системой при выполнении действия.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-159">Created by the system when the action is ingested.</span></span> <span data-ttu-id="b1b6c-160">Созданный GUID/уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-160">Generated GUID/unique identifier.</span></span> <span data-ttu-id="b1b6c-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-161">Read-only.</span></span>|
|<span data-ttu-id="b1b6c-162">ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="b1b6c-162">lastActionDateTime</span></span>|<span data-ttu-id="b1b6c-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1b6c-163">DateTimeOffset</span></span>| <span data-ttu-id="b1b6c-164">Временная метка при последнем обновлении этого действия.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-164">Timestamp when this action was last updated.</span></span> <span data-ttu-id="b1b6c-165">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b1b6c-165">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b1b6c-166">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-166">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b1b6c-167">name</span><span class="sxs-lookup"><span data-stu-id="b1b6c-167">name</span></span>|<span data-ttu-id="b1b6c-168">Строка</span><span class="sxs-lookup"><span data-stu-id="b1b6c-168">String</span></span>| <span data-ttu-id="b1b6c-169">Имя действия.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-169">Action name.</span></span>|
|<span data-ttu-id="b1b6c-170">parameters</span><span class="sxs-lookup"><span data-stu-id="b1b6c-170">parameters</span></span>|<span data-ttu-id="b1b6c-171">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b1b6c-171">[keyValuePair](keyvaluepair.md) collection</span></span>| <span data-ttu-id="b1b6c-172">Коллекция параметров (пар "ключ-значение"), необходимых для вызова действия, например URL-адрес или fileHash для блокировки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="b1b6c-172">Collection of parameters (key-value pairs) necessary to invoke the action, e.g. URL or fileHash to block, etc.).</span></span> <span data-ttu-id="b1b6c-173">**Required**</span><span class="sxs-lookup"><span data-stu-id="b1b6c-173">**Required**</span></span>|
|<span data-ttu-id="b1b6c-174">состояния</span><span class="sxs-lookup"><span data-stu-id="b1b6c-174">states</span></span>|<span data-ttu-id="b1b6c-175">Коллекция [секуритяктионстате](securityactionstate.md)</span><span class="sxs-lookup"><span data-stu-id="b1b6c-175">[securityActionState](securityactionstate.md) collection</span></span>|<span data-ttu-id="b1b6c-176">Коллекция Секуритяктионстате, в которой будет храниться журнал действия.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-176">Collection of securityActionState to keep the history of an action.</span></span>|
|<span data-ttu-id="b1b6c-177">status</span><span class="sxs-lookup"><span data-stu-id="b1b6c-177">status</span></span>|<span data-ttu-id="b1b6c-178">string</span><span class="sxs-lookup"><span data-stu-id="b1b6c-178">string</span></span>| <span data-ttu-id="b1b6c-179">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-179">Status of the action.</span></span> <span data-ttu-id="b1b6c-180">Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-180">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="b1b6c-181">user</span><span class="sxs-lookup"><span data-stu-id="b1b6c-181">user</span></span>|<span data-ttu-id="b1b6c-182">String</span><span class="sxs-lookup"><span data-stu-id="b1b6c-182">String</span></span>| <span data-ttu-id="b1b6c-183">Имя участника-пользователя, который выполнил вход в действие (POST).</span><span class="sxs-lookup"><span data-stu-id="b1b6c-183">The user principal name of the signed-in user that submitted  (POST) the action.</span></span> <span data-ttu-id="b1b6c-184">Пользователь должен быть извлечен из маркера проверки подлинности и не был введен вручную вызывающим приложением вручную.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-184">The user should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="b1b6c-185">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="b1b6c-185">vendorInformation</span></span>|[<span data-ttu-id="b1b6c-186">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="b1b6c-186">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="b1b6c-187">Сложный тип, содержащий сведения о продуктах, поставщиках и подчиненных поставщиках системы безопасности (например, Vendor = Microsoft; Provider = защитник Windows ATP; подчиненный поставщик = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="b1b6c-187">Complex Type containing details about the Security product/service vendor, provider, and sub-provider (e.g. vendor=Microsoft; provider=Windows Defender ATP; sub-provider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1b6c-188">Связи</span><span class="sxs-lookup"><span data-stu-id="b1b6c-188">Relationships</span></span>

<span data-ttu-id="b1b6c-189">Нет</span><span class="sxs-lookup"><span data-stu-id="b1b6c-189">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1b6c-190">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1b6c-190">JSON representation</span></span>

<span data-ttu-id="b1b6c-191">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1b6c-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
  "baseType": "",
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
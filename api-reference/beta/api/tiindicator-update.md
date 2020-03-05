---
title: Обновление объекта tiIndicator
description: Обновление свойств объекта Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 0db1441030dc75d60dcbb1bd3d3eab2b09a5aad4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452346"
---
# <a name="update-tiindicator"></a><span data-ttu-id="3be7c-103">Обновление объекта tiIndicator</span><span class="sxs-lookup"><span data-stu-id="3be7c-103">Update tiIndicator</span></span>

<span data-ttu-id="3be7c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3be7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3be7c-105">Обновление свойств объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="3be7c-105">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3be7c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3be7c-106">Permissions</span></span>

<span data-ttu-id="3be7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3be7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3be7c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3be7c-109">Permission type</span></span>                        | <span data-ttu-id="3be7c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3be7c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3be7c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3be7c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3be7c-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="3be7c-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="3be7c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3be7c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3be7c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3be7c-114">Not supported.</span></span> |
| <span data-ttu-id="3be7c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3be7c-115">Application</span></span>                            | <span data-ttu-id="3be7c-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="3be7c-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="3be7c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3be7c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3be7c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3be7c-118">Request headers</span></span>

| <span data-ttu-id="3be7c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3be7c-119">Name</span></span>       | <span data-ttu-id="3be7c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3be7c-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3be7c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3be7c-121">Authorization</span></span> | <span data-ttu-id="3be7c-122">**Необходим** носитель {код}</span><span class="sxs-lookup"><span data-stu-id="3be7c-122">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="3be7c-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="3be7c-123">Prefer</span></span> | <span data-ttu-id="3be7c-124">Возврат = представление</span><span class="sxs-lookup"><span data-stu-id="3be7c-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="3be7c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3be7c-125">Request body</span></span>

<span data-ttu-id="3be7c-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3be7c-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3be7c-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="3be7c-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3be7c-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3be7c-128">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="3be7c-129">Обязательные поля: `id`, `expirationDateTime`, `targetProduct`.</span><span class="sxs-lookup"><span data-stu-id="3be7c-129">Required fields are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="3be7c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3be7c-130">Property</span></span>     | <span data-ttu-id="3be7c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3be7c-131">Type</span></span>        | <span data-ttu-id="3be7c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3be7c-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3be7c-133">action</span><span class="sxs-lookup"><span data-stu-id="3be7c-133">action</span></span>|<span data-ttu-id="3be7c-134">строка</span><span class="sxs-lookup"><span data-stu-id="3be7c-134">string</span></span>| <span data-ttu-id="3be7c-135">Действие, которое необходимо применить, если индикатор сопоставлен с помощью средства безопасности Таржетпродукт.</span><span class="sxs-lookup"><span data-stu-id="3be7c-135">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="3be7c-136">Возможные значения: `unknown`, `allow`, `block`, `alert`.</span><span class="sxs-lookup"><span data-stu-id="3be7c-136">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="3be7c-137">активитиграупнамес</span><span class="sxs-lookup"><span data-stu-id="3be7c-137">activityGroupNames</span></span>|<span data-ttu-id="3be7c-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3be7c-138">String collection</span></span>|<span data-ttu-id="3be7c-139">Имя (-ы) логики операций с угрозами кибератак для сторон, ответственных за вредоносные действия, охваченные индикатором угроз.</span><span class="sxs-lookup"><span data-stu-id="3be7c-139">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="3be7c-140">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="3be7c-140">additionalInformation</span></span>|<span data-ttu-id="3be7c-141">String</span><span class="sxs-lookup"><span data-stu-id="3be7c-141">String</span></span>|<span data-ttu-id="3be7c-142">Область общего пользования, в которую могут быть размещены дополнительные данные из индикатора, не охваченные другими свойствами Тииндикатор.</span><span class="sxs-lookup"><span data-stu-id="3be7c-142">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="3be7c-143">Данные, помещаемые в Аддитионалинформатион, обычно не используются средством безопасности Таржетпродукт.</span><span class="sxs-lookup"><span data-stu-id="3be7c-143">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="3be7c-144">confidence</span><span class="sxs-lookup"><span data-stu-id="3be7c-144">confidence</span></span>|<span data-ttu-id="3be7c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3be7c-145">Int32</span></span>|<span data-ttu-id="3be7c-146">Целое число, представляющее достоверность, с помощью которой данные в индикаторе точно определяют вредоносное поведение.</span><span class="sxs-lookup"><span data-stu-id="3be7c-146">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="3be7c-147">Допустимые значения: 0 – 100 с 100 по убыванию.</span><span class="sxs-lookup"><span data-stu-id="3be7c-147">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="3be7c-148">description</span><span class="sxs-lookup"><span data-stu-id="3be7c-148">description</span></span>|<span data-ttu-id="3be7c-149">String</span><span class="sxs-lookup"><span data-stu-id="3be7c-149">String</span></span>|<span data-ttu-id="3be7c-150">Краткое описание угрозы, представленное индикатором (100 символов или меньше).</span><span class="sxs-lookup"><span data-stu-id="3be7c-150">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="3be7c-151">диамондмодел</span><span class="sxs-lookup"><span data-stu-id="3be7c-151">diamondModel</span></span>|[<span data-ttu-id="3be7c-152">диамондмодел</span><span class="sxs-lookup"><span data-stu-id="3be7c-152">diamondModel</span></span>](#diamondmodel-values)|<span data-ttu-id="3be7c-153">Область модели ромба, в которой существует этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="3be7c-153">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="3be7c-154">Возможные значения: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span><span class="sxs-lookup"><span data-stu-id="3be7c-154">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="3be7c-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3be7c-155">expirationDateTime</span></span>|<span data-ttu-id="3be7c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3be7c-156">DateTimeOffset</span></span>| <span data-ttu-id="3be7c-157">Строка DateTime, указывающая, когда истечет срок действия индикатора.</span><span class="sxs-lookup"><span data-stu-id="3be7c-157">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="3be7c-158">Все индикаторы должны иметь дату истечения срока действия, чтобы не допустить устаревших показателей в системе.</span><span class="sxs-lookup"><span data-stu-id="3be7c-158">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="3be7c-159">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3be7c-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3be7c-160">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="3be7c-160">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="3be7c-161">externalId</span><span class="sxs-lookup"><span data-stu-id="3be7c-161">externalId</span></span>|<span data-ttu-id="3be7c-162">String</span><span class="sxs-lookup"><span data-stu-id="3be7c-162">String</span></span>|<span data-ttu-id="3be7c-163">Идентификационный номер, который привязывает индикатор к системе поставщика индикаторов (например, внешнему ключу).</span><span class="sxs-lookup"><span data-stu-id="3be7c-163">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="3be7c-164">isActive</span><span class="sxs-lookup"><span data-stu-id="3be7c-164">isActive</span></span>|<span data-ttu-id="3be7c-165">Логический</span><span class="sxs-lookup"><span data-stu-id="3be7c-165">Boolean</span></span>|<span data-ttu-id="3be7c-166">Используется для отключения индикаторов в системе.</span><span class="sxs-lookup"><span data-stu-id="3be7c-166">Used to deactivate indicators within system.</span></span> <span data-ttu-id="3be7c-167">По умолчанию все отправленные индикаторы задаются как активные.</span><span class="sxs-lookup"><span data-stu-id="3be7c-167">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="3be7c-168">Однако поставщики могут отсылать существующие индикаторы с этим набором в значение false, чтобы отключить индикаторы в системе.</span><span class="sxs-lookup"><span data-stu-id="3be7c-168">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="3be7c-169">киллчаин</span><span class="sxs-lookup"><span data-stu-id="3be7c-169">killChain</span></span>|<span data-ttu-id="3be7c-170">Коллекция [киллчаин](#killchain-values)</span><span class="sxs-lookup"><span data-stu-id="3be7c-170">[killChain](#killchain-values) collection</span></span>|<span data-ttu-id="3be7c-171">Массив строк JSON, указывающий, какая точка или точки в цепочке аннулирования этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="3be7c-171">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="3be7c-172">Точные значения приведены в разделе "значения Киллчаин".</span><span class="sxs-lookup"><span data-stu-id="3be7c-172">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="3be7c-173">кновнфалсепоситивес</span><span class="sxs-lookup"><span data-stu-id="3be7c-173">knownFalsePositives</span></span>|<span data-ttu-id="3be7c-174">String</span><span class="sxs-lookup"><span data-stu-id="3be7c-174">String</span></span>|<span data-ttu-id="3be7c-175">Сценарии, в которых индикатор может вызывать ложные срабатывания.</span><span class="sxs-lookup"><span data-stu-id="3be7c-175">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="3be7c-176">Это должен быть понятный для человека текст.</span><span class="sxs-lookup"><span data-stu-id="3be7c-176">This should be human-readable text.</span></span>|
|<span data-ttu-id="3be7c-177">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3be7c-177">lastReportedDateTime</span></span>|<span data-ttu-id="3be7c-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3be7c-178">DateTimeOffset</span></span>|<span data-ttu-id="3be7c-179">Время последнего рассмотрения индикатора.</span><span class="sxs-lookup"><span data-stu-id="3be7c-179">The last time the indicator was seen.</span></span> <span data-ttu-id="3be7c-180">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3be7c-180">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3be7c-181">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="3be7c-181">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="3be7c-182">малварефамилинамес</span><span class="sxs-lookup"><span data-stu-id="3be7c-182">malwareFamilyNames</span></span>|<span data-ttu-id="3be7c-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3be7c-183">String collection</span></span>|<span data-ttu-id="3be7c-184">Имя семейства вредоносных программ, связанное с индикатором, если оно существует.</span><span class="sxs-lookup"><span data-stu-id="3be7c-184">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="3be7c-185">Корпорация Майкрософт применяет имя семейства вредоносных программ (Майкрософт), если это возможно, то, что можно найти с помощью [энциклопедии](https://www.microsoft.com/wdsi/threats)по системе безопасности защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="3be7c-185">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="3be7c-186">пассивеонли</span><span class="sxs-lookup"><span data-stu-id="3be7c-186">passiveOnly</span></span>|<span data-ttu-id="3be7c-187">Логический</span><span class="sxs-lookup"><span data-stu-id="3be7c-187">Boolean</span></span>|<span data-ttu-id="3be7c-188">Определяет, должен ли индикатор инициировать событие, видимое конечному пользователю.</span><span class="sxs-lookup"><span data-stu-id="3be7c-188">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="3be7c-189">Если задано значение true, средства безопасности не уведомляют конечного пользователя о выполнении "попадания".</span><span class="sxs-lookup"><span data-stu-id="3be7c-189">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="3be7c-190">Чаще всего это рассматривается как аудит или тихий режим по продуктам безопасности, в котором они просто зарегистрируются, но не будут выполнять действие.</span><span class="sxs-lookup"><span data-stu-id="3be7c-190">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="3be7c-191">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="3be7c-191">Default value is false.</span></span>|
|<span data-ttu-id="3be7c-192">severity</span><span class="sxs-lookup"><span data-stu-id="3be7c-192">severity</span></span>|<span data-ttu-id="3be7c-193">Int32</span><span class="sxs-lookup"><span data-stu-id="3be7c-193">Int32</span></span>|<span data-ttu-id="3be7c-194">Целое число, представляющее серьезность вредоносного поведения, идентифицируемого данными в индикаторе.</span><span class="sxs-lookup"><span data-stu-id="3be7c-194">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="3be7c-195">Допустимые значения: 0 – 5, где 5 — самый серьезный, а ноль — нет.</span><span class="sxs-lookup"><span data-stu-id="3be7c-195">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="3be7c-196">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="3be7c-196">Default value is 3.</span></span>|
|<span data-ttu-id="3be7c-197">tags</span><span class="sxs-lookup"><span data-stu-id="3be7c-197">tags</span></span>|<span data-ttu-id="3be7c-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3be7c-198">String collection</span></span>|<span data-ttu-id="3be7c-199">Массив строк JSON, в котором хранятся произвольные Теги и ключевые слова.</span><span class="sxs-lookup"><span data-stu-id="3be7c-199">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="3be7c-200">тлплевел</span><span class="sxs-lookup"><span data-stu-id="3be7c-200">tlpLevel</span></span>|[<span data-ttu-id="3be7c-201">тлплевел</span><span class="sxs-lookup"><span data-stu-id="3be7c-201">tlpLevel</span></span>](#tlplevel-values)| <span data-ttu-id="3be7c-202">Значение протокола светофора для индикатора.</span><span class="sxs-lookup"><span data-stu-id="3be7c-202">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="3be7c-203">Возможные значения: `unknown`, `white`, `green`, `amber`, `red`.</span><span class="sxs-lookup"><span data-stu-id="3be7c-203">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="3be7c-204">значения Диамондмодел</span><span class="sxs-lookup"><span data-stu-id="3be7c-204">diamondModel values</span></span>

<span data-ttu-id="3be7c-205">Сведения об этой модели можно найти [в разделе Модель ромба](http://diamondmodel.org).</span><span class="sxs-lookup"><span data-stu-id="3be7c-205">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="3be7c-206">Значения</span><span class="sxs-lookup"><span data-stu-id="3be7c-206">Values</span></span> | <span data-ttu-id="3be7c-207">Описание</span><span class="sxs-lookup"><span data-stu-id="3be7c-207">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="3be7c-208">Злоумышленник</span><span class="sxs-lookup"><span data-stu-id="3be7c-208">adversary</span></span>|<span data-ttu-id="3be7c-209">Индикатор описывает.</span><span class="sxs-lookup"><span data-stu-id="3be7c-209">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="3be7c-210">поставлен</span><span class="sxs-lookup"><span data-stu-id="3be7c-210">capability</span></span>|<span data-ttu-id="3be7c-211">Индикатор является возможностью злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="3be7c-211">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="3be7c-212">инфраструктур</span><span class="sxs-lookup"><span data-stu-id="3be7c-212">infrastructure</span></span>|<span data-ttu-id="3be7c-213">Индикатор описывает инфраструктуру злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="3be7c-213">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="3be7c-214">стала</span><span class="sxs-lookup"><span data-stu-id="3be7c-214">victim</span></span>|<span data-ttu-id="3be7c-215">Индикатор описывает жертвой злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="3be7c-215">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="3be7c-216">значения Киллчаин</span><span class="sxs-lookup"><span data-stu-id="3be7c-216">killChain values</span></span>

| <span data-ttu-id="3be7c-217">Значения</span><span class="sxs-lookup"><span data-stu-id="3be7c-217">Values</span></span> | <span data-ttu-id="3be7c-218">Описание</span><span class="sxs-lookup"><span data-stu-id="3be7c-218">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="3be7c-219">Действия</span><span class="sxs-lookup"><span data-stu-id="3be7c-219">Actions</span></span>|<span data-ttu-id="3be7c-220">Представляет "действия по целям".</span><span class="sxs-lookup"><span data-stu-id="3be7c-220">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="3be7c-221">Злоумышленник получает такие действия, как распределенная атака типа "отказ в обслуживании".</span><span class="sxs-lookup"><span data-stu-id="3be7c-221">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="3be7c-222">C2</span><span class="sxs-lookup"><span data-stu-id="3be7c-222">C2</span></span>|<span data-ttu-id="3be7c-223">Представляет канал управления, с которым работает скомпрометированная система.</span><span class="sxs-lookup"><span data-stu-id="3be7c-223">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="3be7c-224">Delivery</span><span class="sxs-lookup"><span data-stu-id="3be7c-224">Delivery</span></span>|<span data-ttu-id="3be7c-225">Процесс распространения кода эксплойта для жертв (например, USB, электронной почты, веб-сайтов).</span><span class="sxs-lookup"><span data-stu-id="3be7c-225">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="3be7c-226">Опасность</span><span class="sxs-lookup"><span data-stu-id="3be7c-226">Exploitation</span></span>|<span data-ttu-id="3be7c-227">Код эксплойта использует преимущества уязвимостей (например, выполнение кода).</span><span class="sxs-lookup"><span data-stu-id="3be7c-227">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="3be7c-228">Установка</span><span class="sxs-lookup"><span data-stu-id="3be7c-228">Installation</span></span>|<span data-ttu-id="3be7c-229">Установка вредоносных программ после использования уязвимости.</span><span class="sxs-lookup"><span data-stu-id="3be7c-229">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="3be7c-230">реконнаиссанце</span><span class="sxs-lookup"><span data-stu-id="3be7c-230">Reconnaissance</span></span>|<span data-ttu-id="3be7c-231">Индикатор — это свидетельство того, что Группа действий получает сведения, которые будут использоваться при следующей атаке.</span><span class="sxs-lookup"><span data-stu-id="3be7c-231">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="3be7c-232">веапонизатион</span><span class="sxs-lookup"><span data-stu-id="3be7c-232">Weaponization</span></span>|<span data-ttu-id="3be7c-233">Включение уязвимости в код эксплойта (например, вредоносные программы).</span><span class="sxs-lookup"><span data-stu-id="3be7c-233">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="3be7c-234">значения Тлплевел</span><span class="sxs-lookup"><span data-stu-id="3be7c-234">tlpLevel values</span></span>

<span data-ttu-id="3be7c-235">При отправке каждого индикатора должен быть задано значение протокола светофора (ТЛП).</span><span class="sxs-lookup"><span data-stu-id="3be7c-235">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="3be7c-236">Это значение представляет собой чувствительность и область общего доступа к заданному индикатору.</span><span class="sxs-lookup"><span data-stu-id="3be7c-236">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="3be7c-237">Значения</span><span class="sxs-lookup"><span data-stu-id="3be7c-237">Values</span></span> | <span data-ttu-id="3be7c-238">Описание</span><span class="sxs-lookup"><span data-stu-id="3be7c-238">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="3be7c-239">Белый</span><span class="sxs-lookup"><span data-stu-id="3be7c-239">White</span></span>| <span data-ttu-id="3be7c-240">Область общего доступа: unlimited.</span><span class="sxs-lookup"><span data-stu-id="3be7c-240">Sharing scope: Unlimited.</span></span> <span data-ttu-id="3be7c-241">Индикаторы могут быть предоставлены бесплатно, без ограничений.</span><span class="sxs-lookup"><span data-stu-id="3be7c-241">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="3be7c-242">Зеленый</span><span class="sxs-lookup"><span data-stu-id="3be7c-242">Green</span></span>| <span data-ttu-id="3be7c-243">Область общего доступа: сообщество.</span><span class="sxs-lookup"><span data-stu-id="3be7c-243">Sharing scope: Community.</span></span> <span data-ttu-id="3be7c-244">С помощью сообщества безопасности можно предоставить доступ к индикаторам.</span><span class="sxs-lookup"><span data-stu-id="3be7c-244">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="3be7c-245">Оранжевого</span><span class="sxs-lookup"><span data-stu-id="3be7c-245">Amber</span></span>| <span data-ttu-id="3be7c-246">Область общего доступа: ограничена.</span><span class="sxs-lookup"><span data-stu-id="3be7c-246">Sharing scope: Limited.</span></span> <span data-ttu-id="3be7c-247">Это параметр по умолчанию для индикаторов и разрешает совместное использование только тем, у которых есть ненужные: 1) службы и операторы служб, реализующие логику операций с угрозами; 2) клиенты, чьи системы соответствуют поведению с индикатором.</span><span class="sxs-lookup"><span data-stu-id="3be7c-247">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="3be7c-248">Красный</span><span class="sxs-lookup"><span data-stu-id="3be7c-248">Red</span></span>| <span data-ttu-id="3be7c-249">Область общего доступа: личная.</span><span class="sxs-lookup"><span data-stu-id="3be7c-249">Sharing scope: Personal.</span></span> <span data-ttu-id="3be7c-250">Эти индикаторы предназначены только для предоставления доступа напрямую и, желательно, в случае человека.</span><span class="sxs-lookup"><span data-stu-id="3be7c-250">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="3be7c-251">Как правило, ТЛП красные индикаторы не отправляются из-за ограничений, заданных ранее.</span><span class="sxs-lookup"><span data-stu-id="3be7c-251">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="3be7c-252">Если отправляются красные индикаторы ТЛП, свойству **пассивеонли** следует присвоить значение `True` также.</span><span class="sxs-lookup"><span data-stu-id="3be7c-252">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="3be7c-253">Ответ</span><span class="sxs-lookup"><span data-stu-id="3be7c-253">Response</span></span>

<span data-ttu-id="3be7c-254">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3be7c-254">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="3be7c-255">Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3be7c-255">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3be7c-256">Примеры</span><span class="sxs-lookup"><span data-stu-id="3be7c-256">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="3be7c-257">Пример 1: запрос без верхнего колонтитула</span><span class="sxs-lookup"><span data-stu-id="3be7c-257">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="3be7c-258">Запрос</span><span class="sxs-lookup"><span data-stu-id="3be7c-258">Request</span></span>

<span data-ttu-id="3be7c-259">Ниже приведен пример запроса без `Prefer` заголовка.</span><span class="sxs-lookup"><span data-stu-id="3be7c-259">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="3be7c-260">HTTP</span><span class="sxs-lookup"><span data-stu-id="3be7c-260">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```
# <a name="c"></a>[<span data-ttu-id="3be7c-261">C#</span><span class="sxs-lookup"><span data-stu-id="3be7c-261">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3be7c-262">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3be7c-262">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3be7c-263">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3be7c-263">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3be7c-264">Отклик</span><span class="sxs-lookup"><span data-stu-id="3be7c-264">Response</span></span>

<span data-ttu-id="3be7c-265">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3be7c-265">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="3be7c-266">Пример 2: запрос с заголовком предпочтения</span><span class="sxs-lookup"><span data-stu-id="3be7c-266">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="3be7c-267">Запрос</span><span class="sxs-lookup"><span data-stu-id="3be7c-267">Request</span></span>

<span data-ttu-id="3be7c-268">Ниже приведен пример запроса, включающего `Prefer` заголовок.</span><span class="sxs-lookup"><span data-stu-id="3be7c-268">The following is an example of the request that includes the `Prefer` header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json
Prefer: return=representation

{
  "additionalInformation": "additionalInformation-after-update",
  "confidence": 42,
  "description": "description-after-update",
}
```

#### <a name="response"></a><span data-ttu-id="3be7c-269">Отклик</span><span class="sxs-lookup"><span data-stu-id="3be7c-269">Response</span></span>

<span data-ttu-id="3be7c-270">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3be7c-270">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="3be7c-271">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3be7c-271">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3be7c-272">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3be7c-272">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXXXXXXX",
    "action": null,
    "additionalInformation": "additionalInformation-after-update",
    "activityGroupNames": [],
    "confidence": 42,
    "description": "description-after-update",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

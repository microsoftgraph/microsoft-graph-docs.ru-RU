---
title: Обновление объекта tiIndicator
description: Обновление свойств объекта Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: d5d02eab6441941d9bcdcb62bf78c353e26e3e5a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362733"
---
# <a name="update-tiindicator"></a><span data-ttu-id="80bd4-103">Обновление объекта tiIndicator</span><span class="sxs-lookup"><span data-stu-id="80bd4-103">Update tiIndicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80bd4-104">Обновление свойств объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="80bd4-104">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="80bd4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80bd4-105">Permissions</span></span>

<span data-ttu-id="80bd4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80bd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="80bd4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80bd4-108">Permission type</span></span>                        | <span data-ttu-id="80bd4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80bd4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="80bd4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80bd4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="80bd4-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="80bd4-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="80bd4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80bd4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80bd4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80bd4-113">Not supported.</span></span> |
| <span data-ttu-id="80bd4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80bd4-114">Application</span></span>                            | <span data-ttu-id="80bd4-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="80bd4-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="80bd4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80bd4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="80bd4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80bd4-117">Request headers</span></span>

| <span data-ttu-id="80bd4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="80bd4-118">Name</span></span>       | <span data-ttu-id="80bd4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="80bd4-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="80bd4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80bd4-120">Authorization</span></span> | <span data-ttu-id="80bd4-121">**Необходим** носитель {код}</span><span class="sxs-lookup"><span data-stu-id="80bd4-121">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="80bd4-122">Prefer</span><span class="sxs-lookup"><span data-stu-id="80bd4-122">Prefer</span></span> | <span data-ttu-id="80bd4-123">Возврат = представление</span><span class="sxs-lookup"><span data-stu-id="80bd4-123">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="80bd4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80bd4-124">Request body</span></span>

<span data-ttu-id="80bd4-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="80bd4-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="80bd4-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="80bd4-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="80bd4-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="80bd4-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="80bd4-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="80bd4-128">Property</span></span>     | <span data-ttu-id="80bd4-129">Тип</span><span class="sxs-lookup"><span data-stu-id="80bd4-129">Type</span></span>        | <span data-ttu-id="80bd4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="80bd4-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="80bd4-131">action</span><span class="sxs-lookup"><span data-stu-id="80bd4-131">action</span></span>|<span data-ttu-id="80bd4-132">string</span><span class="sxs-lookup"><span data-stu-id="80bd4-132">string</span></span>| <span data-ttu-id="80bd4-133">Действие, которое необходимо применить, если индикатор сопоставлен с помощью средства безопасности Таржетпродукт.</span><span class="sxs-lookup"><span data-stu-id="80bd4-133">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="80bd4-134">Возможные значения: `unknown`, `allow`, `block`, `alert`.</span><span class="sxs-lookup"><span data-stu-id="80bd4-134">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="80bd4-135">активитиграупнамес</span><span class="sxs-lookup"><span data-stu-id="80bd4-135">activityGroupNames</span></span>|<span data-ttu-id="80bd4-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="80bd4-136">String collection</span></span>|<span data-ttu-id="80bd4-137">Имя (-ы) логики операций с угрозами кибератак для сторон, ответственных за вредоносные действия, охваченные индикатором угроз.</span><span class="sxs-lookup"><span data-stu-id="80bd4-137">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="80bd4-138">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="80bd4-138">additionalInformation</span></span>|<span data-ttu-id="80bd4-139">String</span><span class="sxs-lookup"><span data-stu-id="80bd4-139">String</span></span>|<span data-ttu-id="80bd4-140">Область общего пользования, в которую могут быть размещены дополнительные данные из индикатора, не охваченные другими свойствами Тииндикатор.</span><span class="sxs-lookup"><span data-stu-id="80bd4-140">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="80bd4-141">Данные, помещаемые в Аддитионалинформатион, обычно не используются средством безопасности Таржетпродукт.</span><span class="sxs-lookup"><span data-stu-id="80bd4-141">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="80bd4-142">confidence</span><span class="sxs-lookup"><span data-stu-id="80bd4-142">confidence</span></span>|<span data-ttu-id="80bd4-143">Int32</span><span class="sxs-lookup"><span data-stu-id="80bd4-143">Int32</span></span>|<span data-ttu-id="80bd4-144">Целое число, представляющее достоверность, с помощью которой данные в индикаторе точно определяют вредоносное поведение.</span><span class="sxs-lookup"><span data-stu-id="80bd4-144">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="80bd4-145">Допустимые значения: 0 – 100 с 100 по убыванию.</span><span class="sxs-lookup"><span data-stu-id="80bd4-145">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="80bd4-146">description</span><span class="sxs-lookup"><span data-stu-id="80bd4-146">description</span></span>|<span data-ttu-id="80bd4-147">String</span><span class="sxs-lookup"><span data-stu-id="80bd4-147">String</span></span>|<span data-ttu-id="80bd4-148">Краткое описание угрозы, представленное индикатором (100 символов или меньше).</span><span class="sxs-lookup"><span data-stu-id="80bd4-148">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="80bd4-149">диамондмодел</span><span class="sxs-lookup"><span data-stu-id="80bd4-149">diamondModel</span></span>|[<span data-ttu-id="80bd4-150">диамондмодел</span><span class="sxs-lookup"><span data-stu-id="80bd4-150">diamondModel</span></span>](#diamondmodel-values)|<span data-ttu-id="80bd4-151">Область модели ромба, в которой существует этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="80bd4-151">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="80bd4-152">Возможные значения: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span><span class="sxs-lookup"><span data-stu-id="80bd4-152">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="80bd4-153">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="80bd4-153">expirationDateTime</span></span>|<span data-ttu-id="80bd4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80bd4-154">DateTimeOffset</span></span>| <span data-ttu-id="80bd4-155">Строка DateTime, указывающая, когда истечет срок действия индикатора.</span><span class="sxs-lookup"><span data-stu-id="80bd4-155">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="80bd4-156">Все индикаторы должны иметь дату истечения срока действия, чтобы не допустить устаревших показателей в системе.</span><span class="sxs-lookup"><span data-stu-id="80bd4-156">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="80bd4-157">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="80bd4-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80bd4-158">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="80bd4-158">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="80bd4-159">externalId</span><span class="sxs-lookup"><span data-stu-id="80bd4-159">externalId</span></span>|<span data-ttu-id="80bd4-160">String</span><span class="sxs-lookup"><span data-stu-id="80bd4-160">String</span></span>|<span data-ttu-id="80bd4-161">Идентификационный номер, который привязывает индикатор к системе поставщика индикаторов (например, внешнему ключу).</span><span class="sxs-lookup"><span data-stu-id="80bd4-161">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="80bd4-162">isActive</span><span class="sxs-lookup"><span data-stu-id="80bd4-162">isActive</span></span>|<span data-ttu-id="80bd4-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="80bd4-163">Boolean</span></span>|<span data-ttu-id="80bd4-164">Используется для отключения индикаторов в системе.</span><span class="sxs-lookup"><span data-stu-id="80bd4-164">Used to deactivate indicators within system.</span></span> <span data-ttu-id="80bd4-165">По умолчанию все отправленные индикаторы задаются как активные.</span><span class="sxs-lookup"><span data-stu-id="80bd4-165">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="80bd4-166">Однако поставщики могут отсылать существующие индикаторы с этим набором в значение false, чтобы отключить индикаторы в системе.</span><span class="sxs-lookup"><span data-stu-id="80bd4-166">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="80bd4-167">киллчаин</span><span class="sxs-lookup"><span data-stu-id="80bd4-167">killChain</span></span>|<span data-ttu-id="80bd4-168">Коллекция [киллчаин](#killchain-values)</span><span class="sxs-lookup"><span data-stu-id="80bd4-168">[killChain](#killchain-values) collection</span></span>|<span data-ttu-id="80bd4-169">Массив строк JSON, указывающий, какая точка или точки в цепочке аннулирования этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="80bd4-169">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="80bd4-170">Точные значения приведены в разделе "значения Киллчаин".</span><span class="sxs-lookup"><span data-stu-id="80bd4-170">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="80bd4-171">кновнфалсепоситивес</span><span class="sxs-lookup"><span data-stu-id="80bd4-171">knownFalsePositives</span></span>|<span data-ttu-id="80bd4-172">String</span><span class="sxs-lookup"><span data-stu-id="80bd4-172">String</span></span>|<span data-ttu-id="80bd4-173">Сценарии, в которых индикатор может вызывать ложные срабатывания.</span><span class="sxs-lookup"><span data-stu-id="80bd4-173">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="80bd4-174">Это должен быть понятный для человека текст.</span><span class="sxs-lookup"><span data-stu-id="80bd4-174">This should be human-readable text.</span></span>|
|<span data-ttu-id="80bd4-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="80bd4-175">lastReportedDateTime</span></span>|<span data-ttu-id="80bd4-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80bd4-176">DateTimeOffset</span></span>|<span data-ttu-id="80bd4-177">Время последнего рассмотрения индикатора.</span><span class="sxs-lookup"><span data-stu-id="80bd4-177">The last time the indicator was seen.</span></span> <span data-ttu-id="80bd4-178">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="80bd4-178">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80bd4-179">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="80bd4-179">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="80bd4-180">малварефамилинамес</span><span class="sxs-lookup"><span data-stu-id="80bd4-180">malwareFamilyNames</span></span>|<span data-ttu-id="80bd4-181">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="80bd4-181">String collection</span></span>|<span data-ttu-id="80bd4-182">Имя семейства вредоносных программ, связанное с индикатором, если оно существует.</span><span class="sxs-lookup"><span data-stu-id="80bd4-182">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="80bd4-183">Корпорация Майкрософт применяет имя семейства вредоносных программ (Майкрософт), если это возможно, то, что можно [](https://www.microsoft.com/wdsi/threats)найти с помощью энциклопедии по системе безопасности защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="80bd4-183">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="80bd4-184">пассивеонли</span><span class="sxs-lookup"><span data-stu-id="80bd4-184">passiveOnly</span></span>|<span data-ttu-id="80bd4-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="80bd4-185">Boolean</span></span>|<span data-ttu-id="80bd4-186">Определяет, должен ли индикатор инициировать событие, видимое конечному пользователю.</span><span class="sxs-lookup"><span data-stu-id="80bd4-186">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="80bd4-187">Если задано значение true, средства безопасности не уведомляют конечного пользователя о выполнении "попадания".</span><span class="sxs-lookup"><span data-stu-id="80bd4-187">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="80bd4-188">Чаще всего это рассматривается как аудит или тихий режим по продуктам безопасности, в котором они просто зарегистрируются, но не будут выполнять действие.</span><span class="sxs-lookup"><span data-stu-id="80bd4-188">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="80bd4-189">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="80bd4-189">Default value is false.</span></span>|
|<span data-ttu-id="80bd4-190">severity</span><span class="sxs-lookup"><span data-stu-id="80bd4-190">severity</span></span>|<span data-ttu-id="80bd4-191">Int32</span><span class="sxs-lookup"><span data-stu-id="80bd4-191">Int32</span></span>|<span data-ttu-id="80bd4-192">Целое число, представляющее серьезность вредоносного поведения, идентифицируемого данными в индикаторе.</span><span class="sxs-lookup"><span data-stu-id="80bd4-192">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="80bd4-193">Допустимые значения: 0 – 5, где 5 — самый серьезный, а ноль — нет.</span><span class="sxs-lookup"><span data-stu-id="80bd4-193">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="80bd4-194">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="80bd4-194">Default value is 3.</span></span>|
|<span data-ttu-id="80bd4-195">tags</span><span class="sxs-lookup"><span data-stu-id="80bd4-195">tags</span></span>|<span data-ttu-id="80bd4-196">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="80bd4-196">String collection</span></span>|<span data-ttu-id="80bd4-197">Массив строк JSON, в котором хранятся произвольные Теги и ключевые слова.</span><span class="sxs-lookup"><span data-stu-id="80bd4-197">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="80bd4-198">тлплевел</span><span class="sxs-lookup"><span data-stu-id="80bd4-198">tlpLevel</span></span>|[<span data-ttu-id="80bd4-199">тлплевел</span><span class="sxs-lookup"><span data-stu-id="80bd4-199">tlpLevel</span></span>](#tlplevel-values)| <span data-ttu-id="80bd4-200">Значение протокола светофора для индикатора.</span><span class="sxs-lookup"><span data-stu-id="80bd4-200">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="80bd4-201">Возможные значения: `unknown`, `white`, `green`, `amber`, `red`.</span><span class="sxs-lookup"><span data-stu-id="80bd4-201">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="80bd4-202">значения Диамондмодел</span><span class="sxs-lookup"><span data-stu-id="80bd4-202">diamondModel values</span></span>

<span data-ttu-id="80bd4-203">Сведения об этой модели можно найти [в разделе Модель ромба](http://diamondmodel.org).</span><span class="sxs-lookup"><span data-stu-id="80bd4-203">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="80bd4-204">Значения</span><span class="sxs-lookup"><span data-stu-id="80bd4-204">Values</span></span> | <span data-ttu-id="80bd4-205">Описание</span><span class="sxs-lookup"><span data-stu-id="80bd4-205">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="80bd4-206">Злоумышленник</span><span class="sxs-lookup"><span data-stu-id="80bd4-206">adversary</span></span>|<span data-ttu-id="80bd4-207">Индикатор описывает.</span><span class="sxs-lookup"><span data-stu-id="80bd4-207">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="80bd4-208">поставлен</span><span class="sxs-lookup"><span data-stu-id="80bd4-208">capability</span></span>|<span data-ttu-id="80bd4-209">Индикатор является возможностью злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="80bd4-209">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="80bd4-210">инфраструктур</span><span class="sxs-lookup"><span data-stu-id="80bd4-210">infrastructure</span></span>|<span data-ttu-id="80bd4-211">Индикатор описывает инфраструктуру злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="80bd4-211">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="80bd4-212">стала</span><span class="sxs-lookup"><span data-stu-id="80bd4-212">victim</span></span>|<span data-ttu-id="80bd4-213">Индикатор описывает жертвой злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="80bd4-213">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="80bd4-214">значения Киллчаин</span><span class="sxs-lookup"><span data-stu-id="80bd4-214">killChain values</span></span>

| <span data-ttu-id="80bd4-215">Значения</span><span class="sxs-lookup"><span data-stu-id="80bd4-215">Values</span></span> | <span data-ttu-id="80bd4-216">Описание</span><span class="sxs-lookup"><span data-stu-id="80bd4-216">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="80bd4-217">Действия</span><span class="sxs-lookup"><span data-stu-id="80bd4-217">Actions</span></span>|<span data-ttu-id="80bd4-218">Представляет "действия по целям".</span><span class="sxs-lookup"><span data-stu-id="80bd4-218">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="80bd4-219">Злоумышленник получает такие действия, как распределенная атака типа "отказ в обслуживании".</span><span class="sxs-lookup"><span data-stu-id="80bd4-219">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="80bd4-220">C2</span><span class="sxs-lookup"><span data-stu-id="80bd4-220">C2</span></span>|<span data-ttu-id="80bd4-221">Представляет канал управления, с которым работает скомпрометированная система.</span><span class="sxs-lookup"><span data-stu-id="80bd4-221">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="80bd4-222">Delivery</span><span class="sxs-lookup"><span data-stu-id="80bd4-222">Delivery</span></span>|<span data-ttu-id="80bd4-223">Процесс распространения кода эксплойта для жертв (например, USB, электронной почты, веб-сайтов).</span><span class="sxs-lookup"><span data-stu-id="80bd4-223">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="80bd4-224">Опасность</span><span class="sxs-lookup"><span data-stu-id="80bd4-224">Exploitation</span></span>|<span data-ttu-id="80bd4-225">Код эксплойта использует преимущества уязвимостей (например, выполнение кода).</span><span class="sxs-lookup"><span data-stu-id="80bd4-225">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="80bd4-226">Установка</span><span class="sxs-lookup"><span data-stu-id="80bd4-226">Installation</span></span>|<span data-ttu-id="80bd4-227">Установка вредоносных программ после использования уязвимости.</span><span class="sxs-lookup"><span data-stu-id="80bd4-227">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="80bd4-228">реконнаиссанце</span><span class="sxs-lookup"><span data-stu-id="80bd4-228">Reconnaissance</span></span>|<span data-ttu-id="80bd4-229">Индикатор — это свидетельство того, что Группа действий получает сведения, которые будут использоваться при следующей атаке.</span><span class="sxs-lookup"><span data-stu-id="80bd4-229">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="80bd4-230">веапонизатион</span><span class="sxs-lookup"><span data-stu-id="80bd4-230">Weaponization</span></span>|<span data-ttu-id="80bd4-231">Включение уязвимости в код эксплойта (например, вредоносные программы).</span><span class="sxs-lookup"><span data-stu-id="80bd4-231">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="80bd4-232">значения Тлплевел</span><span class="sxs-lookup"><span data-stu-id="80bd4-232">tlpLevel values</span></span>

<span data-ttu-id="80bd4-233">При отправке каждого индикатора должен быть задано значение протокола светофора (ТЛП).</span><span class="sxs-lookup"><span data-stu-id="80bd4-233">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="80bd4-234">Это значение представляет собой чувствительность и область общего доступа к заданному индикатору.</span><span class="sxs-lookup"><span data-stu-id="80bd4-234">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="80bd4-235">Значения</span><span class="sxs-lookup"><span data-stu-id="80bd4-235">Values</span></span> | <span data-ttu-id="80bd4-236">Описание</span><span class="sxs-lookup"><span data-stu-id="80bd4-236">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="80bd4-237">Белый</span><span class="sxs-lookup"><span data-stu-id="80bd4-237">White</span></span>| <span data-ttu-id="80bd4-238">Область общего доступа: unlimited.</span><span class="sxs-lookup"><span data-stu-id="80bd4-238">Sharing scope: Unlimited.</span></span> <span data-ttu-id="80bd4-239">Индикаторы могут быть предоставлены бесплатно, без ограничений.</span><span class="sxs-lookup"><span data-stu-id="80bd4-239">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="80bd4-240">Зеленый</span><span class="sxs-lookup"><span data-stu-id="80bd4-240">Green</span></span>| <span data-ttu-id="80bd4-241">Область общего доступа: сообщество.</span><span class="sxs-lookup"><span data-stu-id="80bd4-241">Sharing scope: Community.</span></span> <span data-ttu-id="80bd4-242">С помощью сообщества безопасности можно предоставить доступ к индикаторам.</span><span class="sxs-lookup"><span data-stu-id="80bd4-242">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="80bd4-243">Оранжевого</span><span class="sxs-lookup"><span data-stu-id="80bd4-243">Amber</span></span>| <span data-ttu-id="80bd4-244">Область общего доступа: ограничена.</span><span class="sxs-lookup"><span data-stu-id="80bd4-244">Sharing scope: Limited.</span></span> <span data-ttu-id="80bd4-245">Это параметр по умолчанию для индикаторов и разрешает совместное использование только тем, у которых есть ненужные: 1) службы и операторы служб, реализующие логику операций с угрозами; 2) клиенты, чьи системы соответствуют поведению с индикатором.</span><span class="sxs-lookup"><span data-stu-id="80bd4-245">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="80bd4-246">Красный</span><span class="sxs-lookup"><span data-stu-id="80bd4-246">Red</span></span>| <span data-ttu-id="80bd4-247">Область общего доступа: личная.</span><span class="sxs-lookup"><span data-stu-id="80bd4-247">Sharing scope: Personal.</span></span> <span data-ttu-id="80bd4-248">Эти индикаторы предназначены только для предоставления доступа напрямую и, желательно, в случае человека.</span><span class="sxs-lookup"><span data-stu-id="80bd4-248">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="80bd4-249">Как правило, ТЛП красные индикаторы не отправляются из-за ограничений, заданных ранее.</span><span class="sxs-lookup"><span data-stu-id="80bd4-249">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="80bd4-250">Если отправляются красные индикаторы ТЛП, свойству **пассивеонли** следует присвоить значение `True` также.</span><span class="sxs-lookup"><span data-stu-id="80bd4-250">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="80bd4-251">Ответ</span><span class="sxs-lookup"><span data-stu-id="80bd4-251">Response</span></span>

<span data-ttu-id="80bd4-252">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="80bd4-252">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="80bd4-253">Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="80bd4-253">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80bd4-254">Примеры</span><span class="sxs-lookup"><span data-stu-id="80bd4-254">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="80bd4-255">Пример 1: запрос без верхнего колонтитула</span><span class="sxs-lookup"><span data-stu-id="80bd4-255">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="80bd4-256">Запрос</span><span class="sxs-lookup"><span data-stu-id="80bd4-256">Request</span></span>

<span data-ttu-id="80bd4-257">Ниже приведен пример запроса без `Prefer` заголовка.</span><span class="sxs-lookup"><span data-stu-id="80bd4-257">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="80bd4-258">HTTP</span><span class="sxs-lookup"><span data-stu-id="80bd4-258">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="80bd4-259">C#</span><span class="sxs-lookup"><span data-stu-id="80bd4-259">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80bd4-260">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80bd4-260">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="80bd4-261">Цель — C</span><span class="sxs-lookup"><span data-stu-id="80bd4-261">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="80bd4-262">Java</span><span class="sxs-lookup"><span data-stu-id="80bd4-262">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="80bd4-263">Отклик</span><span class="sxs-lookup"><span data-stu-id="80bd4-263">Response</span></span>

<span data-ttu-id="80bd4-264">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="80bd4-264">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="80bd4-265">Пример 2: запрос с заголовком предпочтения</span><span class="sxs-lookup"><span data-stu-id="80bd4-265">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="80bd4-266">Запрос</span><span class="sxs-lookup"><span data-stu-id="80bd4-266">Request</span></span>

<span data-ttu-id="80bd4-267">Ниже приведен пример запроса, включающего `Prefer` заголовок.</span><span class="sxs-lookup"><span data-stu-id="80bd4-267">The following is an example of the request that includes the `Prefer` header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="80bd4-268">Отклик</span><span class="sxs-lookup"><span data-stu-id="80bd4-268">Response</span></span>

<span data-ttu-id="80bd4-269">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="80bd4-269">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="80bd4-270">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="80bd4-270">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="80bd4-271">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80bd4-271">All the properties will be returned from an actual call.</span></span>

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

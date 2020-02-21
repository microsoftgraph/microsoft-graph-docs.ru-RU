---
title: Обновление объекта tiIndicator
description: Обновление свойств объекта Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 34c73f3acec6084989f48d7e96b7bc05cbd2b115
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219743"
---
# <a name="update-tiindicator"></a><span data-ttu-id="65ba1-103">Обновление объекта tiIndicator</span><span class="sxs-lookup"><span data-stu-id="65ba1-103">Update tiIndicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65ba1-104">Обновление свойств объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="65ba1-104">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="65ba1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65ba1-105">Permissions</span></span>

<span data-ttu-id="65ba1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65ba1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65ba1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65ba1-108">Permission type</span></span>                        | <span data-ttu-id="65ba1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65ba1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="65ba1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65ba1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="65ba1-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="65ba1-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="65ba1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65ba1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65ba1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65ba1-113">Not supported.</span></span> |
| <span data-ttu-id="65ba1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65ba1-114">Application</span></span>                            | <span data-ttu-id="65ba1-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="65ba1-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="65ba1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65ba1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="65ba1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65ba1-117">Request headers</span></span>

| <span data-ttu-id="65ba1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="65ba1-118">Name</span></span>       | <span data-ttu-id="65ba1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="65ba1-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="65ba1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="65ba1-120">Authorization</span></span> | <span data-ttu-id="65ba1-121">**Необходим** носитель {код}</span><span class="sxs-lookup"><span data-stu-id="65ba1-121">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="65ba1-122">Prefer</span><span class="sxs-lookup"><span data-stu-id="65ba1-122">Prefer</span></span> | <span data-ttu-id="65ba1-123">Возврат = представление</span><span class="sxs-lookup"><span data-stu-id="65ba1-123">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="65ba1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65ba1-124">Request body</span></span>

<span data-ttu-id="65ba1-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="65ba1-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="65ba1-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="65ba1-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="65ba1-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="65ba1-127">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="65ba1-128">Обязательные поля: `id`, `expirationDateTime`, `targetProduct`.</span><span class="sxs-lookup"><span data-stu-id="65ba1-128">Required fields are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="65ba1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="65ba1-129">Property</span></span>     | <span data-ttu-id="65ba1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="65ba1-130">Type</span></span>        | <span data-ttu-id="65ba1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="65ba1-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="65ba1-132">action</span><span class="sxs-lookup"><span data-stu-id="65ba1-132">action</span></span>|<span data-ttu-id="65ba1-133">string</span><span class="sxs-lookup"><span data-stu-id="65ba1-133">string</span></span>| <span data-ttu-id="65ba1-134">Действие, которое необходимо применить, если индикатор сопоставлен с помощью средства безопасности Таржетпродукт.</span><span class="sxs-lookup"><span data-stu-id="65ba1-134">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="65ba1-135">Возможные значения: `unknown`, `allow`, `block`, `alert`.</span><span class="sxs-lookup"><span data-stu-id="65ba1-135">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="65ba1-136">активитиграупнамес</span><span class="sxs-lookup"><span data-stu-id="65ba1-136">activityGroupNames</span></span>|<span data-ttu-id="65ba1-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65ba1-137">String collection</span></span>|<span data-ttu-id="65ba1-138">Имя (-ы) логики операций с угрозами кибератак для сторон, ответственных за вредоносные действия, охваченные индикатором угроз.</span><span class="sxs-lookup"><span data-stu-id="65ba1-138">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="65ba1-139">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="65ba1-139">additionalInformation</span></span>|<span data-ttu-id="65ba1-140">String</span><span class="sxs-lookup"><span data-stu-id="65ba1-140">String</span></span>|<span data-ttu-id="65ba1-141">Область общего пользования, в которую могут быть размещены дополнительные данные из индикатора, не охваченные другими свойствами Тииндикатор.</span><span class="sxs-lookup"><span data-stu-id="65ba1-141">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="65ba1-142">Данные, помещаемые в Аддитионалинформатион, обычно не используются средством безопасности Таржетпродукт.</span><span class="sxs-lookup"><span data-stu-id="65ba1-142">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="65ba1-143">confidence</span><span class="sxs-lookup"><span data-stu-id="65ba1-143">confidence</span></span>|<span data-ttu-id="65ba1-144">Int32</span><span class="sxs-lookup"><span data-stu-id="65ba1-144">Int32</span></span>|<span data-ttu-id="65ba1-145">Целое число, представляющее достоверность, с помощью которой данные в индикаторе точно определяют вредоносное поведение.</span><span class="sxs-lookup"><span data-stu-id="65ba1-145">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="65ba1-146">Допустимые значения: 0 – 100 с 100 по убыванию.</span><span class="sxs-lookup"><span data-stu-id="65ba1-146">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="65ba1-147">description</span><span class="sxs-lookup"><span data-stu-id="65ba1-147">description</span></span>|<span data-ttu-id="65ba1-148">String</span><span class="sxs-lookup"><span data-stu-id="65ba1-148">String</span></span>|<span data-ttu-id="65ba1-149">Краткое описание угрозы, представленное индикатором (100 символов или меньше).</span><span class="sxs-lookup"><span data-stu-id="65ba1-149">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="65ba1-150">диамондмодел</span><span class="sxs-lookup"><span data-stu-id="65ba1-150">diamondModel</span></span>|[<span data-ttu-id="65ba1-151">диамондмодел</span><span class="sxs-lookup"><span data-stu-id="65ba1-151">diamondModel</span></span>](#diamondmodel-values)|<span data-ttu-id="65ba1-152">Область модели ромба, в которой существует этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="65ba1-152">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="65ba1-153">Возможные значения: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span><span class="sxs-lookup"><span data-stu-id="65ba1-153">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="65ba1-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="65ba1-154">expirationDateTime</span></span>|<span data-ttu-id="65ba1-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65ba1-155">DateTimeOffset</span></span>| <span data-ttu-id="65ba1-156">Строка DateTime, указывающая, когда истечет срок действия индикатора.</span><span class="sxs-lookup"><span data-stu-id="65ba1-156">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="65ba1-157">Все индикаторы должны иметь дату истечения срока действия, чтобы не допустить устаревших показателей в системе.</span><span class="sxs-lookup"><span data-stu-id="65ba1-157">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="65ba1-158">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="65ba1-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="65ba1-159">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="65ba1-159">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="65ba1-160">externalId</span><span class="sxs-lookup"><span data-stu-id="65ba1-160">externalId</span></span>|<span data-ttu-id="65ba1-161">String</span><span class="sxs-lookup"><span data-stu-id="65ba1-161">String</span></span>|<span data-ttu-id="65ba1-162">Идентификационный номер, который привязывает индикатор к системе поставщика индикаторов (например, внешнему ключу).</span><span class="sxs-lookup"><span data-stu-id="65ba1-162">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="65ba1-163">isActive</span><span class="sxs-lookup"><span data-stu-id="65ba1-163">isActive</span></span>|<span data-ttu-id="65ba1-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="65ba1-164">Boolean</span></span>|<span data-ttu-id="65ba1-165">Используется для отключения индикаторов в системе.</span><span class="sxs-lookup"><span data-stu-id="65ba1-165">Used to deactivate indicators within system.</span></span> <span data-ttu-id="65ba1-166">По умолчанию все отправленные индикаторы задаются как активные.</span><span class="sxs-lookup"><span data-stu-id="65ba1-166">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="65ba1-167">Однако поставщики могут отсылать существующие индикаторы с этим набором в значение false, чтобы отключить индикаторы в системе.</span><span class="sxs-lookup"><span data-stu-id="65ba1-167">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="65ba1-168">киллчаин</span><span class="sxs-lookup"><span data-stu-id="65ba1-168">killChain</span></span>|<span data-ttu-id="65ba1-169">Коллекция [киллчаин](#killchain-values)</span><span class="sxs-lookup"><span data-stu-id="65ba1-169">[killChain](#killchain-values) collection</span></span>|<span data-ttu-id="65ba1-170">Массив строк JSON, указывающий, какая точка или точки в цепочке аннулирования этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="65ba1-170">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="65ba1-171">Точные значения приведены в разделе "значения Киллчаин".</span><span class="sxs-lookup"><span data-stu-id="65ba1-171">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="65ba1-172">кновнфалсепоситивес</span><span class="sxs-lookup"><span data-stu-id="65ba1-172">knownFalsePositives</span></span>|<span data-ttu-id="65ba1-173">String</span><span class="sxs-lookup"><span data-stu-id="65ba1-173">String</span></span>|<span data-ttu-id="65ba1-174">Сценарии, в которых индикатор может вызывать ложные срабатывания.</span><span class="sxs-lookup"><span data-stu-id="65ba1-174">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="65ba1-175">Это должен быть понятный для человека текст.</span><span class="sxs-lookup"><span data-stu-id="65ba1-175">This should be human-readable text.</span></span>|
|<span data-ttu-id="65ba1-176">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="65ba1-176">lastReportedDateTime</span></span>|<span data-ttu-id="65ba1-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65ba1-177">DateTimeOffset</span></span>|<span data-ttu-id="65ba1-178">Время последнего рассмотрения индикатора.</span><span class="sxs-lookup"><span data-stu-id="65ba1-178">The last time the indicator was seen.</span></span> <span data-ttu-id="65ba1-179">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="65ba1-179">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="65ba1-180">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="65ba1-180">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="65ba1-181">малварефамилинамес</span><span class="sxs-lookup"><span data-stu-id="65ba1-181">malwareFamilyNames</span></span>|<span data-ttu-id="65ba1-182">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65ba1-182">String collection</span></span>|<span data-ttu-id="65ba1-183">Имя семейства вредоносных программ, связанное с индикатором, если оно существует.</span><span class="sxs-lookup"><span data-stu-id="65ba1-183">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="65ba1-184">Корпорация Майкрософт применяет имя семейства вредоносных программ (Майкрософт), если это возможно, то, что можно найти с помощью [энциклопедии](https://www.microsoft.com/wdsi/threats)по системе безопасности защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="65ba1-184">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="65ba1-185">пассивеонли</span><span class="sxs-lookup"><span data-stu-id="65ba1-185">passiveOnly</span></span>|<span data-ttu-id="65ba1-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="65ba1-186">Boolean</span></span>|<span data-ttu-id="65ba1-187">Определяет, должен ли индикатор инициировать событие, видимое конечному пользователю.</span><span class="sxs-lookup"><span data-stu-id="65ba1-187">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="65ba1-188">Если задано значение true, средства безопасности не уведомляют конечного пользователя о выполнении "попадания".</span><span class="sxs-lookup"><span data-stu-id="65ba1-188">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="65ba1-189">Чаще всего это рассматривается как аудит или тихий режим по продуктам безопасности, в котором они просто зарегистрируются, но не будут выполнять действие.</span><span class="sxs-lookup"><span data-stu-id="65ba1-189">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="65ba1-190">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="65ba1-190">Default value is false.</span></span>|
|<span data-ttu-id="65ba1-191">severity</span><span class="sxs-lookup"><span data-stu-id="65ba1-191">severity</span></span>|<span data-ttu-id="65ba1-192">Int32</span><span class="sxs-lookup"><span data-stu-id="65ba1-192">Int32</span></span>|<span data-ttu-id="65ba1-193">Целое число, представляющее серьезность вредоносного поведения, идентифицируемого данными в индикаторе.</span><span class="sxs-lookup"><span data-stu-id="65ba1-193">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="65ba1-194">Допустимые значения: 0 – 5, где 5 — самый серьезный, а ноль — нет.</span><span class="sxs-lookup"><span data-stu-id="65ba1-194">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="65ba1-195">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="65ba1-195">Default value is 3.</span></span>|
|<span data-ttu-id="65ba1-196">tags</span><span class="sxs-lookup"><span data-stu-id="65ba1-196">tags</span></span>|<span data-ttu-id="65ba1-197">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="65ba1-197">String collection</span></span>|<span data-ttu-id="65ba1-198">Массив строк JSON, в котором хранятся произвольные Теги и ключевые слова.</span><span class="sxs-lookup"><span data-stu-id="65ba1-198">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="65ba1-199">тлплевел</span><span class="sxs-lookup"><span data-stu-id="65ba1-199">tlpLevel</span></span>|[<span data-ttu-id="65ba1-200">тлплевел</span><span class="sxs-lookup"><span data-stu-id="65ba1-200">tlpLevel</span></span>](#tlplevel-values)| <span data-ttu-id="65ba1-201">Значение протокола светофора для индикатора.</span><span class="sxs-lookup"><span data-stu-id="65ba1-201">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="65ba1-202">Возможные значения: `unknown`, `white`, `green`, `amber`, `red`.</span><span class="sxs-lookup"><span data-stu-id="65ba1-202">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="65ba1-203">значения Диамондмодел</span><span class="sxs-lookup"><span data-stu-id="65ba1-203">diamondModel values</span></span>

<span data-ttu-id="65ba1-204">Сведения об этой модели можно найти [в разделе Модель ромба](http://diamondmodel.org).</span><span class="sxs-lookup"><span data-stu-id="65ba1-204">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="65ba1-205">Значения</span><span class="sxs-lookup"><span data-stu-id="65ba1-205">Values</span></span> | <span data-ttu-id="65ba1-206">Описание</span><span class="sxs-lookup"><span data-stu-id="65ba1-206">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="65ba1-207">Злоумышленник</span><span class="sxs-lookup"><span data-stu-id="65ba1-207">adversary</span></span>|<span data-ttu-id="65ba1-208">Индикатор описывает.</span><span class="sxs-lookup"><span data-stu-id="65ba1-208">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="65ba1-209">поставлен</span><span class="sxs-lookup"><span data-stu-id="65ba1-209">capability</span></span>|<span data-ttu-id="65ba1-210">Индикатор является возможностью злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="65ba1-210">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="65ba1-211">инфраструктур</span><span class="sxs-lookup"><span data-stu-id="65ba1-211">infrastructure</span></span>|<span data-ttu-id="65ba1-212">Индикатор описывает инфраструктуру злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="65ba1-212">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="65ba1-213">стала</span><span class="sxs-lookup"><span data-stu-id="65ba1-213">victim</span></span>|<span data-ttu-id="65ba1-214">Индикатор описывает жертвой злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="65ba1-214">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="65ba1-215">значения Киллчаин</span><span class="sxs-lookup"><span data-stu-id="65ba1-215">killChain values</span></span>

| <span data-ttu-id="65ba1-216">Значения</span><span class="sxs-lookup"><span data-stu-id="65ba1-216">Values</span></span> | <span data-ttu-id="65ba1-217">Описание</span><span class="sxs-lookup"><span data-stu-id="65ba1-217">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="65ba1-218">Действия</span><span class="sxs-lookup"><span data-stu-id="65ba1-218">Actions</span></span>|<span data-ttu-id="65ba1-219">Представляет "действия по целям".</span><span class="sxs-lookup"><span data-stu-id="65ba1-219">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="65ba1-220">Злоумышленник получает такие действия, как распределенная атака типа "отказ в обслуживании".</span><span class="sxs-lookup"><span data-stu-id="65ba1-220">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="65ba1-221">C2</span><span class="sxs-lookup"><span data-stu-id="65ba1-221">C2</span></span>|<span data-ttu-id="65ba1-222">Представляет канал управления, с которым работает скомпрометированная система.</span><span class="sxs-lookup"><span data-stu-id="65ba1-222">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="65ba1-223">Delivery</span><span class="sxs-lookup"><span data-stu-id="65ba1-223">Delivery</span></span>|<span data-ttu-id="65ba1-224">Процесс распространения кода эксплойта для жертв (например, USB, электронной почты, веб-сайтов).</span><span class="sxs-lookup"><span data-stu-id="65ba1-224">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="65ba1-225">Опасность</span><span class="sxs-lookup"><span data-stu-id="65ba1-225">Exploitation</span></span>|<span data-ttu-id="65ba1-226">Код эксплойта использует преимущества уязвимостей (например, выполнение кода).</span><span class="sxs-lookup"><span data-stu-id="65ba1-226">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="65ba1-227">Установка</span><span class="sxs-lookup"><span data-stu-id="65ba1-227">Installation</span></span>|<span data-ttu-id="65ba1-228">Установка вредоносных программ после использования уязвимости.</span><span class="sxs-lookup"><span data-stu-id="65ba1-228">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="65ba1-229">реконнаиссанце</span><span class="sxs-lookup"><span data-stu-id="65ba1-229">Reconnaissance</span></span>|<span data-ttu-id="65ba1-230">Индикатор — это свидетельство того, что Группа действий получает сведения, которые будут использоваться при следующей атаке.</span><span class="sxs-lookup"><span data-stu-id="65ba1-230">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="65ba1-231">веапонизатион</span><span class="sxs-lookup"><span data-stu-id="65ba1-231">Weaponization</span></span>|<span data-ttu-id="65ba1-232">Включение уязвимости в код эксплойта (например, вредоносные программы).</span><span class="sxs-lookup"><span data-stu-id="65ba1-232">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="65ba1-233">значения Тлплевел</span><span class="sxs-lookup"><span data-stu-id="65ba1-233">tlpLevel values</span></span>

<span data-ttu-id="65ba1-234">При отправке каждого индикатора должен быть задано значение протокола светофора (ТЛП).</span><span class="sxs-lookup"><span data-stu-id="65ba1-234">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="65ba1-235">Это значение представляет собой чувствительность и область общего доступа к заданному индикатору.</span><span class="sxs-lookup"><span data-stu-id="65ba1-235">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="65ba1-236">Значения</span><span class="sxs-lookup"><span data-stu-id="65ba1-236">Values</span></span> | <span data-ttu-id="65ba1-237">Описание</span><span class="sxs-lookup"><span data-stu-id="65ba1-237">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="65ba1-238">Белый</span><span class="sxs-lookup"><span data-stu-id="65ba1-238">White</span></span>| <span data-ttu-id="65ba1-239">Область общего доступа: unlimited.</span><span class="sxs-lookup"><span data-stu-id="65ba1-239">Sharing scope: Unlimited.</span></span> <span data-ttu-id="65ba1-240">Индикаторы могут быть предоставлены бесплатно, без ограничений.</span><span class="sxs-lookup"><span data-stu-id="65ba1-240">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="65ba1-241">Зеленый</span><span class="sxs-lookup"><span data-stu-id="65ba1-241">Green</span></span>| <span data-ttu-id="65ba1-242">Область общего доступа: сообщество.</span><span class="sxs-lookup"><span data-stu-id="65ba1-242">Sharing scope: Community.</span></span> <span data-ttu-id="65ba1-243">С помощью сообщества безопасности можно предоставить доступ к индикаторам.</span><span class="sxs-lookup"><span data-stu-id="65ba1-243">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="65ba1-244">Оранжевого</span><span class="sxs-lookup"><span data-stu-id="65ba1-244">Amber</span></span>| <span data-ttu-id="65ba1-245">Область общего доступа: ограничена.</span><span class="sxs-lookup"><span data-stu-id="65ba1-245">Sharing scope: Limited.</span></span> <span data-ttu-id="65ba1-246">Это параметр по умолчанию для индикаторов и разрешает совместное использование только тем, у которых есть ненужные: 1) службы и операторы служб, реализующие логику операций с угрозами; 2) клиенты, чьи системы соответствуют поведению с индикатором.</span><span class="sxs-lookup"><span data-stu-id="65ba1-246">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="65ba1-247">Красный</span><span class="sxs-lookup"><span data-stu-id="65ba1-247">Red</span></span>| <span data-ttu-id="65ba1-248">Область общего доступа: личная.</span><span class="sxs-lookup"><span data-stu-id="65ba1-248">Sharing scope: Personal.</span></span> <span data-ttu-id="65ba1-249">Эти индикаторы предназначены только для предоставления доступа напрямую и, желательно, в случае человека.</span><span class="sxs-lookup"><span data-stu-id="65ba1-249">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="65ba1-250">Как правило, ТЛП красные индикаторы не отправляются из-за ограничений, заданных ранее.</span><span class="sxs-lookup"><span data-stu-id="65ba1-250">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="65ba1-251">Если отправляются красные индикаторы ТЛП, свойству **пассивеонли** следует присвоить значение `True` также.</span><span class="sxs-lookup"><span data-stu-id="65ba1-251">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="65ba1-252">Ответ</span><span class="sxs-lookup"><span data-stu-id="65ba1-252">Response</span></span>

<span data-ttu-id="65ba1-253">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="65ba1-253">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="65ba1-254">Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65ba1-254">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65ba1-255">Примеры</span><span class="sxs-lookup"><span data-stu-id="65ba1-255">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="65ba1-256">Пример 1: запрос без верхнего колонтитула</span><span class="sxs-lookup"><span data-stu-id="65ba1-256">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="65ba1-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="65ba1-257">Request</span></span>

<span data-ttu-id="65ba1-258">Ниже приведен пример запроса без `Prefer` заголовка.</span><span class="sxs-lookup"><span data-stu-id="65ba1-258">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="65ba1-259">HTTP</span><span class="sxs-lookup"><span data-stu-id="65ba1-259">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="65ba1-260">C#</span><span class="sxs-lookup"><span data-stu-id="65ba1-260">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65ba1-261">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65ba1-261">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65ba1-262">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65ba1-262">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65ba1-263">Отклик</span><span class="sxs-lookup"><span data-stu-id="65ba1-263">Response</span></span>

<span data-ttu-id="65ba1-264">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="65ba1-264">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="65ba1-265">Пример 2: запрос с заголовком предпочтения</span><span class="sxs-lookup"><span data-stu-id="65ba1-265">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="65ba1-266">Запрос</span><span class="sxs-lookup"><span data-stu-id="65ba1-266">Request</span></span>

<span data-ttu-id="65ba1-267">Ниже приведен пример запроса, включающего `Prefer` заголовок.</span><span class="sxs-lookup"><span data-stu-id="65ba1-267">The following is an example of the request that includes the `Prefer` header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="65ba1-268">Отклик</span><span class="sxs-lookup"><span data-stu-id="65ba1-268">Response</span></span>

<span data-ttu-id="65ba1-269">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="65ba1-269">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="65ba1-270">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="65ba1-270">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="65ba1-271">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65ba1-271">All the properties will be returned from an actual call.</span></span>

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

---
title: Обновление объекта tiIndicator
description: Обновление свойств объекта Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 75a34acb98ee00e737fb75e5e49f7c0fb4adea20
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637572"
---
# <a name="update-tiindicator"></a><span data-ttu-id="4a59e-103">Обновление объекта tiIndicator</span><span class="sxs-lookup"><span data-stu-id="4a59e-103">Update tiIndicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a59e-104">Обновление свойств объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="4a59e-104">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a59e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a59e-105">Permissions</span></span>

<span data-ttu-id="4a59e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a59e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a59e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a59e-108">Permission type</span></span>                        | <span data-ttu-id="4a59e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a59e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4a59e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a59e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a59e-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="4a59e-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="4a59e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a59e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a59e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a59e-113">Not supported.</span></span> |
| <span data-ttu-id="4a59e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a59e-114">Application</span></span>                            | <span data-ttu-id="4a59e-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="4a59e-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a59e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a59e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4a59e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a59e-117">Request headers</span></span>

| <span data-ttu-id="4a59e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4a59e-118">Name</span></span>       | <span data-ttu-id="4a59e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4a59e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4a59e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a59e-120">Authorization</span></span> | <span data-ttu-id="4a59e-121">**Необходим** носитель {код}</span><span class="sxs-lookup"><span data-stu-id="4a59e-121">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="4a59e-122">Prefer</span><span class="sxs-lookup"><span data-stu-id="4a59e-122">Prefer</span></span> | <span data-ttu-id="4a59e-123">Возврат = представление</span><span class="sxs-lookup"><span data-stu-id="4a59e-123">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a59e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a59e-124">Request body</span></span>

<span data-ttu-id="4a59e-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4a59e-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4a59e-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4a59e-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4a59e-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4a59e-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4a59e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a59e-128">Property</span></span>     | <span data-ttu-id="4a59e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4a59e-129">Type</span></span>        | <span data-ttu-id="4a59e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4a59e-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a59e-131">action</span><span class="sxs-lookup"><span data-stu-id="4a59e-131">action</span></span>|<span data-ttu-id="4a59e-132">string</span><span class="sxs-lookup"><span data-stu-id="4a59e-132">string</span></span>| <span data-ttu-id="4a59e-133">Действие, которое необходимо применить, если индикатор сопоставлен с помощью средства безопасности Таржетпродукт.</span><span class="sxs-lookup"><span data-stu-id="4a59e-133">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="4a59e-134">Возможные значения: `unknown`, `allow`, `block`, `alert`.</span><span class="sxs-lookup"><span data-stu-id="4a59e-134">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="4a59e-135">Активитиграупнамес</span><span class="sxs-lookup"><span data-stu-id="4a59e-135">activityGroupNames</span></span>|<span data-ttu-id="4a59e-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4a59e-136">String collection</span></span>|<span data-ttu-id="4a59e-137">Имя (-ы) логики операций с угрозами кибератак для сторон, ответственных за вредоносные действия, охваченные индикатором угроз.</span><span class="sxs-lookup"><span data-stu-id="4a59e-137">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="4a59e-138">Аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="4a59e-138">additionalInformation</span></span>|<span data-ttu-id="4a59e-139">String</span><span class="sxs-lookup"><span data-stu-id="4a59e-139">String</span></span>|<span data-ttu-id="4a59e-140">Область общего пользования, в которую могут быть размещены дополнительные данные из индикатора, не охваченные другими свойствами Тииндикатор.</span><span class="sxs-lookup"><span data-stu-id="4a59e-140">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="4a59e-141">Данные, помещаемые в Аддитионалинформатион, обычно не используются средством безопасности Таржетпродукт.</span><span class="sxs-lookup"><span data-stu-id="4a59e-141">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="4a59e-142">confidence</span><span class="sxs-lookup"><span data-stu-id="4a59e-142">confidence</span></span>|<span data-ttu-id="4a59e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4a59e-143">Int32</span></span>|<span data-ttu-id="4a59e-144">Целое число, представляющее достоверность, с помощью которой данные в индикаторе точно определяют вредоносное поведение.</span><span class="sxs-lookup"><span data-stu-id="4a59e-144">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="4a59e-145">Допустимые значения: 0 – 100 с 100 по убыванию.</span><span class="sxs-lookup"><span data-stu-id="4a59e-145">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="4a59e-146">description</span><span class="sxs-lookup"><span data-stu-id="4a59e-146">description</span></span>|<span data-ttu-id="4a59e-147">String</span><span class="sxs-lookup"><span data-stu-id="4a59e-147">String</span></span>|<span data-ttu-id="4a59e-148">Краткое описание угрозы, представленное индикатором (100 символов или меньше).</span><span class="sxs-lookup"><span data-stu-id="4a59e-148">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="4a59e-149">Диамондмодел</span><span class="sxs-lookup"><span data-stu-id="4a59e-149">diamondModel</span></span>|[<span data-ttu-id="4a59e-150">Диамондмодел</span><span class="sxs-lookup"><span data-stu-id="4a59e-150">diamondModel</span></span>](#diamondmodel-values)|<span data-ttu-id="4a59e-151">Область модели ромба, в которой существует этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="4a59e-151">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="4a59e-152">Возможные значения: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span><span class="sxs-lookup"><span data-stu-id="4a59e-152">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="4a59e-153">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4a59e-153">expirationDateTime</span></span>|<span data-ttu-id="4a59e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a59e-154">DateTimeOffset</span></span>| <span data-ttu-id="4a59e-155">Строка DateTime, указывающая, когда истечет срок действия индикатора.</span><span class="sxs-lookup"><span data-stu-id="4a59e-155">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="4a59e-156">Все индикаторы должны иметь дату истечения срока действия, чтобы не допустить устаревших показателей в системе.</span><span class="sxs-lookup"><span data-stu-id="4a59e-156">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="4a59e-157">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4a59e-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4a59e-158">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4a59e-158">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="4a59e-159">externalId</span><span class="sxs-lookup"><span data-stu-id="4a59e-159">externalId</span></span>|<span data-ttu-id="4a59e-160">String</span><span class="sxs-lookup"><span data-stu-id="4a59e-160">String</span></span>|<span data-ttu-id="4a59e-161">Идентификационный номер, который привязывает индикатор к системе поставщика индикаторов (например, внешнему ключу).</span><span class="sxs-lookup"><span data-stu-id="4a59e-161">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="4a59e-162">isActive</span><span class="sxs-lookup"><span data-stu-id="4a59e-162">isActive</span></span>|<span data-ttu-id="4a59e-163">Логический</span><span class="sxs-lookup"><span data-stu-id="4a59e-163">Boolean</span></span>|<span data-ttu-id="4a59e-164">Используется для отключения индикаторов в системе.</span><span class="sxs-lookup"><span data-stu-id="4a59e-164">Used to deactivate indicators within system.</span></span> <span data-ttu-id="4a59e-165">По умолчанию все отправленные индикаторы задаются как активные.</span><span class="sxs-lookup"><span data-stu-id="4a59e-165">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="4a59e-166">Однако поставщики могут отсылать существующие индикаторы с этим набором в значение false, чтобы отключить индикаторы в системе.</span><span class="sxs-lookup"><span data-stu-id="4a59e-166">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="4a59e-167">Киллчаин</span><span class="sxs-lookup"><span data-stu-id="4a59e-167">killChain</span></span>|<span data-ttu-id="4a59e-168">Коллекция [киллчаин](#killchain-values)</span><span class="sxs-lookup"><span data-stu-id="4a59e-168">[killChain](#killchain-values) collection</span></span>|<span data-ttu-id="4a59e-169">Массив строк JSON, указывающий, какая точка или точки в цепочке аннулирования этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="4a59e-169">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="4a59e-170">Точные значения приведены в разделе "значения Киллчаин".</span><span class="sxs-lookup"><span data-stu-id="4a59e-170">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="4a59e-171">Кновнфалсепоситивес</span><span class="sxs-lookup"><span data-stu-id="4a59e-171">knownFalsePositives</span></span>|<span data-ttu-id="4a59e-172">String</span><span class="sxs-lookup"><span data-stu-id="4a59e-172">String</span></span>|<span data-ttu-id="4a59e-173">Сценарии, в которых индикатор может вызывать ложные срабатывания.</span><span class="sxs-lookup"><span data-stu-id="4a59e-173">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="4a59e-174">Это должен быть понятный для человека текст.</span><span class="sxs-lookup"><span data-stu-id="4a59e-174">This should be human-readable text.</span></span>|
|<span data-ttu-id="4a59e-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a59e-175">lastReportedDateTime</span></span>|<span data-ttu-id="4a59e-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a59e-176">DateTimeOffset</span></span>|<span data-ttu-id="4a59e-177">Время последнего рассмотрения индикатора.</span><span class="sxs-lookup"><span data-stu-id="4a59e-177">The last time the indicator was seen.</span></span> <span data-ttu-id="4a59e-178">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4a59e-178">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4a59e-179">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4a59e-179">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="4a59e-180">Малварефамилинамес</span><span class="sxs-lookup"><span data-stu-id="4a59e-180">malwareFamilyNames</span></span>|<span data-ttu-id="4a59e-181">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4a59e-181">String collection</span></span>|<span data-ttu-id="4a59e-182">Имя семейства вредоносных программ, связанное с индикатором, если оно существует.</span><span class="sxs-lookup"><span data-stu-id="4a59e-182">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="4a59e-183">Корпорация Майкрософт применяет имя семейства вредоносных программ (Майкрософт), если это возможно, то, что можно [](https://www.microsoft.com/wdsi/threats)найти с помощью энциклопедии по системе безопасности защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="4a59e-183">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="4a59e-184">Пассивеонли</span><span class="sxs-lookup"><span data-stu-id="4a59e-184">passiveOnly</span></span>|<span data-ttu-id="4a59e-185">Логический</span><span class="sxs-lookup"><span data-stu-id="4a59e-185">Boolean</span></span>|<span data-ttu-id="4a59e-186">Определяет, должен ли индикатор инициировать событие, видимое конечному пользователю.</span><span class="sxs-lookup"><span data-stu-id="4a59e-186">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="4a59e-187">Если задано значение true, средства безопасности не уведомляют конечного пользователя о выполнении "попадания".</span><span class="sxs-lookup"><span data-stu-id="4a59e-187">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="4a59e-188">Чаще всего это рассматривается как аудит или тихий режим по продуктам безопасности, в котором они просто зарегистрируются, но не будут выполнять действие.</span><span class="sxs-lookup"><span data-stu-id="4a59e-188">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="4a59e-189">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="4a59e-189">Default value is false.</span></span>|
|<span data-ttu-id="4a59e-190">severity</span><span class="sxs-lookup"><span data-stu-id="4a59e-190">severity</span></span>|<span data-ttu-id="4a59e-191">Int32</span><span class="sxs-lookup"><span data-stu-id="4a59e-191">Int32</span></span>|<span data-ttu-id="4a59e-192">Целое число, представляющее серьезность вредоносного поведения, идентифицируемого данными в индикаторе.</span><span class="sxs-lookup"><span data-stu-id="4a59e-192">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="4a59e-193">Допустимые значения: 0 – 5, где 5 — самый серьезный, а ноль — нет.</span><span class="sxs-lookup"><span data-stu-id="4a59e-193">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="4a59e-194">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="4a59e-194">Default value is 3.</span></span>|
|<span data-ttu-id="4a59e-195">tags</span><span class="sxs-lookup"><span data-stu-id="4a59e-195">tags</span></span>|<span data-ttu-id="4a59e-196">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4a59e-196">String collection</span></span>|<span data-ttu-id="4a59e-197">Массив строк JSON, В котором хранятся произвольные Теги и ключевые слова.</span><span class="sxs-lookup"><span data-stu-id="4a59e-197">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="4a59e-198">Тлплевел</span><span class="sxs-lookup"><span data-stu-id="4a59e-198">tlpLevel</span></span>|[<span data-ttu-id="4a59e-199">Тлплевел</span><span class="sxs-lookup"><span data-stu-id="4a59e-199">tlpLevel</span></span>](#tlplevel-values)| <span data-ttu-id="4a59e-200">Значение протокола светофора для индикатора.</span><span class="sxs-lookup"><span data-stu-id="4a59e-200">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="4a59e-201">Возможные значения: `unknown`, `white`, `green`, `amber`, `red`.</span><span class="sxs-lookup"><span data-stu-id="4a59e-201">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="4a59e-202">значения Диамондмодел</span><span class="sxs-lookup"><span data-stu-id="4a59e-202">diamondModel values</span></span>

<span data-ttu-id="4a59e-203">Сведения об этой модели можно найти [в разделе Модель ромба](http://diamondmodel.org).</span><span class="sxs-lookup"><span data-stu-id="4a59e-203">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="4a59e-204">Значения</span><span class="sxs-lookup"><span data-stu-id="4a59e-204">Values</span></span> | <span data-ttu-id="4a59e-205">Описание</span><span class="sxs-lookup"><span data-stu-id="4a59e-205">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="4a59e-206">Злоумышленник</span><span class="sxs-lookup"><span data-stu-id="4a59e-206">adversary</span></span>|<span data-ttu-id="4a59e-207">Индикатор описывает.</span><span class="sxs-lookup"><span data-stu-id="4a59e-207">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="4a59e-208">поставлен</span><span class="sxs-lookup"><span data-stu-id="4a59e-208">capability</span></span>|<span data-ttu-id="4a59e-209">Индикатор является возможностью злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="4a59e-209">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="4a59e-210">инфраструктур</span><span class="sxs-lookup"><span data-stu-id="4a59e-210">infrastructure</span></span>|<span data-ttu-id="4a59e-211">Индикатор описывает инфраструктуру злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="4a59e-211">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="4a59e-212">стала</span><span class="sxs-lookup"><span data-stu-id="4a59e-212">victim</span></span>|<span data-ttu-id="4a59e-213">Индикатор описывает жертвой злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="4a59e-213">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="4a59e-214">значения Киллчаин</span><span class="sxs-lookup"><span data-stu-id="4a59e-214">killChain values</span></span>

| <span data-ttu-id="4a59e-215">Значения</span><span class="sxs-lookup"><span data-stu-id="4a59e-215">Values</span></span> | <span data-ttu-id="4a59e-216">Описание</span><span class="sxs-lookup"><span data-stu-id="4a59e-216">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="4a59e-217">Действия</span><span class="sxs-lookup"><span data-stu-id="4a59e-217">Actions</span></span>|<span data-ttu-id="4a59e-218">Представляет "действия по целям".</span><span class="sxs-lookup"><span data-stu-id="4a59e-218">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="4a59e-219">Злоумышленник получает такие действия, как распределенная атака типа "отказ в обслуживании".</span><span class="sxs-lookup"><span data-stu-id="4a59e-219">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="4a59e-220">C2</span><span class="sxs-lookup"><span data-stu-id="4a59e-220">C2</span></span>|<span data-ttu-id="4a59e-221">Представляет канал управления, с которым работает скомпрометированная система.</span><span class="sxs-lookup"><span data-stu-id="4a59e-221">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="4a59e-222">Delivery</span><span class="sxs-lookup"><span data-stu-id="4a59e-222">Delivery</span></span>|<span data-ttu-id="4a59e-223">Процесс распространения кода эксплойта для жертв (например, USB, электронной почты, веб-сайтов).</span><span class="sxs-lookup"><span data-stu-id="4a59e-223">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="4a59e-224">Опасность</span><span class="sxs-lookup"><span data-stu-id="4a59e-224">Exploitation</span></span>|<span data-ttu-id="4a59e-225">Код эксплойта использует преимущества уязвимостей (например, выполнение кода).</span><span class="sxs-lookup"><span data-stu-id="4a59e-225">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="4a59e-226">Установка</span><span class="sxs-lookup"><span data-stu-id="4a59e-226">Installation</span></span>|<span data-ttu-id="4a59e-227">Установка вредоносных программ после использования уязвимости.</span><span class="sxs-lookup"><span data-stu-id="4a59e-227">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="4a59e-228">Реконнаиссанце</span><span class="sxs-lookup"><span data-stu-id="4a59e-228">Reconnaissance</span></span>|<span data-ttu-id="4a59e-229">Индикатор — это свидетельство того, что Группа действий получает сведения, которые будут использоваться при следующей атаке.</span><span class="sxs-lookup"><span data-stu-id="4a59e-229">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="4a59e-230">Веапонизатион</span><span class="sxs-lookup"><span data-stu-id="4a59e-230">Weaponization</span></span>|<span data-ttu-id="4a59e-231">Включение уязвимости в код эксплойта (например, вредоносные программы).</span><span class="sxs-lookup"><span data-stu-id="4a59e-231">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="4a59e-232">значения Тлплевел</span><span class="sxs-lookup"><span data-stu-id="4a59e-232">tlpLevel values</span></span>

<span data-ttu-id="4a59e-233">При отправке каждого индикатора должен быть задано значение протокола светофора (ТЛП).</span><span class="sxs-lookup"><span data-stu-id="4a59e-233">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="4a59e-234">Это значение представляет собой чувствительность и область общего доступа к заданному индикатору.</span><span class="sxs-lookup"><span data-stu-id="4a59e-234">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="4a59e-235">Значения</span><span class="sxs-lookup"><span data-stu-id="4a59e-235">Values</span></span> | <span data-ttu-id="4a59e-236">Описание</span><span class="sxs-lookup"><span data-stu-id="4a59e-236">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="4a59e-237">Белый</span><span class="sxs-lookup"><span data-stu-id="4a59e-237">White</span></span>| <span data-ttu-id="4a59e-238">Область общего доступа: unlimited.</span><span class="sxs-lookup"><span data-stu-id="4a59e-238">Sharing scope: Unlimited.</span></span> <span data-ttu-id="4a59e-239">Индикаторы могут быть предоставлены бесплатно, без ограничений.</span><span class="sxs-lookup"><span data-stu-id="4a59e-239">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="4a59e-240">Зеленый</span><span class="sxs-lookup"><span data-stu-id="4a59e-240">Green</span></span>| <span data-ttu-id="4a59e-241">Область общего доступа: сообщество.</span><span class="sxs-lookup"><span data-stu-id="4a59e-241">Sharing scope: Community.</span></span> <span data-ttu-id="4a59e-242">С помощью сообщества безопасности можно предоставить доступ к индикаторам.</span><span class="sxs-lookup"><span data-stu-id="4a59e-242">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="4a59e-243">Оранжевого</span><span class="sxs-lookup"><span data-stu-id="4a59e-243">Amber</span></span>| <span data-ttu-id="4a59e-244">Область общего доступа: ограничена.</span><span class="sxs-lookup"><span data-stu-id="4a59e-244">Sharing scope: Limited.</span></span> <span data-ttu-id="4a59e-245">Это параметр по умолчанию для индикаторов и разрешает совместное использование только тем, у которых есть ненужные: 1) службы и операторы служб, реализующие логику операций с угрозами; 2) клиенты, чьи системы соответствуют поведению с индикатором.</span><span class="sxs-lookup"><span data-stu-id="4a59e-245">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="4a59e-246">Красный</span><span class="sxs-lookup"><span data-stu-id="4a59e-246">Red</span></span>| <span data-ttu-id="4a59e-247">Область общего доступа: личная.</span><span class="sxs-lookup"><span data-stu-id="4a59e-247">Sharing scope: Personal.</span></span> <span data-ttu-id="4a59e-248">Эти индикаторы предназначены только для предоставления доступа напрямую и, желательно, в случае человека.</span><span class="sxs-lookup"><span data-stu-id="4a59e-248">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="4a59e-249">Как правило, ТЛП красные индикаторы не отправляются из-за ограничений, заданных ранее.</span><span class="sxs-lookup"><span data-stu-id="4a59e-249">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="4a59e-250">Если отправляются красные индикаторы ТЛП, свойству **пассивеонли** следует присвоить значение `True` также.</span><span class="sxs-lookup"><span data-stu-id="4a59e-250">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="4a59e-251">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a59e-251">Response</span></span>

<span data-ttu-id="4a59e-252">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4a59e-252">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="4a59e-253">Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [тииндикатор](../resources/tiIndicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a59e-253">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiIndicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a59e-254">Примеры</span><span class="sxs-lookup"><span data-stu-id="4a59e-254">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="4a59e-255">Пример 1: запрос без верхнего колонтитула</span><span class="sxs-lookup"><span data-stu-id="4a59e-255">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="4a59e-256">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a59e-256">Request</span></span>

<span data-ttu-id="4a59e-257">Ниже приведен пример запроса без `Prefer` заголовка.</span><span class="sxs-lookup"><span data-stu-id="4a59e-257">The following is an example of the request without the `Prefer` header.</span></span>
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

#### <a name="response"></a><span data-ttu-id="4a59e-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a59e-258">Response</span></span>

<span data-ttu-id="4a59e-259">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a59e-259">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4a59e-260">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="4a59e-260">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4a59e-261">Языках</span><span class="sxs-lookup"><span data-stu-id="4a59e-261">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_tiIndicator-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a59e-262">Язык</span><span class="sxs-lookup"><span data-stu-id="4a59e-262">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_tiIndicator-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="4a59e-263">Пример 2: запрос с заголовком предпочтения</span><span class="sxs-lookup"><span data-stu-id="4a59e-263">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="4a59e-264">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a59e-264">Request</span></span>

<span data-ttu-id="4a59e-265">Ниже приведен пример запроса, включающего `Prefer` заголовок.</span><span class="sxs-lookup"><span data-stu-id="4a59e-265">The following is an example of the request that includes the `Prefer` header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="4a59e-266">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a59e-266">Response</span></span>

<span data-ttu-id="4a59e-267">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a59e-267">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4a59e-268">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4a59e-268">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4a59e-269">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a59e-269">All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/tiindicator-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/tiindicator-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

---
title: Обновление объекта tiIndicator
description: Обновление свойств объекта Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e19213c34730d42bd133ae446c02b182865f5f70
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457956"
---
# <a name="update-tiindicator"></a><span data-ttu-id="577bb-103">Обновление объекта tiIndicator</span><span class="sxs-lookup"><span data-stu-id="577bb-103">Update tiIndicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="577bb-104">Обновление свойств объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="577bb-104">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="577bb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="577bb-105">Permissions</span></span>

<span data-ttu-id="577bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="577bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="577bb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="577bb-108">Permission type</span></span>                        | <span data-ttu-id="577bb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="577bb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="577bb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="577bb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="577bb-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="577bb-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="577bb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="577bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="577bb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="577bb-113">Not supported.</span></span> |
| <span data-ttu-id="577bb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="577bb-114">Application</span></span>                            | <span data-ttu-id="577bb-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="577bb-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="577bb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="577bb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="577bb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="577bb-117">Request headers</span></span>

| <span data-ttu-id="577bb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="577bb-118">Name</span></span>       | <span data-ttu-id="577bb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="577bb-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="577bb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="577bb-120">Authorization</span></span> | <span data-ttu-id="577bb-121">**Необходим** носитель {код}</span><span class="sxs-lookup"><span data-stu-id="577bb-121">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="577bb-122">Prefer</span><span class="sxs-lookup"><span data-stu-id="577bb-122">Prefer</span></span> | <span data-ttu-id="577bb-123">Возврат = представление</span><span class="sxs-lookup"><span data-stu-id="577bb-123">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="577bb-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="577bb-124">Request body</span></span>

<span data-ttu-id="577bb-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="577bb-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="577bb-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="577bb-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="577bb-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="577bb-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="577bb-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="577bb-128">Property</span></span>     | <span data-ttu-id="577bb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="577bb-129">Type</span></span>        | <span data-ttu-id="577bb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="577bb-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="577bb-131">action</span><span class="sxs-lookup"><span data-stu-id="577bb-131">action</span></span>|<span data-ttu-id="577bb-132">string</span><span class="sxs-lookup"><span data-stu-id="577bb-132">string</span></span>| <span data-ttu-id="577bb-133">Действие, которое необходимо применить, если индикатор сопоставлен с помощью средства безопасности Таржетпродукт.</span><span class="sxs-lookup"><span data-stu-id="577bb-133">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="577bb-134">Возможные значения: `unknown`, `allow`, `block`, `alert`.</span><span class="sxs-lookup"><span data-stu-id="577bb-134">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="577bb-135">Активитиграупнамес</span><span class="sxs-lookup"><span data-stu-id="577bb-135">activityGroupNames</span></span>|<span data-ttu-id="577bb-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="577bb-136">String collection</span></span>|<span data-ttu-id="577bb-137">Имя (-ы) логики операций с угрозами кибератак для сторон, ответственных за вредоносные действия, охваченные индикатором угроз.</span><span class="sxs-lookup"><span data-stu-id="577bb-137">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="577bb-138">Аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="577bb-138">additionalInformation</span></span>|<span data-ttu-id="577bb-139">String</span><span class="sxs-lookup"><span data-stu-id="577bb-139">String</span></span>|<span data-ttu-id="577bb-140">Область общего пользования, в которую могут быть размещены дополнительные данные из индикатора, не охваченные другими свойствами Тииндикатор.</span><span class="sxs-lookup"><span data-stu-id="577bb-140">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="577bb-141">Данные, помещаемые в Аддитионалинформатион, обычно не используются средством безопасности Таржетпродукт.</span><span class="sxs-lookup"><span data-stu-id="577bb-141">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="577bb-142">confidence</span><span class="sxs-lookup"><span data-stu-id="577bb-142">confidence</span></span>|<span data-ttu-id="577bb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="577bb-143">Int32</span></span>|<span data-ttu-id="577bb-144">Целое число, представляющее достоверность, с помощью которой данные в индикаторе точно определяют вредоносное поведение.</span><span class="sxs-lookup"><span data-stu-id="577bb-144">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="577bb-145">Допустимые значения: 0 – 100 с 100 по убыванию.</span><span class="sxs-lookup"><span data-stu-id="577bb-145">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="577bb-146">description</span><span class="sxs-lookup"><span data-stu-id="577bb-146">description</span></span>|<span data-ttu-id="577bb-147">String</span><span class="sxs-lookup"><span data-stu-id="577bb-147">String</span></span>|<span data-ttu-id="577bb-148">Краткое описание угрозы, представленное индикатором (100 символов или меньше).</span><span class="sxs-lookup"><span data-stu-id="577bb-148">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="577bb-149">Диамондмодел</span><span class="sxs-lookup"><span data-stu-id="577bb-149">diamondModel</span></span>|[<span data-ttu-id="577bb-150">Диамондмодел</span><span class="sxs-lookup"><span data-stu-id="577bb-150">diamondModel</span></span>](#diamondmodel-values)|<span data-ttu-id="577bb-151">Область модели ромба, в которой существует этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="577bb-151">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="577bb-152">Возможные значения: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span><span class="sxs-lookup"><span data-stu-id="577bb-152">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="577bb-153">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="577bb-153">expirationDateTime</span></span>|<span data-ttu-id="577bb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="577bb-154">DateTimeOffset</span></span>| <span data-ttu-id="577bb-155">Строка DateTime, указывающая, когда истечет срок действия индикатора.</span><span class="sxs-lookup"><span data-stu-id="577bb-155">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="577bb-156">Все индикаторы должны иметь дату истечения срока действия, чтобы не допустить устаревших показателей в системе.</span><span class="sxs-lookup"><span data-stu-id="577bb-156">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="577bb-157">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="577bb-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="577bb-158">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="577bb-158">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="577bb-159">externalId</span><span class="sxs-lookup"><span data-stu-id="577bb-159">externalId</span></span>|<span data-ttu-id="577bb-160">String</span><span class="sxs-lookup"><span data-stu-id="577bb-160">String</span></span>|<span data-ttu-id="577bb-161">Идентификационный номер, который привязывает индикатор к системе поставщика индикаторов (например, внешнему ключу).</span><span class="sxs-lookup"><span data-stu-id="577bb-161">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="577bb-162">isActive</span><span class="sxs-lookup"><span data-stu-id="577bb-162">isActive</span></span>|<span data-ttu-id="577bb-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="577bb-163">Boolean</span></span>|<span data-ttu-id="577bb-164">Используется для отключения индикаторов в системе.</span><span class="sxs-lookup"><span data-stu-id="577bb-164">Used to deactivate indicators within system.</span></span> <span data-ttu-id="577bb-165">По умолчанию все отправленные индикаторы задаются как активные.</span><span class="sxs-lookup"><span data-stu-id="577bb-165">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="577bb-166">Однако поставщики могут отсылать существующие индикаторы с этим набором в значение false, чтобы отключить индикаторы в системе.</span><span class="sxs-lookup"><span data-stu-id="577bb-166">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="577bb-167">Киллчаин</span><span class="sxs-lookup"><span data-stu-id="577bb-167">killChain</span></span>|<span data-ttu-id="577bb-168">Коллекция [киллчаин](#killchain-values)</span><span class="sxs-lookup"><span data-stu-id="577bb-168">[killChain](#killchain-values) collection</span></span>|<span data-ttu-id="577bb-169">Массив строк JSON, указывающий, какая точка или точки в цепочке аннулирования этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="577bb-169">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="577bb-170">Точные значения приведены в разделе "значения Киллчаин".</span><span class="sxs-lookup"><span data-stu-id="577bb-170">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="577bb-171">Кновнфалсепоситивес</span><span class="sxs-lookup"><span data-stu-id="577bb-171">knownFalsePositives</span></span>|<span data-ttu-id="577bb-172">String</span><span class="sxs-lookup"><span data-stu-id="577bb-172">String</span></span>|<span data-ttu-id="577bb-173">Сценарии, в которых индикатор может вызывать ложные срабатывания.</span><span class="sxs-lookup"><span data-stu-id="577bb-173">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="577bb-174">Это должен быть понятный для человека текст.</span><span class="sxs-lookup"><span data-stu-id="577bb-174">This should be human-readable text.</span></span>|
|<span data-ttu-id="577bb-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="577bb-175">lastReportedDateTime</span></span>|<span data-ttu-id="577bb-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="577bb-176">DateTimeOffset</span></span>|<span data-ttu-id="577bb-177">Время последнего рассмотрения индикатора.</span><span class="sxs-lookup"><span data-stu-id="577bb-177">The last time the indicator was seen.</span></span> <span data-ttu-id="577bb-178">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="577bb-178">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="577bb-179">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="577bb-179">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="577bb-180">Малварефамилинамес</span><span class="sxs-lookup"><span data-stu-id="577bb-180">malwareFamilyNames</span></span>|<span data-ttu-id="577bb-181">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="577bb-181">String collection</span></span>|<span data-ttu-id="577bb-182">Имя семейства вредоносных программ, связанное с индикатором, если оно существует.</span><span class="sxs-lookup"><span data-stu-id="577bb-182">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="577bb-183">Корпорация Майкрософт применяет имя семейства вредоносных программ (Майкрософт), если это возможно, то, что можно [](https://www.microsoft.com/wdsi/threats)найти с помощью энциклопедии по системе безопасности защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="577bb-183">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="577bb-184">Пассивеонли</span><span class="sxs-lookup"><span data-stu-id="577bb-184">passiveOnly</span></span>|<span data-ttu-id="577bb-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="577bb-185">Boolean</span></span>|<span data-ttu-id="577bb-186">Определяет, должен ли индикатор инициировать событие, видимое конечному пользователю.</span><span class="sxs-lookup"><span data-stu-id="577bb-186">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="577bb-187">Если задано значение true, средства безопасности не уведомляют конечного пользователя о выполнении "попадания".</span><span class="sxs-lookup"><span data-stu-id="577bb-187">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="577bb-188">Чаще всего это рассматривается как аудит или тихий режим по продуктам безопасности, в котором они просто зарегистрируются, но не будут выполнять действие.</span><span class="sxs-lookup"><span data-stu-id="577bb-188">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="577bb-189">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="577bb-189">Default value is false.</span></span>|
|<span data-ttu-id="577bb-190">severity</span><span class="sxs-lookup"><span data-stu-id="577bb-190">severity</span></span>|<span data-ttu-id="577bb-191">Int32</span><span class="sxs-lookup"><span data-stu-id="577bb-191">Int32</span></span>|<span data-ttu-id="577bb-192">Целое число, представляющее серьезность вредоносного поведения, идентифицируемого данными в индикаторе.</span><span class="sxs-lookup"><span data-stu-id="577bb-192">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="577bb-193">Допустимые значения: 0 – 5, где 5 — самый серьезный, а ноль — нет.</span><span class="sxs-lookup"><span data-stu-id="577bb-193">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="577bb-194">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="577bb-194">Default value is 3.</span></span>|
|<span data-ttu-id="577bb-195">tags</span><span class="sxs-lookup"><span data-stu-id="577bb-195">tags</span></span>|<span data-ttu-id="577bb-196">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="577bb-196">String collection</span></span>|<span data-ttu-id="577bb-197">Массив строк JSON, в котором хранятся произвольные Теги и ключевые слова.</span><span class="sxs-lookup"><span data-stu-id="577bb-197">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="577bb-198">Тлплевел</span><span class="sxs-lookup"><span data-stu-id="577bb-198">tlpLevel</span></span>|[<span data-ttu-id="577bb-199">Тлплевел</span><span class="sxs-lookup"><span data-stu-id="577bb-199">tlpLevel</span></span>](#tlplevel-values)| <span data-ttu-id="577bb-200">Значение протокола светофора для индикатора.</span><span class="sxs-lookup"><span data-stu-id="577bb-200">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="577bb-201">Возможные значения: `unknown`, `white`, `green`, `amber`, `red`.</span><span class="sxs-lookup"><span data-stu-id="577bb-201">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="577bb-202">значения Диамондмодел</span><span class="sxs-lookup"><span data-stu-id="577bb-202">diamondModel values</span></span>

<span data-ttu-id="577bb-203">Сведения об этой модели можно найти [в разделе Модель ромба](http://diamondmodel.org).</span><span class="sxs-lookup"><span data-stu-id="577bb-203">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="577bb-204">Значения</span><span class="sxs-lookup"><span data-stu-id="577bb-204">Values</span></span> | <span data-ttu-id="577bb-205">Описание</span><span class="sxs-lookup"><span data-stu-id="577bb-205">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="577bb-206">Злоумышленник</span><span class="sxs-lookup"><span data-stu-id="577bb-206">adversary</span></span>|<span data-ttu-id="577bb-207">Индикатор описывает.</span><span class="sxs-lookup"><span data-stu-id="577bb-207">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="577bb-208">поставлен</span><span class="sxs-lookup"><span data-stu-id="577bb-208">capability</span></span>|<span data-ttu-id="577bb-209">Индикатор является возможностью злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="577bb-209">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="577bb-210">инфраструктур</span><span class="sxs-lookup"><span data-stu-id="577bb-210">infrastructure</span></span>|<span data-ttu-id="577bb-211">Индикатор описывает инфраструктуру злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="577bb-211">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="577bb-212">стала</span><span class="sxs-lookup"><span data-stu-id="577bb-212">victim</span></span>|<span data-ttu-id="577bb-213">Индикатор описывает жертвой злоумышленника.</span><span class="sxs-lookup"><span data-stu-id="577bb-213">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="577bb-214">значения Киллчаин</span><span class="sxs-lookup"><span data-stu-id="577bb-214">killChain values</span></span>

| <span data-ttu-id="577bb-215">Значения</span><span class="sxs-lookup"><span data-stu-id="577bb-215">Values</span></span> | <span data-ttu-id="577bb-216">Описание</span><span class="sxs-lookup"><span data-stu-id="577bb-216">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="577bb-217">Действия</span><span class="sxs-lookup"><span data-stu-id="577bb-217">Actions</span></span>|<span data-ttu-id="577bb-218">Представляет "действия по целям".</span><span class="sxs-lookup"><span data-stu-id="577bb-218">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="577bb-219">Злоумышленник получает такие действия, как распределенная атака типа "отказ в обслуживании".</span><span class="sxs-lookup"><span data-stu-id="577bb-219">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="577bb-220">C2</span><span class="sxs-lookup"><span data-stu-id="577bb-220">C2</span></span>|<span data-ttu-id="577bb-221">Представляет канал управления, с которым работает скомпрометированная система.</span><span class="sxs-lookup"><span data-stu-id="577bb-221">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="577bb-222">Delivery</span><span class="sxs-lookup"><span data-stu-id="577bb-222">Delivery</span></span>|<span data-ttu-id="577bb-223">Процесс распространения кода эксплойта для жертв (например, USB, электронной почты, веб-сайтов).</span><span class="sxs-lookup"><span data-stu-id="577bb-223">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="577bb-224">Опасность</span><span class="sxs-lookup"><span data-stu-id="577bb-224">Exploitation</span></span>|<span data-ttu-id="577bb-225">Код эксплойта использует преимущества уязвимостей (например, выполнение кода).</span><span class="sxs-lookup"><span data-stu-id="577bb-225">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="577bb-226">Установка</span><span class="sxs-lookup"><span data-stu-id="577bb-226">Installation</span></span>|<span data-ttu-id="577bb-227">Установка вредоносных программ после использования уязвимости.</span><span class="sxs-lookup"><span data-stu-id="577bb-227">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="577bb-228">Реконнаиссанце</span><span class="sxs-lookup"><span data-stu-id="577bb-228">Reconnaissance</span></span>|<span data-ttu-id="577bb-229">Индикатор — это свидетельство того, что Группа действий получает сведения, которые будут использоваться при следующей атаке.</span><span class="sxs-lookup"><span data-stu-id="577bb-229">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="577bb-230">Веапонизатион</span><span class="sxs-lookup"><span data-stu-id="577bb-230">Weaponization</span></span>|<span data-ttu-id="577bb-231">Включение уязвимости в код эксплойта (например, вредоносные программы).</span><span class="sxs-lookup"><span data-stu-id="577bb-231">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="577bb-232">значения Тлплевел</span><span class="sxs-lookup"><span data-stu-id="577bb-232">tlpLevel values</span></span>

<span data-ttu-id="577bb-233">При отправке каждого индикатора должен быть задано значение протокола светофора (ТЛП).</span><span class="sxs-lookup"><span data-stu-id="577bb-233">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="577bb-234">Это значение представляет собой чувствительность и область общего доступа к заданному индикатору.</span><span class="sxs-lookup"><span data-stu-id="577bb-234">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="577bb-235">Значения</span><span class="sxs-lookup"><span data-stu-id="577bb-235">Values</span></span> | <span data-ttu-id="577bb-236">Описание</span><span class="sxs-lookup"><span data-stu-id="577bb-236">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="577bb-237">Белый</span><span class="sxs-lookup"><span data-stu-id="577bb-237">White</span></span>| <span data-ttu-id="577bb-238">Область общего доступа: unlimited.</span><span class="sxs-lookup"><span data-stu-id="577bb-238">Sharing scope: Unlimited.</span></span> <span data-ttu-id="577bb-239">Индикаторы могут быть предоставлены бесплатно, без ограничений.</span><span class="sxs-lookup"><span data-stu-id="577bb-239">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="577bb-240">Зеленый</span><span class="sxs-lookup"><span data-stu-id="577bb-240">Green</span></span>| <span data-ttu-id="577bb-241">Область общего доступа: сообщество.</span><span class="sxs-lookup"><span data-stu-id="577bb-241">Sharing scope: Community.</span></span> <span data-ttu-id="577bb-242">С помощью сообщества безопасности можно предоставить доступ к индикаторам.</span><span class="sxs-lookup"><span data-stu-id="577bb-242">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="577bb-243">Оранжевого</span><span class="sxs-lookup"><span data-stu-id="577bb-243">Amber</span></span>| <span data-ttu-id="577bb-244">Область общего доступа: ограничена.</span><span class="sxs-lookup"><span data-stu-id="577bb-244">Sharing scope: Limited.</span></span> <span data-ttu-id="577bb-245">Это параметр по умолчанию для индикаторов и разрешает совместное использование только тем, у которых есть ненужные: 1) службы и операторы служб, реализующие логику операций с угрозами; 2) клиенты, чьи системы соответствуют поведению с индикатором.</span><span class="sxs-lookup"><span data-stu-id="577bb-245">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="577bb-246">Красный</span><span class="sxs-lookup"><span data-stu-id="577bb-246">Red</span></span>| <span data-ttu-id="577bb-247">Область общего доступа: личная.</span><span class="sxs-lookup"><span data-stu-id="577bb-247">Sharing scope: Personal.</span></span> <span data-ttu-id="577bb-248">Эти индикаторы предназначены только для предоставления доступа напрямую и, желательно, в случае человека.</span><span class="sxs-lookup"><span data-stu-id="577bb-248">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="577bb-249">Как правило, ТЛП красные индикаторы не отправляются из-за ограничений, заданных ранее.</span><span class="sxs-lookup"><span data-stu-id="577bb-249">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="577bb-250">Если отправляются красные индикаторы ТЛП, свойству **пассивеонли** следует присвоить значение `True` также.</span><span class="sxs-lookup"><span data-stu-id="577bb-250">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="577bb-251">Ответ</span><span class="sxs-lookup"><span data-stu-id="577bb-251">Response</span></span>

<span data-ttu-id="577bb-252">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="577bb-252">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="577bb-253">Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="577bb-253">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="577bb-254">Примеры</span><span class="sxs-lookup"><span data-stu-id="577bb-254">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="577bb-255">Пример 1: запрос без верхнего колонтитула</span><span class="sxs-lookup"><span data-stu-id="577bb-255">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="577bb-256">Запрос</span><span class="sxs-lookup"><span data-stu-id="577bb-256">Request</span></span>

<span data-ttu-id="577bb-257">Ниже приведен пример запроса без `Prefer` заголовка.</span><span class="sxs-lookup"><span data-stu-id="577bb-257">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="577bb-258">HTTP</span><span class="sxs-lookup"><span data-stu-id="577bb-258">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="577bb-259">C#</span><span class="sxs-lookup"><span data-stu-id="577bb-259">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="577bb-260">Javascript</span><span class="sxs-lookup"><span data-stu-id="577bb-260">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="577bb-261">Цель — C</span><span class="sxs-lookup"><span data-stu-id="577bb-261">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="577bb-262">Отклик</span><span class="sxs-lookup"><span data-stu-id="577bb-262">Response</span></span>

<span data-ttu-id="577bb-263">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="577bb-263">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="577bb-264">Пример 2: запрос с заголовком предпочтения</span><span class="sxs-lookup"><span data-stu-id="577bb-264">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="577bb-265">Запрос</span><span class="sxs-lookup"><span data-stu-id="577bb-265">Request</span></span>

<span data-ttu-id="577bb-266">Ниже приведен пример запроса, включающего `Prefer` заголовок.</span><span class="sxs-lookup"><span data-stu-id="577bb-266">The following is an example of the request that includes the `Prefer` header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="577bb-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="577bb-267">Response</span></span>

<span data-ttu-id="577bb-268">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="577bb-268">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="577bb-269">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="577bb-269">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="577bb-270">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="577bb-270">All the properties will be returned from an actual call.</span></span>

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

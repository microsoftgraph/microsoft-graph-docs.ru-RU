---
title: Обновление объекта tiIndicator
description: Обновление свойств объекта tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 589c34a024097599e5b6f9de074cd635d28ccc77
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942199"
---
# <a name="update-tiindicator"></a><span data-ttu-id="0cccb-103">Обновление объекта tiIndicator</span><span class="sxs-lookup"><span data-stu-id="0cccb-103">Update tiIndicator</span></span>

<span data-ttu-id="0cccb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cccb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cccb-105">Обновление свойств объекта [tiIndicator.](../resources/tiindicator.md)</span><span class="sxs-lookup"><span data-stu-id="0cccb-105">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cccb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0cccb-106">Permissions</span></span>

<span data-ttu-id="0cccb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cccb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0cccb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cccb-109">Permission type</span></span>                        | <span data-ttu-id="0cccb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cccb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0cccb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cccb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0cccb-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="0cccb-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="0cccb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cccb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cccb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cccb-114">Not supported.</span></span> |
| <span data-ttu-id="0cccb-115">Application</span><span class="sxs-lookup"><span data-stu-id="0cccb-115">Application</span></span>                            | <span data-ttu-id="0cccb-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="0cccb-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cccb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cccb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0cccb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cccb-118">Request headers</span></span>

| <span data-ttu-id="0cccb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0cccb-119">Name</span></span>       | <span data-ttu-id="0cccb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0cccb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0cccb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cccb-121">Authorization</span></span> | <span data-ttu-id="0cccb-122">Bearer {code} **Required**</span><span class="sxs-lookup"><span data-stu-id="0cccb-122">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="0cccb-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="0cccb-123">Prefer</span></span> | <span data-ttu-id="0cccb-124">return=representation</span><span class="sxs-lookup"><span data-stu-id="0cccb-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cccb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cccb-125">Request body</span></span>

<span data-ttu-id="0cccb-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0cccb-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0cccb-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0cccb-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0cccb-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0cccb-128">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="0cccb-129">Необходимые поля: `id` , `expirationDateTime` `targetProduct` .</span><span class="sxs-lookup"><span data-stu-id="0cccb-129">Required fields are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="0cccb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cccb-130">Property</span></span>     | <span data-ttu-id="0cccb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0cccb-131">Type</span></span>        | <span data-ttu-id="0cccb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0cccb-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0cccb-133">action</span><span class="sxs-lookup"><span data-stu-id="0cccb-133">action</span></span>|<span data-ttu-id="0cccb-134">string</span><span class="sxs-lookup"><span data-stu-id="0cccb-134">string</span></span>| <span data-ttu-id="0cccb-135">Действие, применяемая, если индикатор соответствует из средства безопасности targetProduct.</span><span class="sxs-lookup"><span data-stu-id="0cccb-135">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="0cccb-136">Возможные значения: `unknown`, `allow`, `block`, `alert`.</span><span class="sxs-lookup"><span data-stu-id="0cccb-136">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="0cccb-137">activityGroupNames</span><span class="sxs-lookup"><span data-stu-id="0cccb-137">activityGroupNames</span></span>|<span data-ttu-id="0cccb-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0cccb-138">String collection</span></span>|<span data-ttu-id="0cccb-139">Имя разведки киберугроз для сторон, ответственных за вредоносную деятельность, подпадаемую под индикатор угрозы.</span><span class="sxs-lookup"><span data-stu-id="0cccb-139">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="0cccb-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="0cccb-140">additionalInformation</span></span>|<span data-ttu-id="0cccb-141">Строка</span><span class="sxs-lookup"><span data-stu-id="0cccb-141">String</span></span>|<span data-ttu-id="0cccb-142">Область catchall, в которую могут быть помещены дополнительные данные из индикатора, не охваченного другими свойствами tiIndicator.</span><span class="sxs-lookup"><span data-stu-id="0cccb-142">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="0cccb-143">Данные, помещенные в дополнительнуюinformation, как правило, не будут использоваться средством безопасности targetProduct.</span><span class="sxs-lookup"><span data-stu-id="0cccb-143">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="0cccb-144">confidence</span><span class="sxs-lookup"><span data-stu-id="0cccb-144">confidence</span></span>|<span data-ttu-id="0cccb-145">Int32</span><span class="sxs-lookup"><span data-stu-id="0cccb-145">Int32</span></span>|<span data-ttu-id="0cccb-146">Integer, представляющий доверие к данным в индикаторе, точно определяет вредоносное поведение.</span><span class="sxs-lookup"><span data-stu-id="0cccb-146">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="0cccb-147">Допустимые значения : 0 — 100, а 100 — самые высокие.</span><span class="sxs-lookup"><span data-stu-id="0cccb-147">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="0cccb-148">description</span><span class="sxs-lookup"><span data-stu-id="0cccb-148">description</span></span>|<span data-ttu-id="0cccb-149">Строка</span><span class="sxs-lookup"><span data-stu-id="0cccb-149">String</span></span>|<span data-ttu-id="0cccb-150">Краткое описание (100 символов или менее) угрозы, представленной индикатором.</span><span class="sxs-lookup"><span data-stu-id="0cccb-150">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="0cccb-151">diamondModel</span><span class="sxs-lookup"><span data-stu-id="0cccb-151">diamondModel</span></span>|[<span data-ttu-id="0cccb-152">diamondModel</span><span class="sxs-lookup"><span data-stu-id="0cccb-152">diamondModel</span></span>](../resources/tiindicator.md#diamondmodel-values)|<span data-ttu-id="0cccb-153">Область бриллиантовой модели, в которой существует этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="0cccb-153">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="0cccb-154">Возможные значения: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span><span class="sxs-lookup"><span data-stu-id="0cccb-154">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="0cccb-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0cccb-155">expirationDateTime</span></span>|<span data-ttu-id="0cccb-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cccb-156">DateTimeOffset</span></span>| <span data-ttu-id="0cccb-157">Строка DateTime, указывающая, когда истекает срок действия индикатора.</span><span class="sxs-lookup"><span data-stu-id="0cccb-157">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="0cccb-158">Чтобы избежать сохраняющихся в системе устаревших индикаторов, все индикаторы должны иметь дату истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="0cccb-158">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="0cccb-159">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0cccb-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0cccb-160">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="0cccb-160">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="0cccb-161">externalId</span><span class="sxs-lookup"><span data-stu-id="0cccb-161">externalId</span></span>|<span data-ttu-id="0cccb-162">String</span><span class="sxs-lookup"><span data-stu-id="0cccb-162">String</span></span>|<span data-ttu-id="0cccb-163">Идентификационный номер, который связывает индикатор с системой поставщика индикаторов (например, с иностранным ключом).</span><span class="sxs-lookup"><span data-stu-id="0cccb-163">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="0cccb-164">isActive</span><span class="sxs-lookup"><span data-stu-id="0cccb-164">isActive</span></span>|<span data-ttu-id="0cccb-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cccb-165">Boolean</span></span>|<span data-ttu-id="0cccb-166">Используется для отключения индикаторов внутри системы.</span><span class="sxs-lookup"><span data-stu-id="0cccb-166">Used to deactivate indicators within system.</span></span> <span data-ttu-id="0cccb-167">По умолчанию любой представленный индикатор задан как активный.</span><span class="sxs-lookup"><span data-stu-id="0cccb-167">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="0cccb-168">Однако для отключения индикаторов в системе поставщики могут отправлять существующие индикаторы с этим набором в "False".</span><span class="sxs-lookup"><span data-stu-id="0cccb-168">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="0cccb-169">killChain</span><span class="sxs-lookup"><span data-stu-id="0cccb-169">killChain</span></span>|<span data-ttu-id="0cccb-170">[коллекция killChain](../resources/tiindicator.md#killchain-values)</span><span class="sxs-lookup"><span data-stu-id="0cccb-170">[killChain](../resources/tiindicator.md#killchain-values) collection</span></span>|<span data-ttu-id="0cccb-171">Массив строк JSON, который описывает, какие точки или точки на цепочке убийств этот индикатор цели.</span><span class="sxs-lookup"><span data-stu-id="0cccb-171">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="0cccb-172">Для точных значений см. ниже "killChain values".</span><span class="sxs-lookup"><span data-stu-id="0cccb-172">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="0cccb-173">knownFalsePositives</span><span class="sxs-lookup"><span data-stu-id="0cccb-173">knownFalsePositives</span></span>|<span data-ttu-id="0cccb-174">Строка</span><span class="sxs-lookup"><span data-stu-id="0cccb-174">String</span></span>|<span data-ttu-id="0cccb-175">Сценарии, в которых индикатор может вызывать ложные срабатыва-</span><span class="sxs-lookup"><span data-stu-id="0cccb-175">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="0cccb-176">Это должен быть текст, читаемый для человека.</span><span class="sxs-lookup"><span data-stu-id="0cccb-176">This should be human-readable text.</span></span>|
|<span data-ttu-id="0cccb-177">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cccb-177">lastReportedDateTime</span></span>|<span data-ttu-id="0cccb-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cccb-178">DateTimeOffset</span></span>|<span data-ttu-id="0cccb-179">Последний раз индикатор был замечен.</span><span class="sxs-lookup"><span data-stu-id="0cccb-179">The last time the indicator was seen.</span></span> <span data-ttu-id="0cccb-180">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0cccb-180">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0cccb-181">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="0cccb-181">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="0cccb-182">malwareFamilyNames</span><span class="sxs-lookup"><span data-stu-id="0cccb-182">malwareFamilyNames</span></span>|<span data-ttu-id="0cccb-183">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0cccb-183">String collection</span></span>|<span data-ttu-id="0cccb-184">Семейство вредоносных программ, связанное с индикатором, если оно существует.</span><span class="sxs-lookup"><span data-stu-id="0cccb-184">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="0cccb-185">Корпорация Майкрософт предпочитает имя семейства вредоносных программ Майкрософт, если это возможно, которое можно найти в энциклопедии Защитник Windows security [Intelligence.](https://www.microsoft.com/wdsi/threats)</span><span class="sxs-lookup"><span data-stu-id="0cccb-185">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="0cccb-186">passiveOnly</span><span class="sxs-lookup"><span data-stu-id="0cccb-186">passiveOnly</span></span>|<span data-ttu-id="0cccb-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cccb-187">Boolean</span></span>|<span data-ttu-id="0cccb-188">Определяет, должен ли индикатор вызвать событие, которое видно конечному пользователю.</span><span class="sxs-lookup"><span data-stu-id="0cccb-188">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="0cccb-189">При наборе "true" средства безопасности не будут уведомлять конечного пользователя о том, что произошло "попадание".</span><span class="sxs-lookup"><span data-stu-id="0cccb-189">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="0cccb-190">Это чаще всего рассматривается как режим аудита или бесшумного режима с помощью продуктов безопасности, в которых они просто регистрировали совпадение, но не выполняли действие.</span><span class="sxs-lookup"><span data-stu-id="0cccb-190">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="0cccb-191">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="0cccb-191">Default value is false.</span></span>|
|<span data-ttu-id="0cccb-192">severity</span><span class="sxs-lookup"><span data-stu-id="0cccb-192">severity</span></span>|<span data-ttu-id="0cccb-193">Int32</span><span class="sxs-lookup"><span data-stu-id="0cccb-193">Int32</span></span>|<span data-ttu-id="0cccb-194">Набор, представляющий серьезность вредоносного поведения, определяемого данными в индикаторе.</span><span class="sxs-lookup"><span data-stu-id="0cccb-194">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="0cccb-195">Допустимые значения : 0 — 5, где 5 является самым строгим, а нуль — не очень серьезным.</span><span class="sxs-lookup"><span data-stu-id="0cccb-195">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="0cccb-196">Значение по умолчанию: 3.</span><span class="sxs-lookup"><span data-stu-id="0cccb-196">Default value is 3.</span></span>|
|<span data-ttu-id="0cccb-197">tags</span><span class="sxs-lookup"><span data-stu-id="0cccb-197">tags</span></span>|<span data-ttu-id="0cccb-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0cccb-198">String collection</span></span>|<span data-ttu-id="0cccb-199">Массив строк JSON, который хранит произвольные теги и ключевые слова.</span><span class="sxs-lookup"><span data-stu-id="0cccb-199">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="0cccb-200">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="0cccb-200">tlpLevel</span></span>|[<span data-ttu-id="0cccb-201">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="0cccb-201">tlpLevel</span></span>](../resources/tiindicator.md#tlplevel-values)| <span data-ttu-id="0cccb-202">Значение Протокола светофора для индикатора.</span><span class="sxs-lookup"><span data-stu-id="0cccb-202">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="0cccb-203">Возможные значения: `unknown`, `white`, `green`, `amber`, `red`.</span><span class="sxs-lookup"><span data-stu-id="0cccb-203">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|


## <a name="response"></a><span data-ttu-id="0cccb-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cccb-204">Response</span></span>

<span data-ttu-id="0cccb-205">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0cccb-205">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="0cccb-206">Если используется необязательный заголовок запроса, метод возвращает код ответа и обновленный `200 OK` [объект tiIndicator](../resources/tiindicator.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0cccb-206">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0cccb-207">Примеры</span><span class="sxs-lookup"><span data-stu-id="0cccb-207">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="0cccb-208">Пример 1. Запрос без загона Prefer</span><span class="sxs-lookup"><span data-stu-id="0cccb-208">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="0cccb-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cccb-209">Request</span></span>

<span data-ttu-id="0cccb-210">Ниже приводится пример запроса без `Prefer` загона.</span><span class="sxs-lookup"><span data-stu-id="0cccb-210">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="0cccb-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cccb-211">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```
# <a name="c"></a>[<span data-ttu-id="0cccb-212">C#</span><span class="sxs-lookup"><span data-stu-id="0cccb-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cccb-213">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cccb-213">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cccb-214">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cccb-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cccb-215">Java</span><span class="sxs-lookup"><span data-stu-id="0cccb-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0cccb-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cccb-216">Response</span></span>

<span data-ttu-id="0cccb-217">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0cccb-217">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="0cccb-218">Пример 2. Запрос с помощью загона Prefer</span><span class="sxs-lookup"><span data-stu-id="0cccb-218">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="0cccb-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cccb-219">Request</span></span>

<span data-ttu-id="0cccb-220">Ниже приводится пример запроса, включаемого `Prefer` в заглавную.</span><span class="sxs-lookup"><span data-stu-id="0cccb-220">The following is an example of the request that includes the `Prefer` header.</span></span>


# <a name="http"></a>[<span data-ttu-id="0cccb-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cccb-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator_2"
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
# <a name="c"></a>[<span data-ttu-id="0cccb-222">C#</span><span class="sxs-lookup"><span data-stu-id="0cccb-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cccb-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cccb-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cccb-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cccb-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cccb-225">Java</span><span class="sxs-lookup"><span data-stu-id="0cccb-225">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0cccb-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cccb-226">Response</span></span>

<span data-ttu-id="0cccb-227">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0cccb-227">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="0cccb-228">Объект отклика, показанный здесь, может быть сокращен для чтения.</span><span class="sxs-lookup"><span data-stu-id="0cccb-228">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0cccb-229">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0cccb-229">All the properties will be returned from an actual call.</span></span>

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



---
title: Обновление объекта tiIndicator
description: Обновление свойств объекта tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 3ded1ad2ac77cfd08320c54480de5dd24d319b91
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176957"
---
# <a name="update-tiindicator"></a><span data-ttu-id="a04aa-103">Обновление объекта tiIndicator</span><span class="sxs-lookup"><span data-stu-id="a04aa-103">Update tiIndicator</span></span>

<span data-ttu-id="a04aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a04aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a04aa-105">Обновление свойств объекта [tiIndicator.](../resources/tiindicator.md)</span><span class="sxs-lookup"><span data-stu-id="a04aa-105">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a04aa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a04aa-106">Permissions</span></span>

<span data-ttu-id="a04aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a04aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a04aa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a04aa-109">Permission type</span></span>                        | <span data-ttu-id="a04aa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a04aa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a04aa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a04aa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a04aa-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="a04aa-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="a04aa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a04aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a04aa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a04aa-114">Not supported.</span></span> |
| <span data-ttu-id="a04aa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a04aa-115">Application</span></span>                            | <span data-ttu-id="a04aa-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="a04aa-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="a04aa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a04aa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a04aa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a04aa-118">Request headers</span></span>

| <span data-ttu-id="a04aa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a04aa-119">Name</span></span>       | <span data-ttu-id="a04aa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a04aa-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a04aa-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a04aa-121">Authorization</span></span> | <span data-ttu-id="a04aa-122">Bearer {code} **Required**</span><span class="sxs-lookup"><span data-stu-id="a04aa-122">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="a04aa-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="a04aa-123">Prefer</span></span> | <span data-ttu-id="a04aa-124">return=representation</span><span class="sxs-lookup"><span data-stu-id="a04aa-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="a04aa-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a04aa-125">Request body</span></span>

<span data-ttu-id="a04aa-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a04aa-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a04aa-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a04aa-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a04aa-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a04aa-128">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="a04aa-129">Необходимые поля: `id` , `expirationDateTime` , `targetProduct` .</span><span class="sxs-lookup"><span data-stu-id="a04aa-129">Required fields are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="a04aa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a04aa-130">Property</span></span>     | <span data-ttu-id="a04aa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a04aa-131">Type</span></span>        | <span data-ttu-id="a04aa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a04aa-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a04aa-133">action</span><span class="sxs-lookup"><span data-stu-id="a04aa-133">action</span></span>|<span data-ttu-id="a04aa-134">string</span><span class="sxs-lookup"><span data-stu-id="a04aa-134">string</span></span>| <span data-ttu-id="a04aa-135">Действие, применяемая при совпадении индикатора из средства безопасности targetProduct.</span><span class="sxs-lookup"><span data-stu-id="a04aa-135">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="a04aa-136">Возможные значения: `unknown`, `allow`, `block`, `alert`.</span><span class="sxs-lookup"><span data-stu-id="a04aa-136">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="a04aa-137">activityGroupNames</span><span class="sxs-lookup"><span data-stu-id="a04aa-137">activityGroupNames</span></span>|<span data-ttu-id="a04aa-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a04aa-138">String collection</span></span>|<span data-ttu-id="a04aa-139">Имена аналитики киберугроз для сторон, ответственных за вредоносные действия, на которые распространяется индикатор угроз.</span><span class="sxs-lookup"><span data-stu-id="a04aa-139">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="a04aa-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="a04aa-140">additionalInformation</span></span>|<span data-ttu-id="a04aa-141">String</span><span class="sxs-lookup"><span data-stu-id="a04aa-141">String</span></span>|<span data-ttu-id="a04aa-142">Область catchall, в которую могут быть помещены дополнительные данные индикатора, не охваченные другими свойствами tiIndicator.</span><span class="sxs-lookup"><span data-stu-id="a04aa-142">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="a04aa-143">Данные, помещенные в additionalInformation, как правило, не используются средством безопасности targetProduct.</span><span class="sxs-lookup"><span data-stu-id="a04aa-143">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="a04aa-144">confidence</span><span class="sxs-lookup"><span data-stu-id="a04aa-144">confidence</span></span>|<span data-ttu-id="a04aa-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a04aa-145">Int32</span></span>|<span data-ttu-id="a04aa-146">Integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span><span class="sxs-lookup"><span data-stu-id="a04aa-146">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="a04aa-147">Допустимые значения: 0–100, 100 — наивысшее.</span><span class="sxs-lookup"><span data-stu-id="a04aa-147">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="a04aa-148">description</span><span class="sxs-lookup"><span data-stu-id="a04aa-148">description</span></span>|<span data-ttu-id="a04aa-149">String</span><span class="sxs-lookup"><span data-stu-id="a04aa-149">String</span></span>|<span data-ttu-id="a04aa-150">Краткое описание (не более 100 символов) угрозы, представляемой индикатором.</span><span class="sxs-lookup"><span data-stu-id="a04aa-150">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="a04aa-151">diamondModel</span><span class="sxs-lookup"><span data-stu-id="a04aa-151">diamondModel</span></span>|[<span data-ttu-id="a04aa-152">diamondModel</span><span class="sxs-lookup"><span data-stu-id="a04aa-152">diamondModel</span></span>](../resources/tiindicator.md#diamondmodel-values)|<span data-ttu-id="a04aa-153">Область диамантской модели, в которой существует этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="a04aa-153">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="a04aa-154">Возможные значения: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span><span class="sxs-lookup"><span data-stu-id="a04aa-154">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="a04aa-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a04aa-155">expirationDateTime</span></span>|<span data-ttu-id="a04aa-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a04aa-156">DateTimeOffset</span></span>| <span data-ttu-id="a04aa-157">Строка даты и времени, указывающая, когда истекает срок действия индикатора.</span><span class="sxs-lookup"><span data-stu-id="a04aa-157">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="a04aa-158">Все индикаторы должны иметь дату окончания срока действия, чтобы избежать сохраняющихся устаревших индикаторов в системе.</span><span class="sxs-lookup"><span data-stu-id="a04aa-158">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="a04aa-159">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a04aa-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a04aa-160">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a04aa-160">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="a04aa-161">externalId</span><span class="sxs-lookup"><span data-stu-id="a04aa-161">externalId</span></span>|<span data-ttu-id="a04aa-162">String</span><span class="sxs-lookup"><span data-stu-id="a04aa-162">String</span></span>|<span data-ttu-id="a04aa-163">Идентификационный номер, который связывает индикатор с системой поставщика индикаторов (например, с внешней клавишей).</span><span class="sxs-lookup"><span data-stu-id="a04aa-163">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="a04aa-164">isActive</span><span class="sxs-lookup"><span data-stu-id="a04aa-164">isActive</span></span>|<span data-ttu-id="a04aa-165">Логическое</span><span class="sxs-lookup"><span data-stu-id="a04aa-165">Boolean</span></span>|<span data-ttu-id="a04aa-166">Используется для отключения индикаторов в системе.</span><span class="sxs-lookup"><span data-stu-id="a04aa-166">Used to deactivate indicators within system.</span></span> <span data-ttu-id="a04aa-167">По умолчанию любой отправленный индикатор является активным.</span><span class="sxs-lookup"><span data-stu-id="a04aa-167">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="a04aa-168">Однако поставщики могут отправлять существующие индикаторы с этим набором "False", чтобы деактивировать индикаторы в системе.</span><span class="sxs-lookup"><span data-stu-id="a04aa-168">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="a04aa-169">killChain</span><span class="sxs-lookup"><span data-stu-id="a04aa-169">killChain</span></span>|<span data-ttu-id="a04aa-170">[Коллекция killChain](../resources/tiindicator.md#killchain-values)</span><span class="sxs-lookup"><span data-stu-id="a04aa-170">[killChain](../resources/tiindicator.md#killchain-values) collection</span></span>|<span data-ttu-id="a04aa-171">Массив строк JSON, который описывает точку или точку в цепочке событий, на которую направлен этот индикатор.</span><span class="sxs-lookup"><span data-stu-id="a04aa-171">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="a04aa-172">Точные значения см. ниже в "killChain values".</span><span class="sxs-lookup"><span data-stu-id="a04aa-172">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="a04aa-173">knownFalsePositives</span><span class="sxs-lookup"><span data-stu-id="a04aa-173">knownFalsePositives</span></span>|<span data-ttu-id="a04aa-174">String</span><span class="sxs-lookup"><span data-stu-id="a04aa-174">String</span></span>|<span data-ttu-id="a04aa-175">Сценарии, в которых индикатор может вызывать ложные срабатываия.</span><span class="sxs-lookup"><span data-stu-id="a04aa-175">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="a04aa-176">Это должен быть текст, читаемый человеком.</span><span class="sxs-lookup"><span data-stu-id="a04aa-176">This should be human-readable text.</span></span>|
|<span data-ttu-id="a04aa-177">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a04aa-177">lastReportedDateTime</span></span>|<span data-ttu-id="a04aa-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a04aa-178">DateTimeOffset</span></span>|<span data-ttu-id="a04aa-179">Время последнего увидеть индикатор.</span><span class="sxs-lookup"><span data-stu-id="a04aa-179">The last time the indicator was seen.</span></span> <span data-ttu-id="a04aa-180">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a04aa-180">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a04aa-181">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a04aa-181">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a04aa-182">malwareFamilyNames</span><span class="sxs-lookup"><span data-stu-id="a04aa-182">malwareFamilyNames</span></span>|<span data-ttu-id="a04aa-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a04aa-183">String collection</span></span>|<span data-ttu-id="a04aa-184">Имя семейства вредоносных программ, связанное с индикатором, если оно существует.</span><span class="sxs-lookup"><span data-stu-id="a04aa-184">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="a04aa-185">Корпорация Майкрософт по возможности предпочитает имя семейства вредоносных программ Майкрософт, которое можно найти с помощью Защитник Windows аналитики [безопасности.](https://www.microsoft.com/wdsi/threats)</span><span class="sxs-lookup"><span data-stu-id="a04aa-185">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="a04aa-186">passiveOnly</span><span class="sxs-lookup"><span data-stu-id="a04aa-186">passiveOnly</span></span>|<span data-ttu-id="a04aa-187">Логическое</span><span class="sxs-lookup"><span data-stu-id="a04aa-187">Boolean</span></span>|<span data-ttu-id="a04aa-188">Определяет, должен ли индикатор вызывать событие, которое видно конечному пользователю.</span><span class="sxs-lookup"><span data-stu-id="a04aa-188">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="a04aa-189">Если установлено "true", средства безопасности не будут уведомлять конечного пользователя о том, что произошло "попадание".</span><span class="sxs-lookup"><span data-stu-id="a04aa-189">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="a04aa-190">Это чаще всего рассматривается как аудит или режим в тихом режиме продуктами безопасности, в которых они просто регистрировали совпадение, но не выполняли это действие.</span><span class="sxs-lookup"><span data-stu-id="a04aa-190">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="a04aa-191">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="a04aa-191">Default value is false.</span></span>|
|<span data-ttu-id="a04aa-192">severity</span><span class="sxs-lookup"><span data-stu-id="a04aa-192">severity</span></span>|<span data-ttu-id="a04aa-193">Int32</span><span class="sxs-lookup"><span data-stu-id="a04aa-193">Int32</span></span>|<span data-ttu-id="a04aa-194">Integer representing the severity of the malicious behavior identified by the data within the indicator.</span><span class="sxs-lookup"><span data-stu-id="a04aa-194">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="a04aa-195">Допустимые значения: 0–5, где 5 — самый серьезный, а ноль — нет.</span><span class="sxs-lookup"><span data-stu-id="a04aa-195">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="a04aa-196">Значение по умолчанию: 3.</span><span class="sxs-lookup"><span data-stu-id="a04aa-196">Default value is 3.</span></span>|
|<span data-ttu-id="a04aa-197">tags</span><span class="sxs-lookup"><span data-stu-id="a04aa-197">tags</span></span>|<span data-ttu-id="a04aa-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a04aa-198">String collection</span></span>|<span data-ttu-id="a04aa-199">Массив строк JSON, который хранит произвольные теги и ключевые слова.</span><span class="sxs-lookup"><span data-stu-id="a04aa-199">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="a04aa-200">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="a04aa-200">tlpLevel</span></span>|[<span data-ttu-id="a04aa-201">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="a04aa-201">tlpLevel</span></span>](../resources/tiindicator.md#tlplevel-values)| <span data-ttu-id="a04aa-202">Значение протокола light traffic light для индикатора.</span><span class="sxs-lookup"><span data-stu-id="a04aa-202">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="a04aa-203">Возможные значения: `unknown`, `white`, `green`, `amber`, `red`.</span><span class="sxs-lookup"><span data-stu-id="a04aa-203">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|


## <a name="response"></a><span data-ttu-id="a04aa-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="a04aa-204">Response</span></span>

<span data-ttu-id="a04aa-205">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a04aa-205">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="a04aa-206">Если используется необязательный заголовщик запроса, метод возвращает код отклика и обновленный объект `200 OK` [tiIndicator](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a04aa-206">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a04aa-207">Примеры</span><span class="sxs-lookup"><span data-stu-id="a04aa-207">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="a04aa-208">Пример 1. Запрос без загона Prefer</span><span class="sxs-lookup"><span data-stu-id="a04aa-208">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="a04aa-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="a04aa-209">Request</span></span>

<span data-ttu-id="a04aa-210">Ниже приводится пример запроса без `Prefer` загона.</span><span class="sxs-lookup"><span data-stu-id="a04aa-210">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="a04aa-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="a04aa-211">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a04aa-212">C#</span><span class="sxs-lookup"><span data-stu-id="a04aa-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a04aa-213">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a04aa-213">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a04aa-214">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a04aa-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a04aa-215">Java</span><span class="sxs-lookup"><span data-stu-id="a04aa-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a04aa-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="a04aa-216">Response</span></span>

<span data-ttu-id="a04aa-217">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a04aa-217">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="a04aa-218">Пример 2. Запрос с заголбом Prefer</span><span class="sxs-lookup"><span data-stu-id="a04aa-218">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="a04aa-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="a04aa-219">Request</span></span>

<span data-ttu-id="a04aa-220">Ниже приводится пример запроса, включаемого в `Prefer` заголок.</span><span class="sxs-lookup"><span data-stu-id="a04aa-220">The following is an example of the request that includes the `Prefer` header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="a04aa-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="a04aa-221">Response</span></span>

<span data-ttu-id="a04aa-222">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a04aa-222">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a04aa-223">Показанный здесь объект ответа может быть сокращен для учитаемости.</span><span class="sxs-lookup"><span data-stu-id="a04aa-223">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a04aa-224">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a04aa-224">All the properties will be returned from an actual call.</span></span>

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



---
title: 'user: findMeetingTimes'
description: Предложение времени проведения собрания и местоположения с учетом доступности организатора и участников, а также ограничений по местоположению или времени, указанных в качестве параметров.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b9a04d0a7bcde0ebd70646256f644f46c71522bf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970157"
---
# <a name="user-findmeetingtimes"></a><span data-ttu-id="32660-103">user: findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="32660-103">user: findMeetingTimes</span></span>

<span data-ttu-id="32660-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32660-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32660-105">Предложение времени проведения собрания и местоположения с учетом доступности организатора и участников, а также ограничений по местоположению или времени, указанных в качестве параметров.</span><span class="sxs-lookup"><span data-stu-id="32660-105">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints specified as parameters.</span></span>

<span data-ttu-id="32660-p101">Если метод **findMeetingTimes** не может вернуть предложение, то в свойстве **emptySuggestionsReason** будет указана причина. Это значение поможет вам лучше настраивать параметры и снова вызывать метод **findMeetingTimes**.</span><span class="sxs-lookup"><span data-stu-id="32660-p101">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

<span data-ttu-id="32660-108">Алгоритм, используемый для предложения времени проведения собраний и местоположений, периодически подвергается точной настройке.</span><span class="sxs-lookup"><span data-stu-id="32660-108">The algorithm used to suggest meeting times and locations undergoes fine-tuning from time to time.</span></span> <span data-ttu-id="32660-109">В таких сценариях, как среды тестирования, где входные параметры и данные календаря остаются неизменными, можно ожидать, что со временем предлагаемые результаты могут отличаться.</span><span class="sxs-lookup"><span data-stu-id="32660-109">In scenarios like test environments where the input parameters and calendar data remain static, expect that the suggested results may differ over time.</span></span>


## <a name="permissions"></a><span data-ttu-id="32660-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32660-110">Permissions</span></span>
<span data-ttu-id="32660-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32660-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32660-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32660-113">Permission type</span></span>      | <span data-ttu-id="32660-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32660-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32660-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32660-115">Delegated (work or school account)</span></span> | <span data-ttu-id="32660-116">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span><span class="sxs-lookup"><span data-stu-id="32660-116">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span></span>    |
|<span data-ttu-id="32660-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32660-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32660-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32660-118">Not supported.</span></span>    |
|<span data-ttu-id="32660-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32660-119">Application</span></span> | <span data-ttu-id="32660-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32660-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="32660-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32660-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a><span data-ttu-id="32660-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32660-122">Request headers</span></span>
| <span data-ttu-id="32660-123">Имя</span><span class="sxs-lookup"><span data-stu-id="32660-123">Name</span></span>       | <span data-ttu-id="32660-124">Значение</span><span class="sxs-lookup"><span data-stu-id="32660-124">Value</span></span>|
|:---------------|:----------|
| <span data-ttu-id="32660-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32660-125">Authorization</span></span>  | <span data-ttu-id="32660-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32660-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32660-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="32660-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="32660-p105">Строка, представляющая определенный часовой пояс для ответа, например "Тихоокеанское время США (зима)". Необязательный параметр. Время в формате UTC используется, если этот заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="32660-p105">A string representing a specific time zone for the response, for example, "Pacific Standard Time". Optional. UTC is used if this header is not specified.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32660-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32660-132">Request body</span></span>
<span data-ttu-id="32660-p106">Ниже перечислены все поддерживаемые параметры. В зависимости от сценария, укажите объект JSON для каждого из обязательных параметров в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="32660-p106">All the supported parameters are listed below. Depending on your scenario, specify a JSON object for each of the necessary parameters in the request body.</span></span> 


| <span data-ttu-id="32660-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="32660-135">Parameter</span></span>    | <span data-ttu-id="32660-136">Тип</span><span class="sxs-lookup"><span data-stu-id="32660-136">Type</span></span>   |<span data-ttu-id="32660-137">Описание</span><span class="sxs-lookup"><span data-stu-id="32660-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32660-138">attendees</span><span class="sxs-lookup"><span data-stu-id="32660-138">attendees</span></span>|<span data-ttu-id="32660-139">Коллекция объектов [attendeeBase](../resources/attendeebase.md)</span><span class="sxs-lookup"><span data-stu-id="32660-139">[attendeeBase](../resources/attendeebase.md) collection</span></span>|<span data-ttu-id="32660-140">Коллекция участников или ресурсов для собрания.</span><span class="sxs-lookup"><span data-stu-id="32660-140">A collection of attendees or resources for the meeting.</span></span> <span data-ttu-id="32660-141">В соответствующем свойстве **введите** `required` или выберите `optional` для человека и `resource` для ресурса, например комнаты для собраний.</span><span class="sxs-lookup"><span data-stu-id="32660-141">In the corresponding **type** property, specify `required` or `optional` for a person and `resource` for a resource like meeting room.</span></span> <span data-ttu-id="32660-142">Если этот параметр не указан, **findMeetingTimes** предполагается `required` для свойства **Type** .</span><span class="sxs-lookup"><span data-stu-id="32660-142">If not specified, **findMeetingTimes** assumes `required` for the **type** property.</span></span> <span data-ttu-id="32660-143">Если указана пустая коллекция, действие **findMeetingTimes** ищет свободные периоды времени для организатора.</span><span class="sxs-lookup"><span data-stu-id="32660-143">An empty collection causes **findMeetingTimes** to look for free time slots for only the organizer.</span></span> <span data-ttu-id="32660-144">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="32660-144">Optional.</span></span>|
|<span data-ttu-id="32660-145">isOrganizerOptional</span><span class="sxs-lookup"><span data-stu-id="32660-145">isOrganizerOptional</span></span>|<span data-ttu-id="32660-146">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="32660-146">Edm.Boolean</span></span>|<span data-ttu-id="32660-p108">Задайте значение `True`, если присутствие организатора не обязательно. Значение по умолчанию: `false`. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="32660-p108">Specify `True` if the organizer doesn't necessarily have to attend. The default is `false`. Optional.</span></span>|
|<span data-ttu-id="32660-150">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="32660-150">locationConstraint</span></span>|[<span data-ttu-id="32660-151">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="32660-151">locationConstraint</span></span>](../resources/locationconstraint.md)|<span data-ttu-id="32660-p109">Требования организатора к месту проведения собрания (например, требуется ли соответствующее предложение или собрание может пройти только в определенных местах). Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="32660-p109">The organizer's requirements about the meeting location, such as whether a suggestion for a meeting location is required, or there are specific locations only where the meeting can take place. Optional.</span></span>|
|<span data-ttu-id="32660-154">maxCandidates</span><span class="sxs-lookup"><span data-stu-id="32660-154">maxCandidates</span></span>|<span data-ttu-id="32660-155">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="32660-155">Edm.Int32</span></span>|<span data-ttu-id="32660-p110">Максимальное количество возвращаемых предложений времени проведения собрания. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="32660-p110">The maximum number of meeting time suggestions to be returned. Optional.</span></span>|
|<span data-ttu-id="32660-158">meetingDuration</span><span class="sxs-lookup"><span data-stu-id="32660-158">meetingDuration</span></span>|<span data-ttu-id="32660-159">Edm.Duration</span><span class="sxs-lookup"><span data-stu-id="32660-159">Edm.Duration</span></span>|<span data-ttu-id="32660-160">Длительность собрания, обозначенная в формате [ISO 8601](https://www.iso.org/iso/iso8601) .</span><span class="sxs-lookup"><span data-stu-id="32660-160">The length of the meeting, denoted in [ISO 8601](https://www.iso.org/iso/iso8601) format.</span></span> <span data-ttu-id="32660-161">Например, 1 час обозначается как "PT1H", где "P" — это обозначение длительности, а "H" — обозначение часа.</span><span class="sxs-lookup"><span data-stu-id="32660-161">For example, 1 hour is denoted as 'PT1H', where 'P' is the duration designator, 'T' is the time designator, and 'H' is the hour designator.</span></span> <span data-ttu-id="32660-162">Используйте M, чтобы указать минуты для длительности; Например, 2 часа и 30 минут будут иметь вид "PT2H30M".</span><span class="sxs-lookup"><span data-stu-id="32660-162">Use M to indicate minutes for the duration; for example, 2 hours and 30 minutes would be 'PT2H30M'.</span></span> <span data-ttu-id="32660-163">Если продолжительность собрания не указана, метод **findMeetingTimes** использует значение по умолчанию — 30 минут.</span><span class="sxs-lookup"><span data-stu-id="32660-163">If no meeting duration is specified, **findMeetingTimes** uses the default of 30 minutes.</span></span> <span data-ttu-id="32660-164">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="32660-164">Optional.</span></span>|
|<span data-ttu-id="32660-165">minimumAttendeePercentage</span><span class="sxs-lookup"><span data-stu-id="32660-165">minimumAttendeePercentage</span></span>|<span data-ttu-id="32660-166">Edm.Double</span><span class="sxs-lookup"><span data-stu-id="32660-166">Edm.Double</span></span>| <span data-ttu-id="32660-p112">Минимальная [достоверность](#the-confidence-of-a-meeting-suggestion), необходимая, чтобы вернуть период времени в ответе. Это процентное значение от 0 до 100. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="32660-p112">The minimum required [confidence](#the-confidence-of-a-meeting-suggestion) for a time slot to be returned in the response. It is a % value ranging from 0 to 100. Optional.</span></span>|
|<span data-ttu-id="32660-170">returnSuggestionReasons</span><span class="sxs-lookup"><span data-stu-id="32660-170">returnSuggestionReasons</span></span>|<span data-ttu-id="32660-171">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="32660-171">Edm.Boolean</span></span>|<span data-ttu-id="32660-p113">Задайте значение `True`, если требуется вернуть причину каждого предложения в свойстве **suggestionReason**. По умолчанию задано значение `false`, и это свойство не возвращается. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="32660-p113">Specify `True` to return a reason for each meeting suggestion in the **suggestionReason** property. The default is `false` to not return that property. Optional.</span></span>|
|<span data-ttu-id="32660-175">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="32660-175">timeConstraint</span></span>|[<span data-ttu-id="32660-176">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="32660-176">timeConstraint</span></span>](../resources/timeconstraint.md)|<span data-ttu-id="32660-p114">Ограничения по времени для собрания, к которым могут относиться характер собрания (свойство **activityDomain** ) и возможное время проведения собрания (свойство **timeSlots** ). Если параметр **activityDomain** не задан, метод **findMeetingTimes** считает, что для него установлено значение `work`. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="32660-p114">Any time restrictions for a meeting, which can include the nature of the meeting ( **activityDomain** property) and possible meeting time periods ( **timeSlots** property). **findMeetingTimes** assumes **activityDomain** as `work` if you don't specify this parameter. Optional.</span></span>|

<span data-ttu-id="32660-180">В таблице ниже описываются ограничения, которые можно в дальнейшем указать в параметре **timeConstraint**.</span><span class="sxs-lookup"><span data-stu-id="32660-180">The following table describes the restrictions you can further specify in the **timeConstraint** parameter.</span></span>

|<span data-ttu-id="32660-181">Значение activityDomain в параметре timeConstraint</span><span class="sxs-lookup"><span data-stu-id="32660-181">activityDomain value in timeConstraint</span></span>|<span data-ttu-id="32660-182">Предложения по времени проведения собраний</span><span class="sxs-lookup"><span data-stu-id="32660-182">Suggestions for meeting times</span></span>|
|:-----|:-----|
|<span data-ttu-id="32660-183">work</span><span class="sxs-lookup"><span data-stu-id="32660-183">work</span></span>| <span data-ttu-id="32660-p115">Предложения ограничиваются рамками рабочего времени пользователя, которое определяется настройками его календаря. Пользователь или администратор также могут изменять рабочее время. По умолчанию рабочим считается время с 8:00 до 17:00 (в часовом поясе, установленном для почтового ящика пользователя) с понедельника по пятницу. Это значение является значением по умолчанию, если не задан параметр **activityDomain**.</span><span class="sxs-lookup"><span data-stu-id="32660-p115">Suggestions are within the user's work hours which are defined in the user’s calendar configuration and can be customized by the user or administrator. The default work hours are Monday to Friday, 8am to 5pm in the time zone set for the mailbox. This is the default value if no **activityDomain** is specified.</span></span> |
|<span data-ttu-id="32660-187">personal</span><span class="sxs-lookup"><span data-stu-id="32660-187">personal</span></span>| <span data-ttu-id="32660-p116">Предложения возможны в рабочее время пользователя, а также в субботу и воскресенье. По умолчанию задано время с 8:00 до 17:00 (в часовом поясе, установленном для почтового ящика пользователя) с понедельника по воскресенье.</span><span class="sxs-lookup"><span data-stu-id="32660-p116">Suggestions are within the user's work hours, and Saturday and Sunday. The default is Monday to Sunday, 8am to 5pm, in the time zone setting for the mailbox.</span></span>|
|<span data-ttu-id="32660-190">unrestricted</span><span class="sxs-lookup"><span data-stu-id="32660-190">unrestricted</span></span> | <span data-ttu-id="32660-191">Предложения могут относиться к любому времени в любой день недели.</span><span class="sxs-lookup"><span data-stu-id="32660-191">Suggestions can be from all hours of a day, all days of a week.</span></span>|
|<span data-ttu-id="32660-192">unknown</span><span class="sxs-lookup"><span data-stu-id="32660-192">unknown</span></span> | <span data-ttu-id="32660-p117">Не рекомендуем использовать это значение, так как в будущем его поддержка будет прекращена. В настоящее время значение равносильно значению `work`. Измените существующий код, используя соответствующие значения `work`, `personal` или `unrestricted`.</span><span class="sxs-lookup"><span data-stu-id="32660-p117">Do not use this value as it will be deprecated in the future. Currently behaves the same as `work`. Change any existing code to use `work`, `personal` or `unrestricted` as appropriate.</span></span>|


<span data-ttu-id="32660-p118">В зависимости от указанных параметров, действие **findMeetingTimes** проверяет сведения о доступности в основных календарях организатора и участников. Действие вычисляет наиболее подходящее время собрания и возвращает предложения.</span><span class="sxs-lookup"><span data-stu-id="32660-p118">Based on the specified parameters, **findMeetingTimes** checks the free/busy status in the primary calendars of the organizer and attendees. The action calculates the best possible meeting times, and returns any meeting suggestions.</span></span>

## <a name="response"></a><span data-ttu-id="32660-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="32660-198">Response</span></span>

<span data-ttu-id="32660-199">В случае успеха этот метод возвращает код ответа `200 OK` и объект [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="32660-199">If successful, this method returns `200 OK` response code and a [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) in the response body.</span></span> 

<span data-ttu-id="32660-p119">Объект **meetingTimeSuggestionsResult** включает коллекцию предложений и свойство **emptySuggestionsReason**. Каждое предложение определяется как объект [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), где средняя вероятность присутствия участников составляет 50 % или определенное процентное значение, указанное в параметре **minimumAttendeePercentage**.</span><span class="sxs-lookup"><span data-stu-id="32660-p119">A **meetingTimeSuggestionsResult** includes a collection of meeting suggestions and an **emptySuggestionsReason** property. Each suggestion is defined as a [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), with attendees having on the average a confidence level of 50% to attend, or a specific % that you have specified in the **minimumAttendeePercentage** parameter.</span></span> 

<span data-ttu-id="32660-202">По умолчанию каждое предлагаемое время проведения собрания указывается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="32660-202">By default, each meeting time suggestion is returned in UTC.</span></span> 

<span data-ttu-id="32660-p120">Если метод **findMeetingTimes** не может вернуть предложение, то в свойстве **emptySuggestionsReason** будет указана причина. Это значение поможет вам лучше настраивать параметры и снова вызывать метод **findMeetingTimes**.</span><span class="sxs-lookup"><span data-stu-id="32660-p120">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

### <a name="the-confidence-of-a-meeting-suggestion"></a><span data-ttu-id="32660-205">Достоверность предложения</span><span class="sxs-lookup"><span data-stu-id="32660-205">The confidence of a meeting suggestion</span></span>

<span data-ttu-id="32660-206">Свойство **confidence** объекта **meetingTimeSuggestion** принимает значения от 0 % до 100 % и представляет вероятность того, что все участники посетят собрание. Она зависит от сведений о доступности каждого участника:</span><span class="sxs-lookup"><span data-stu-id="32660-206">The **confidence** property of a **meetingTimeSuggestion** ranges from 0% to 100%, and represents the chance that all the attendees attend the meeting, based on each of their individual free/busy status:</span></span>

- <span data-ttu-id="32660-207">Если тот или иной участник доступен в указанный период времени, для него задается вероятность посещения 100 %, если его состояние неизвестно — 49 %, а если он занят— 0 %.</span><span class="sxs-lookup"><span data-stu-id="32660-207">For each attendee, a free status for a specified meeting time period corresponds to 100% chance of attendance, unknown status 49%, and busy status 0%.</span></span>
- <span data-ttu-id="32660-208">Достоверность предлагаемого времени собрания вычисляется как средняя вероятность присутствия всех указанных участников собрания.</span><span class="sxs-lookup"><span data-stu-id="32660-208">The confidence of a meeting time suggestion is computed by averaging the chance of attendance over all the attendees specified for that meeting.</span></span>
- <span data-ttu-id="32660-p121">При наличии нескольких предложений времени действие **findMeetingTimes** сначала сортирует их по убыванию значения достоверности. При наличии нескольких предложений с одинаковой достоверностью это действие сортирует их в хронологическом порядке.</span><span class="sxs-lookup"><span data-stu-id="32660-p121">If there are multiple meeting time suggestions, the **findMeetingTimes** action first orders the suggestions by their computed confidence value from high to low. If there are suggestions with the same confidence, the action then orders these suggestions chronologically.</span></span>
- <span data-ttu-id="32660-p122">С помощью необязательного параметра **minimumAttendeePercentage** метода **findMeetingTimes** вы можете сделать так, чтобы возвращались предложения со значением достоверности не ниже указанного. Например, вы можете задать для параметра **minimumAttendeePercentage** значение 80 %, если вас интересуют только те предложения, для которых вероятность присутствия всех участников составляет не менее 80 %. Если параметр **minimumAttendeePercentage** не указан, метод **findMeetingTimes** предполагает значение 50 %.</span><span class="sxs-lookup"><span data-stu-id="32660-p122">You can use the **minimumAttendeePercentage** optional parameter for **findMeetingTimes** to specify only meeting time suggestions of at least certain confidence level should be returned. For example, you can specify a **minimumAttendeePercentage** of 80% if you want only suggestions that have an 80% chance or more that all the attendees are attending. If you do not specify **minimumAttendeePercentage** , **findMeetingTimes** assumes a value of 50%.</span></span>

<span data-ttu-id="32660-214">Допустим, время проведения собрания предложено с учетом 3 участников со следующими сведениями о доступности:</span><span class="sxs-lookup"><span data-stu-id="32660-214">As an example, if a meeting time suggestion involves 3 attendees with the following free/busy status:</span></span>

|<span data-ttu-id="32660-215">**Участник**</span><span class="sxs-lookup"><span data-stu-id="32660-215">**Attendee**</span></span>|<span data-ttu-id="32660-216">**Сведения о доступности**</span><span class="sxs-lookup"><span data-stu-id="32660-216">**Free/busy status**</span></span>|<span data-ttu-id="32660-217">**Процентная вероятность посещения**</span><span class="sxs-lookup"><span data-stu-id="32660-217">**% Chance of attendance**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="32660-218">Дарья</span><span class="sxs-lookup"><span data-stu-id="32660-218">Dana</span></span> | <span data-ttu-id="32660-219">Свободна</span><span class="sxs-lookup"><span data-stu-id="32660-219">Free</span></span> | <span data-ttu-id="32660-220">100 %</span><span class="sxs-lookup"><span data-stu-id="32660-220">100%</span></span> |
|<span data-ttu-id="32660-221">Иван</span><span class="sxs-lookup"><span data-stu-id="32660-221">John</span></span> | <span data-ttu-id="32660-222">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="32660-222">Unknown</span></span> | <span data-ttu-id="32660-223">49 %</span><span class="sxs-lookup"><span data-stu-id="32660-223">49%</span></span> |
|<span data-ttu-id="32660-224">Samantha</span><span class="sxs-lookup"><span data-stu-id="32660-224">Samantha</span></span> | <span data-ttu-id="32660-225">Занята</span><span class="sxs-lookup"><span data-stu-id="32660-225">Busy</span></span> | <span data-ttu-id="32660-226">0 %</span><span class="sxs-lookup"><span data-stu-id="32660-226">0%</span></span> |

<span data-ttu-id="32660-227">В этом случае достоверность предлагаемого времени проведения собрания (средняя вероятность посещения) составляет (100 % + 49 % + 0 %)/3 = 49,66 %.</span><span class="sxs-lookup"><span data-stu-id="32660-227">Then the confidence of the meeting time suggestion, which is the average chance of attendance, is (100% + 49% + 0%)/3 = 49.66%.</span></span>

<span data-ttu-id="32660-228">Если в методе **findMeetingTimes** указать для параметра **minimumAttendeePercentage** значение 80 %, операция не будет предлагать это время в ответе, так как 49,66 % < 80 %.</span><span class="sxs-lookup"><span data-stu-id="32660-228">If you specify a **minimumAttendeePercentage** of 80% in a **findMeetingTimes** operation, because 49.66% < 80%, the operation will not suggest this time in the response.</span></span>

## <a name="example"></a><span data-ttu-id="32660-229">Пример</span><span class="sxs-lookup"><span data-stu-id="32660-229">Example</span></span>

<span data-ttu-id="32660-230">В приведенном ниже примере показано, как найти время для встречи в заранее установленном месте и запросить причину для каждого предложения, указав следующие параметры в тексте запроса:</span><span class="sxs-lookup"><span data-stu-id="32660-230">The following example shows how to find time to meet at a pre-determined location, and request a reason for each suggestion, by specifying the following parameters in the request body:</span></span>

- <span data-ttu-id="32660-231">**attendees**</span><span class="sxs-lookup"><span data-stu-id="32660-231">**attendees**</span></span>
- <span data-ttu-id="32660-232">**locationConstraint**</span><span class="sxs-lookup"><span data-stu-id="32660-232">**locationConstraint**</span></span>
- <span data-ttu-id="32660-233">**timeConstraint**</span><span class="sxs-lookup"><span data-stu-id="32660-233">**timeConstraint**</span></span>
- <span data-ttu-id="32660-234">**isOrganizerOptional**</span><span class="sxs-lookup"><span data-stu-id="32660-234">**isOrganizerOptional**</span></span>
- <span data-ttu-id="32660-235">**meetingDuration**</span><span class="sxs-lookup"><span data-stu-id="32660-235">**meetingDuration**</span></span>
- <span data-ttu-id="32660-236">**returnSuggestionReasons**</span><span class="sxs-lookup"><span data-stu-id="32660-236">**returnSuggestionReasons**</span></span>
- <span data-ttu-id="32660-237">**minimumAttendeePercentage**</span><span class="sxs-lookup"><span data-stu-id="32660-237">**minimumAttendeePercentage**</span></span>

<span data-ttu-id="32660-238">Указав параметр **returnSuggestionReasons** , вы также получите в свойстве **suggestionReason** объяснение для каждого предложения, если метод **findMeetingTimes** возвращает какие-либо предложения.</span><span class="sxs-lookup"><span data-stu-id="32660-238">By setting the **returnSuggestionReasons** parameter, you also get an explanation in the **suggestionReason** property for each suggestion, if **findMeetingTimes** returns any suggestion.</span></span>

<span data-ttu-id="32660-239">Обратите внимание, что в запросе указывается Тихоокеанское время.</span><span class="sxs-lookup"><span data-stu-id="32660-239">Notice that the request specifies time in the PST time zone.</span></span> <span data-ttu-id="32660-240">В ответе по умолчанию возвращаются предложения времени проведения собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="32660-240">By default, the response returns meeting time suggestions in UTC.</span></span> <span data-ttu-id="32660-241">С помощью заголовка запроса `Prefer: outlook.timezone` вы можете сделать так, чтобы в ответе тоже возвращалось Тихоокеанское время.</span><span class="sxs-lookup"><span data-stu-id="32660-241">You can use the `Prefer: outlook.timezone` request header to specify PST as well for the time values in the response.</span></span>

##### <a name="request"></a><span data-ttu-id="32660-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="32660-242">Request</span></span>
<span data-ttu-id="32660-243">Ниже представлен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32660-243">Here is the example request.</span></span>

# <a name="http"></a>[<span data-ttu-id="32660-244">HTTP</span><span class="sxs-lookup"><span data-stu-id="32660-244">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/beta/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Alex Wilbur",
        "address": "alexw@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": "false",  
    "suggestLocation": "false",  
    "locations": [ 
      { 
        "resolveAvailability": "false",
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"work", 
    "timeSlots": [ 
      { 
        "start": { 
          "dateTime": "2019-04-16T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2019-04-18T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "isOrganizerOptional": "false",
  "meetingDuration": "PT1H",
  "returnSuggestionReasons": "true",
  "minimumAttendeePercentage": "100"
}
```
# <a name="c"></a>[<span data-ttu-id="32660-245">C#</span><span class="sxs-lookup"><span data-stu-id="32660-245">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-findmeetingtimes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32660-246">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32660-246">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-findmeetingtimes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32660-247">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32660-247">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-findmeetingtimes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32660-248">Java</span><span class="sxs-lookup"><span data-stu-id="32660-248">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-findmeetingtimes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="32660-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="32660-249">Response</span></span>
<span data-ttu-id="32660-p124">Ниже представлен пример ответа. Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32660-p124">Here is an example response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason": "",
    "meetingTimeSuggestions": [
        {
            "confidence": 100,
            "order": 1,
            "organizerAvailability": "free",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T16:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T17:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "order": 2,
            "organizerAvailability": "free",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T08:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T09:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "order": 3,
            "organizerAvailability": "tentative",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T15:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T16:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "order": 4,
            "organizerAvailability": "tentative",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T09:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T10:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "order": 5,
            "organizerAvailability": "tentative",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T12:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T13:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/api/user_findmeetingtimes.md:\r\n      Failed to parse any rows out of table with headers: |activityDomain value|Suggestions for meeting times|",
    "Error: user_findmeetingtimes/meetingTimeSuggestions/member/confidence:\r\n    Expected type Float but actual was Int64. Property: confidence, actual value: '100'",
    "Error: user_findmeetingtimes/meetingTimeSuggestions/member/confidence:\r\n    Expected type Double but actual was Int64. Property: confidence, actual value: '100'"
  ]
}
-->



---
title: 'user: findMeetingTimes'
description: Предложение времени проведения собрания и местоположения с учетом доступности организатора и участников, а также ограничений по местоположению или времени, указанных в качестве параметров.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 59f5977169563acd3589e0a8417b12c5f5daf1d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509204"
---
# <a name="user-findmeetingtimes"></a><span data-ttu-id="bd7ee-103">user: findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="bd7ee-103">user: findMeetingTimes</span></span>

<span data-ttu-id="bd7ee-104">Пространство имен: microsoft.graph. Предложение времени проведения собрания и местоположения с учетом доступности организатора и участников, а также ограничений по местоположению или времени, указанных в качестве параметров.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-104">Namespace: microsoft.graph Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints specified as parameters.</span></span>

<span data-ttu-id="bd7ee-p101">Если метод **findMeetingTimes** не может вернуть предложение, то в свойстве **emptySuggestionsReason** будет указана причина. Это значение поможет вам лучше настраивать параметры и снова вызывать метод **findMeetingTimes**.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p101">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

<span data-ttu-id="bd7ee-107">Алгоритм, используемый для предложения времени проведения собраний и местоположений, периодически подвергается точной настройке.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-107">The algorithm used to suggest meeting times and locations undergoes fine-tuning from time to time.</span></span> <span data-ttu-id="bd7ee-108">В таких сценариях, как среды тестирования, где входные параметры и данные календаря остаются неизменными, можно ожидать, что со временем предлагаемые результаты могут отличаться.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-108">In scenarios like test environments where the input parameters and calendar data remain static, expect that the suggested results may differ over time.</span></span>


## <a name="permissions"></a><span data-ttu-id="bd7ee-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd7ee-109">Permissions</span></span>
<span data-ttu-id="bd7ee-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd7ee-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd7ee-112">Permission type</span></span>      | <span data-ttu-id="bd7ee-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd7ee-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd7ee-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd7ee-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bd7ee-115">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span><span class="sxs-lookup"><span data-stu-id="bd7ee-115">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span></span>    |
|<span data-ttu-id="bd7ee-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd7ee-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd7ee-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-117">Not supported.</span></span>    |
|<span data-ttu-id="bd7ee-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd7ee-118">Application</span></span> | <span data-ttu-id="bd7ee-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd7ee-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd7ee-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a><span data-ttu-id="bd7ee-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd7ee-121">Request headers</span></span>
| <span data-ttu-id="bd7ee-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bd7ee-122">Name</span></span>       | <span data-ttu-id="bd7ee-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bd7ee-123">Value</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bd7ee-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd7ee-124">Authorization</span></span>  | <span data-ttu-id="bd7ee-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd7ee-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="bd7ee-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="bd7ee-p105">Строка, представляющая определенный часовой пояс для ответа, например "Тихоокеанское время США (зима)". Необязательный параметр. Время в формате UTC используется, если этот заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p105">A string representing a specific time zone for the response, for example, "Pacific Standard Time". Optional. UTC is used if this header is not specified.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd7ee-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bd7ee-131">Request body</span></span>
<span data-ttu-id="bd7ee-p106">Ниже перечислены все поддерживаемые параметры. В зависимости от сценария, укажите объект JSON для каждого из обязательных параметров в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p106">All the supported parameters are listed below. Depending on your scenario, specify a JSON object for each of the necessary parameters in the request body.</span></span> 


| <span data-ttu-id="bd7ee-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="bd7ee-134">Parameter</span></span>    | <span data-ttu-id="bd7ee-135">Тип</span><span class="sxs-lookup"><span data-stu-id="bd7ee-135">Type</span></span>   |<span data-ttu-id="bd7ee-136">Описание</span><span class="sxs-lookup"><span data-stu-id="bd7ee-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd7ee-137">attendees</span><span class="sxs-lookup"><span data-stu-id="bd7ee-137">attendees</span></span>|<span data-ttu-id="bd7ee-138">Коллекция объектов [attendeeBase](../resources/attendeebase.md)</span><span class="sxs-lookup"><span data-stu-id="bd7ee-138">[attendeeBase](../resources/attendeebase.md) collection</span></span>|<span data-ttu-id="bd7ee-p107">Коллекция участников или ресурсов для собрания. Так как действие findMeetingTimes предполагает, что присутствие всех указанных участников-людей обязательно, укажите значение `required` для людей, а значение `resource` для ресурсов в соответствующем свойстве **type**. Если указана пустая коллекция, метод **findMeetingTimes** ищет свободные периоды времени только для организатора. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p107">A collection of attendees or resources for the meeting. Since findMeetingTimes assumes that any attendee who is a person is always required, specify `required` for a person and `resource` for a resource in the corresponding **type** property. An empty collection causes **findMeetingTimes** to look for free time slots for only the organizer. Optional.</span></span>|
|<span data-ttu-id="bd7ee-143">isOrganizerOptional</span><span class="sxs-lookup"><span data-stu-id="bd7ee-143">isOrganizerOptional</span></span>|<span data-ttu-id="bd7ee-144">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="bd7ee-144">Edm.Boolean</span></span>|<span data-ttu-id="bd7ee-p108">Задайте значение `True`, если присутствие организатора не обязательно. Значение по умолчанию: `false`. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p108">Specify `True` if the organizer doesn't necessarily have to attend. The default is `false`. Optional.</span></span>|
|<span data-ttu-id="bd7ee-148">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="bd7ee-148">locationConstraint</span></span>|[<span data-ttu-id="bd7ee-149">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="bd7ee-149">locationConstraint</span></span>](../resources/locationconstraint.md)|<span data-ttu-id="bd7ee-p109">Требования организатора к месту проведения собрания (например, требуется ли соответствующее предложение или собрание может пройти только в определенных местах). Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p109">The organizer's requirements about the meeting location, such as whether a suggestion for a meeting location is required, or there are specific locations only where the meeting can take place. Optional.</span></span>|
|<span data-ttu-id="bd7ee-152">maxCandidates</span><span class="sxs-lookup"><span data-stu-id="bd7ee-152">maxCandidates</span></span>|<span data-ttu-id="bd7ee-153">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="bd7ee-153">Edm.Int32</span></span>|<span data-ttu-id="bd7ee-p110">Максимальное количество возвращаемых предложений времени проведения собрания. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p110">The maximum number of meeting time suggestions to be returned. Optional.</span></span>|
|<span data-ttu-id="bd7ee-156">meetingDuration</span><span class="sxs-lookup"><span data-stu-id="bd7ee-156">meetingDuration</span></span>|<span data-ttu-id="bd7ee-157">Edm.Duration</span><span class="sxs-lookup"><span data-stu-id="bd7ee-157">Edm.Duration</span></span>|<span data-ttu-id="bd7ee-p111">Продолжительность собрания в формате [ISO8601](https://www.iso.org/iso/iso8601). Например, 1 час обозначается как PT1H, где P обозначает продолжительность, T — время, а H — часы. Используйте букву M, чтобы указать количество минут; например, 2 часа и 30 минут будут обозначаться так: PT2H30M. Если продолжительность собрания не указана, метод **findMeetingTimes** использует значение по умолчанию — 30 минут. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p111">The length of the meeting, denoted in [ISO8601](https://www.iso.org/iso/iso8601) format. For example, 1 hour is denoted as 'PT1H', where 'P' is the duration designator, 'T' is the time designator, and 'H' is the hour designator. Use M to indicate minutes for the duration; for example, 2 hours and 30 minutes would be 'PT2H30M'. If no meeting duration is specified, **findMeetingTimes** uses the default of 30 minutes. Optional.</span></span>|
|<span data-ttu-id="bd7ee-163">minimumAttendeePercentage</span><span class="sxs-lookup"><span data-stu-id="bd7ee-163">minimumAttendeePercentage</span></span>|<span data-ttu-id="bd7ee-164">Edm.Double</span><span class="sxs-lookup"><span data-stu-id="bd7ee-164">Edm.Double</span></span>| <span data-ttu-id="bd7ee-p112">Минимальная [достоверность](#the-confidence-of-a-meeting-suggestion), необходимая, чтобы вернуть период времени в ответе. Это процентное значение от 0 до 100. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p112">The minimum required [confidence](#the-confidence-of-a-meeting-suggestion) for a time slot to be returned in the response. It is a % value ranging from 0 to 100. Optional.</span></span>|
|<span data-ttu-id="bd7ee-168">returnSuggestionReasons</span><span class="sxs-lookup"><span data-stu-id="bd7ee-168">returnSuggestionReasons</span></span>|<span data-ttu-id="bd7ee-169">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="bd7ee-169">Edm.Boolean</span></span>|<span data-ttu-id="bd7ee-p113">Задайте значение `True`, если требуется вернуть причину каждого предложения в свойстве **suggestionReason**. По умолчанию задано значение `false`, и это свойство не возвращается. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p113">Specify `True` to return a reason for each meeting suggestion in the **suggestionReason** property. The default is `false` to not return that property. Optional.</span></span>|
|<span data-ttu-id="bd7ee-173">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="bd7ee-173">timeConstraint</span></span>|[<span data-ttu-id="bd7ee-174">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="bd7ee-174">timeConstraint</span></span>](../resources/timeconstraint.md)|<span data-ttu-id="bd7ee-p114">Ограничения по времени для собрания, к которым могут относиться характер собрания (свойство **activityDomain**) и возможное время проведения собрания (свойство **timeSlots**). Если параметр **activityDomain** не задан, метод **findMeetingTimes** считает, что для него установлено значение `work`. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p114">Any time restrictions for a meeting, which can include the nature of the meeting (**activityDomain** property) and possible meeting time periods (**timeSlots** property). **findMeetingTimes** assumes **activityDomain** as `work` if you don't specify this parameter. Optional.</span></span>|

<span data-ttu-id="bd7ee-178">В таблице ниже описываются ограничения **activityDomain**, которые можно в дальнейшем указать в параметре **timeConstraint**.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-178">The following table describes the **activityDomain** restrictions you can further specify in the **timeConstraint** parameter.</span></span>

|<span data-ttu-id="bd7ee-179">Значение activityDomain</span><span class="sxs-lookup"><span data-stu-id="bd7ee-179">activityDomain value</span></span>|<span data-ttu-id="bd7ee-180">Предложения по времени проведения собраний</span><span class="sxs-lookup"><span data-stu-id="bd7ee-180">Suggestions for meeting times</span></span>|
|:-----|:-----|
|<span data-ttu-id="bd7ee-181">work</span><span class="sxs-lookup"><span data-stu-id="bd7ee-181">work</span></span>| <span data-ttu-id="bd7ee-p115">Предложения ограничиваются рамками рабочего времени пользователя, которое определяется настройками его календаря. Пользователь или администратор также могут изменять рабочее время. По умолчанию рабочим считается время с 8:00 до 17:00 (в часовом поясе, установленном для почтового ящика пользователя) с понедельника по пятницу. Это значение является значением по умолчанию, если не задан параметр **activityDomain**.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p115">Suggestions are within the user's work hours which are defined in the user’s calendar configuration and can be customized by the user or administrator. The default work hours are Monday to Friday, 8am to 5pm in the time zone set for the mailbox. This is the default value if no **activityDomain** is specified.</span></span> |
|<span data-ttu-id="bd7ee-185">personal</span><span class="sxs-lookup"><span data-stu-id="bd7ee-185">personal</span></span>| <span data-ttu-id="bd7ee-p116">Предложения возможны в рабочее время пользователя, а также в субботу и воскресенье. По умолчанию задано время с 8:00 до 17:00 (в часовом поясе, установленном для почтового ящика пользователя) с понедельника по воскресенье.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p116">Suggestions are within the user's work hours, and Saturday and Sunday. The default is Monday to Sunday, 8am to 5pm, in the time zone setting for the mailbox.</span></span>|
|<span data-ttu-id="bd7ee-188">unrestricted</span><span class="sxs-lookup"><span data-stu-id="bd7ee-188">unrestricted</span></span> | <span data-ttu-id="bd7ee-189">Предложения могут относиться к любому времени в любой день недели.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-189">Suggestions can be from all hours of a day, all days of a week.</span></span>|
|<span data-ttu-id="bd7ee-190">unknown</span><span class="sxs-lookup"><span data-stu-id="bd7ee-190">unknown</span></span> | <span data-ttu-id="bd7ee-p117">Не рекомендуем использовать это значение, так как в будущем его поддержка будет прекращена. В настоящее время значение равносильно значению `work`. Измените существующий код, используя соответствующие значения `work`, `personal` или `unrestricted`.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p117">Do not use this value as it will be deprecated in the future. Currently behaves the same as `work`. Change any existing code to use `work`, `personal` or `unrestricted` as appropriate.</span></span>


<span data-ttu-id="bd7ee-p118">В зависимости от указанных параметров, действие **findMeetingTimes** проверяет сведения о доступности в основных календарях организатора и участников. Действие вычисляет наиболее подходящее время собрания и возвращает предложения.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p118">Based on the specified parameters,**findMeetingTimes** checks the free/busy status in the primary calendars of the organizer and attendees. The action calculates the best possible meeting times, and returns any meeting suggestions.</span></span>

## <a name="response"></a><span data-ttu-id="bd7ee-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd7ee-196">Response</span></span>

<span data-ttu-id="bd7ee-197">В случае успеха этот метод возвращает код ответа `200 OK` и объект [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-197">If successful, this method returns `200 OK` response code and a [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) in the response body.</span></span> 

<span data-ttu-id="bd7ee-p119">Объект **meetingTimeSuggestionsResult** включает коллекцию предложений и свойство **emptySuggestionsReason**. Каждое предложение определяется как объект [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), где средняя вероятность присутствия участников составляет 50 % или определенное процентное значение, указанное в параметре **minimumAttendeePercentage**.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p119">A **meetingTimeSuggestionsResult** includes a collection of meeting suggestions and an **emptySuggestionsReason** property. Each suggestion is defined as a [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), with attendees having on the average a confidence level of 50% to attend, or a specific % that you have specified in the **minimumAttendeePercentage** parameter.</span></span> 

<span data-ttu-id="bd7ee-200">По умолчанию каждое предлагаемое время проведения собрания указывается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-200">By default, each meeting time suggestion is returned in UTC.</span></span> 

<span data-ttu-id="bd7ee-p120">Если метод **findMeetingTimes** не может вернуть предложение, то в свойстве **emptySuggestionsReason** будет указана причина. Это значение поможет вам лучше настраивать параметры и снова вызывать метод **findMeetingTimes**.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p120">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

### <a name="the-confidence-of-a-meeting-suggestion"></a><span data-ttu-id="bd7ee-203">Достоверность предложения</span><span class="sxs-lookup"><span data-stu-id="bd7ee-203">The confidence of a meeting suggestion</span></span>

<span data-ttu-id="bd7ee-204">Свойство **confidence** объекта **meetingTimeSuggestion** принимает значения от 0 % до 100 % и представляет вероятность того, что все участники посетят собрание. Она зависит от сведений о доступности каждого участника:</span><span class="sxs-lookup"><span data-stu-id="bd7ee-204">The **confidence** property of a **meetingTimeSuggestion** ranges from 0% to 100%, and represents the chance that all the attendees attend the meeting, based on each of their individual free/busy status:</span></span>

- <span data-ttu-id="bd7ee-205">Если тот или иной участник доступен в указанный период времени, для него задается вероятность посещения 100 %, если его состояние неизвестно — 49 %, а если он занят— 0 %.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-205">For each attendee, a free status for a specified meeting time period corresponds to 100% chance of attendance, unknown status 49%, and busy status 0%.</span></span>
- <span data-ttu-id="bd7ee-206">Достоверность предлагаемого времени собрания вычисляется как средняя вероятность присутствия всех указанных участников собрания.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-206">The confidence of a meeting time suggestion is computed by averaging the chance of attendance over all the attendees specified for that meeting.</span></span>
- <span data-ttu-id="bd7ee-p121">С помощью необязательного параметра **minimumAttendeePercentage** метода **findMeetingTimes** вы можете сделать так, чтобы возвращались предложения со значением достоверности не ниже указанного. Например, вы можете задать для параметра **minimumAttendeePercentage** значение 80 %, если вас интересуют только те предложения, для которых вероятность присутствия всех участников составляет не менее 80 %. Если параметр **minimumAttendeePercentage** не указан, метод **findMeetingTimes** предполагает значение 50 %.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p121">You can use the **minimumAttendeePercentage** optional parameter for **findMeetingTimes** to specify only meeting time suggestions of at least certain confidence level should be returned. For example, you can specify a **minimumAttendeePercentage** of 80% if you want only suggestions that have an 80% chance or more that all the attendees are attending. If you do not specify **minimumAttendeePercentage**, **findMeetingTimes** assumes a value of 50%.</span></span>
- <span data-ttu-id="bd7ee-p122">При наличии нескольких предложений времени действие **findMeetingTimes** сначала сортирует их по убыванию значения достоверности. При наличии нескольких предложений с одинаковой достоверностью это действие сортирует их в хронологическом порядке.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p122">If there are multiple meeting time suggestions, the **findMeetingTimes** action first orders the suggestions by their computed confidence value from high to low. If there are suggestions with the same confidence, the action then orders these suggestions chronologically.</span></span>

<span data-ttu-id="bd7ee-212">Допустим, время проведения собрания предложено с учетом 3 участников со следующими сведениями о доступности:</span><span class="sxs-lookup"><span data-stu-id="bd7ee-212">As an example, if a meeting time suggestion involves 3 attendees with the following free/busy status:</span></span>

|<span data-ttu-id="bd7ee-213">**Участник**</span><span class="sxs-lookup"><span data-stu-id="bd7ee-213">**Attendee**</span></span>|<span data-ttu-id="bd7ee-214">**Сведения о доступности**</span><span class="sxs-lookup"><span data-stu-id="bd7ee-214">**Free/busy status**</span></span>|<span data-ttu-id="bd7ee-215">**Процентная вероятность посещения**</span><span class="sxs-lookup"><span data-stu-id="bd7ee-215">**% Chance of attendance**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bd7ee-216">Дарья</span><span class="sxs-lookup"><span data-stu-id="bd7ee-216">Dana</span></span> | <span data-ttu-id="bd7ee-217">Свободна</span><span class="sxs-lookup"><span data-stu-id="bd7ee-217">Free</span></span> | <span data-ttu-id="bd7ee-218">100 %</span><span class="sxs-lookup"><span data-stu-id="bd7ee-218">100%</span></span> |
|<span data-ttu-id="bd7ee-219">Иван</span><span class="sxs-lookup"><span data-stu-id="bd7ee-219">John</span></span> | <span data-ttu-id="bd7ee-220">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="bd7ee-220">Unknown</span></span> | <span data-ttu-id="bd7ee-221">49 %</span><span class="sxs-lookup"><span data-stu-id="bd7ee-221">49%</span></span> |
|<span data-ttu-id="bd7ee-222">Samantha</span><span class="sxs-lookup"><span data-stu-id="bd7ee-222">Samantha</span></span> | <span data-ttu-id="bd7ee-223">Занята</span><span class="sxs-lookup"><span data-stu-id="bd7ee-223">Busy</span></span> | <span data-ttu-id="bd7ee-224">0 %</span><span class="sxs-lookup"><span data-stu-id="bd7ee-224">0%</span></span> |

<span data-ttu-id="bd7ee-225">В этом случае достоверность предлагаемого времени проведения собрания (средняя вероятность посещения) составляет (100 % + 49 % + 0 %)/3 = 49,66 %.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-225">Then the confidence of the meeting time suggestion, which is the average chance of attendance, is (100% + 49% + 0%)/3 = 49.66%.</span></span>

<span data-ttu-id="bd7ee-226">Если в методе **findMeetingTimes** указать для параметра **minimumAttendeePercentage** значение 80 %, операция не будет предлагать это время в ответе, так как 49,66 % < 80 %.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-226">If you specify a **minimumAttendeePercentage** of 80% in a **findMeetingTimes** operation, because 49.66% < 80%, the operation will not suggest this time in the response.</span></span>

## <a name="example"></a><span data-ttu-id="bd7ee-227">Пример</span><span class="sxs-lookup"><span data-stu-id="bd7ee-227">Example</span></span>

<span data-ttu-id="bd7ee-228">В приведенном ниже примере показано, как найти время для встречи в заранее установленном месте и запросить причину для каждого предложения, указав следующие параметры в тексте запроса:</span><span class="sxs-lookup"><span data-stu-id="bd7ee-228">The following example shows how to find time to meet at a pre-determined location, and request a reason for each suggestion, by specifying the following parameters in the request body:</span></span>

- <span data-ttu-id="bd7ee-229">**attendees**</span><span class="sxs-lookup"><span data-stu-id="bd7ee-229">**attendees**</span></span>
- <span data-ttu-id="bd7ee-230">**locationConstraint**</span><span class="sxs-lookup"><span data-stu-id="bd7ee-230">**locationConstraint**</span></span>
- <span data-ttu-id="bd7ee-231">**timeConstraint**</span><span class="sxs-lookup"><span data-stu-id="bd7ee-231">**timeConstraint**</span></span>
- <span data-ttu-id="bd7ee-232">**isOrganizerOptional**</span><span class="sxs-lookup"><span data-stu-id="bd7ee-232">**isOrganizerOptional**</span></span>
- <span data-ttu-id="bd7ee-233">**meetingDuration**</span><span class="sxs-lookup"><span data-stu-id="bd7ee-233">**meetingDuration**</span></span>
- <span data-ttu-id="bd7ee-234">**returnSuggestionReasons**</span><span class="sxs-lookup"><span data-stu-id="bd7ee-234">**returnSuggestionReasons**</span></span>
- <span data-ttu-id="bd7ee-235">**minimumAttendeePercentage**</span><span class="sxs-lookup"><span data-stu-id="bd7ee-235">**minimumAttendeePercentage**</span></span>

<span data-ttu-id="bd7ee-236">Указав параметр **returnSuggestionReasons**, вы также получите в свойстве **suggestionReason** объяснение для каждого предложения, если метод **findMeetingTimes** возвращает какие-либо предложения.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-236">By setting the **returnSuggestionReasons** parameter, you also get an explanation in the **suggestionReason** property for each suggestion, if **findMeetingTimes** returns any suggestion.</span></span>

<span data-ttu-id="bd7ee-237">Обратите внимание, что в запросе указывается Тихоокеанское время.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-237">Notice that the request specifies time in the PST time zone.</span></span> <span data-ttu-id="bd7ee-238">В ответе по умолчанию возвращаются предложения времени проведения собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-238">By default, the response returns meeting time suggestions in UTC.</span></span> <span data-ttu-id="bd7ee-239">С помощью заголовка запроса `Prefer: outlook.timezone` вы можете сделать так, чтобы в ответе тоже возвращалось Тихоокеанское время.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-239">You can use the `Prefer: outlook.timezone` request header to specify PST as well for the time values in the response.</span></span>

##### <a name="request"></a><span data-ttu-id="bd7ee-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd7ee-240">Request</span></span>
<span data-ttu-id="bd7ee-241">Ниже представлен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-241">Here is the example request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd7ee-242">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd7ee-242">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
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
    "timeslots": [ 
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
# <a name="c"></a>[<span data-ttu-id="bd7ee-243">C#</span><span class="sxs-lookup"><span data-stu-id="bd7ee-243">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-findmeetingtimes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd7ee-244">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd7ee-244">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-findmeetingtimes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd7ee-245">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd7ee-245">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-findmeetingtimes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd7ee-246">Java</span><span class="sxs-lookup"><span data-stu-id="bd7ee-246">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-findmeetingtimes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bd7ee-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd7ee-247">Response</span></span>
<span data-ttu-id="bd7ee-p124">Ниже представлен пример ответа. Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd7ee-p124">Here is an example response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
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
<!-- {
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/user-findmeetingtimes.md:
      Failed to parse any rows out of table with headers: |activityDomain value|Suggestions for meeting times|",
      "Error: user_findmeetingtimes/meetingTimeSuggestions/member/confidence:\r\n
      Expected type Double but actual was Int64. Property: confidence, actual value: '100'",
      "Error: user_findmeetingtimes/meetingTimeSuggestions/member/confidence:\r\n
      Expected type Float but actual was Int64. Property: confidence, actual value: '100'"
  ],
  "tocPath": ""
}-->

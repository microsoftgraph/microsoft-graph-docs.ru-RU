---
title: 'user: findMeetingTimes'
description: Предложите совещаний и на основе доступности организатора и участников и ограничения времени или расположение указан как параметры расположения.
localization_priority: Priority
ms.openlocfilehash: 0eb17aaab4eb8a93ce4a6d1af754ab5f192328fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867979"
---
# <a name="user-findmeetingtimes"></a><span data-ttu-id="f9bbc-103">user: findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="f9bbc-103">user: findMeetingTimes</span></span>
<span data-ttu-id="f9bbc-104">Предложите совещаний и на основе доступности организатора и участников и ограничения времени или расположение указан как параметры расположения.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-104">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints specified as parameters.</span></span>

<span data-ttu-id="f9bbc-p101">Если метод **findMeetingTimes** не может вернуть предложение, то в свойстве **emptySuggestionsReason** будет указана причина. Это значение поможет вам лучше настраивать параметры и снова вызывать метод **findMeetingTimes**.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p101">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>


## <a name="permissions"></a><span data-ttu-id="f9bbc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9bbc-107">Permissions</span></span>
<span data-ttu-id="f9bbc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9bbc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9bbc-110">Permission type</span></span>      | <span data-ttu-id="f9bbc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9bbc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9bbc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9bbc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9bbc-113">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span><span class="sxs-lookup"><span data-stu-id="f9bbc-113">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span></span>    |
|<span data-ttu-id="f9bbc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9bbc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9bbc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-115">Not supported.</span></span>    |
|<span data-ttu-id="f9bbc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9bbc-116">Application</span></span> | <span data-ttu-id="f9bbc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9bbc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9bbc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a><span data-ttu-id="f9bbc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9bbc-119">Request headers</span></span>
| <span data-ttu-id="f9bbc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f9bbc-120">Name</span></span>       | <span data-ttu-id="f9bbc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f9bbc-121">Value</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f9bbc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9bbc-122">Authorization</span></span>  | <span data-ttu-id="f9bbc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9bbc-125">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f9bbc-125">Prefer: outlook.timezone</span></span> | <span data-ttu-id="f9bbc-p104">Строка, представляющая определенный часовой пояс для ответа, например "Тихоокеанское время США (зима)". Необязательный параметр. Время в формате UTC используется, если этот заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p104">A string representing a specific time zone for the response, for example, "Pacific Standard Time". Optional. UTC is used if this header is not specified.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9bbc-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f9bbc-129">Request body</span></span>
<span data-ttu-id="f9bbc-p105">Ниже перечислены все поддерживаемые параметры. В зависимости от сценария, укажите объект JSON для каждого из обязательных параметров в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p105">All the supported parameters are listed below. Depending on your scenario, specify a JSON object for each of the necessary parameters in the request body.</span></span> 


| <span data-ttu-id="f9bbc-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="f9bbc-132">Parameter</span></span>    | <span data-ttu-id="f9bbc-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f9bbc-133">Type</span></span>   |<span data-ttu-id="f9bbc-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f9bbc-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9bbc-135">attendees</span><span class="sxs-lookup"><span data-stu-id="f9bbc-135">attendees</span></span>|<span data-ttu-id="f9bbc-136">Коллекция объектов [attendeeBase](../resources/attendeebase.md)</span><span class="sxs-lookup"><span data-stu-id="f9bbc-136">[attendeeBase](../resources/attendeebase.md) collection</span></span>|<span data-ttu-id="f9bbc-p106">Коллекция участников или ресурсов для собрания. Так как действие findMeetingTimes предполагает, что присутствие всех указанных участников-людей обязательно, укажите значение `required` для людей, а значение `resource` для ресурсов в соответствующем свойстве **type**. Если указана пустая коллекция, метод **findMeetingTimes** ищет свободные периоды времени только для организатора. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p106">A collection of attendees or resources for the meeting. Since findMeetingTimes assumes that any attendee who is a person is always required, specify `required` for a person and `resource` for a resource in the corresponding **type** property. An empty collection causes **findMeetingTimes** to look for free time slots for only the organizer. Optional.</span></span>|
|<span data-ttu-id="f9bbc-141">isOrganizerOptional</span><span class="sxs-lookup"><span data-stu-id="f9bbc-141">isOrganizerOptional</span></span>|<span data-ttu-id="f9bbc-142">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="f9bbc-142">Edm.Boolean</span></span>|<span data-ttu-id="f9bbc-p107">Задайте значение `True`, если присутствие организатора не обязательно. Значение по умолчанию: `false`. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p107">Specify `True` if the organizer doesn't necessarily have to attend. The default is `false`. Optional.</span></span>|
|<span data-ttu-id="f9bbc-146">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="f9bbc-146">locationConstraint</span></span>|[<span data-ttu-id="f9bbc-147">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="f9bbc-147">locationConstraint</span></span>](../resources/locationconstraint.md)|<span data-ttu-id="f9bbc-p108">Требования организатора к месту проведения собрания (например, требуется ли соответствующее предложение или собрание может пройти только в определенных местах). Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p108">The organizer's requirements about the meeting location, such as whether a suggestion for a meeting location is required, or there are specific locations only where the meeting can take place. Optional.</span></span>|
|<span data-ttu-id="f9bbc-150">maxCandidates</span><span class="sxs-lookup"><span data-stu-id="f9bbc-150">maxCandidates</span></span>|<span data-ttu-id="f9bbc-151">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="f9bbc-151">Edm.Int32</span></span>|<span data-ttu-id="f9bbc-p109">Максимальное количество возвращаемых предложений времени проведения собрания. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p109">The maximum number of meeting time suggestions to be returned. Optional.</span></span>|
|<span data-ttu-id="f9bbc-154">meetingDuration</span><span class="sxs-lookup"><span data-stu-id="f9bbc-154">meetingDuration</span></span>|<span data-ttu-id="f9bbc-155">Edm.Duration</span><span class="sxs-lookup"><span data-stu-id="f9bbc-155">Edm.Duration</span></span>|<span data-ttu-id="f9bbc-p110">Продолжительность собрания в формате [ISO8601](https://www.iso.org/iso/iso8601). Например, 1 час обозначается как PT1H, где P обозначает продолжительность, T — время, а H — часы. Используйте букву M, чтобы указать количество минут; например, 2 часа и 30 минут будут обозначаться так: PT2H30M. Если продолжительность собрания не указана, метод **findMeetingTimes** использует значение по умолчанию — 30 минут. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p110">The length of the meeting, denoted in [ISO8601](https://www.iso.org/iso/iso8601) format. For example, 1 hour is denoted as 'PT1H', where 'P' is the duration designator, 'T' is the time designator, and 'H' is the hour designator. Use M to indicate minutes for the duration; for example, 2 hours and 30 minutes would be 'PT2H30M'. If no meeting duration is specified, **findMeetingTimes** uses the default of 30 minutes. Optional.</span></span>|
|<span data-ttu-id="f9bbc-161">minimumAttendeePercentage</span><span class="sxs-lookup"><span data-stu-id="f9bbc-161">minimumAttendeePercentage</span></span>|<span data-ttu-id="f9bbc-162">Edm.Double</span><span class="sxs-lookup"><span data-stu-id="f9bbc-162">Edm.Double</span></span>| <span data-ttu-id="f9bbc-p111">Минимальная [достоверность](#the-confidence-of-a-meeting-suggestion), необходимая, чтобы вернуть период времени в ответе. Это процентное значение от 0 до 100. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p111">The minimum required [confidence](#the-confidence-of-a-meeting-suggestion) for a time slot to be returned in the response. It is a % value ranging from 0 to 100. Optional.</span></span>|
|<span data-ttu-id="f9bbc-166">returnSuggestionReasons</span><span class="sxs-lookup"><span data-stu-id="f9bbc-166">returnSuggestionReasons</span></span>|<span data-ttu-id="f9bbc-167">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="f9bbc-167">Edm.Boolean</span></span>|<span data-ttu-id="f9bbc-p112">Задайте значение `True`, если требуется вернуть причину каждого предложения в свойстве **suggestionReason**. По умолчанию задано значение `false`, и это свойство не возвращается. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p112">Specify `True` to return a reason for each meeting suggestion in the **suggestionReason** property. The default is `false` to not return that property. Optional.</span></span>|
|<span data-ttu-id="f9bbc-171">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="f9bbc-171">timeConstraint</span></span>|[<span data-ttu-id="f9bbc-172">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="f9bbc-172">timeConstraint</span></span>](../resources/timeconstraint.md)|<span data-ttu-id="f9bbc-p113">Ограничения по времени для собрания, к которым могут относиться характер собрания (свойство **activityDomain**) и возможное время проведения собрания (свойство **timeSlots**). Если параметр **activityDomain** не задан, метод **findMeetingTimes** считает, что для него установлено значение `work`. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p113">Any time restrictions for a meeting, which can include the nature of the meeting (**activityDomain** property) and possible meeting time periods (**timeSlots** property). **findMeetingTimes** assumes **activityDomain** as `work` if you don't specify this parameter. Optional.</span></span>|

<span data-ttu-id="f9bbc-176">В следующей таблице описаны ограничения **activityDomain** , которые можно указать в параметре **timeConstraint** .</span><span class="sxs-lookup"><span data-stu-id="f9bbc-176">The following table describes the **activityDomain** restrictions you can further specify in the **timeConstraint** parameter.</span></span>

|<span data-ttu-id="f9bbc-177">значение activityDomain</span><span class="sxs-lookup"><span data-stu-id="f9bbc-177">activityDomain value</span></span>|<span data-ttu-id="f9bbc-178">Предложения по времени проведения собраний</span><span class="sxs-lookup"><span data-stu-id="f9bbc-178">Suggestions for meeting times</span></span>|
|:-----|:-----|
|<span data-ttu-id="f9bbc-179">трудозатраты</span><span class="sxs-lookup"><span data-stu-id="f9bbc-179">work</span></span>| <span data-ttu-id="f9bbc-p114">Предложения ограничиваются рамками рабочего времени пользователя, которое определяется настройками его календаря. Пользователь или администратор также могут изменять рабочее время. По умолчанию рабочим считается время с 8:00 до 17:00 (в часовом поясе, установленном для почтового ящика пользователя) с понедельника по пятницу. Это значение является значением по умолчанию, если не задан параметр **activityDomain**.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p114">Suggestions are within the user's work hours which are defined in the user’s calendar configuration and can be customized by the user or administrator. The default work hours are Monday to Friday, 8am to 5pm in the time zone set for the mailbox. This is the default value if no **activityDomain** is specified.</span></span> |
|<span data-ttu-id="f9bbc-183">personal</span><span class="sxs-lookup"><span data-stu-id="f9bbc-183">personal</span></span>| <span data-ttu-id="f9bbc-p115">Предложения возможны в рабочее время пользователя, а также в субботу и воскресенье. По умолчанию задано время с 8:00 до 17:00 (в часовом поясе, установленном для почтового ящика пользователя) с понедельника по воскресенье.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p115">Suggestions are within the user's work hours, and Saturday and Sunday. The default is Monday to Sunday, 8am to 5pm, in the time zone setting for the mailbox.</span></span>|
|<span data-ttu-id="f9bbc-186">unrestricted</span><span class="sxs-lookup"><span data-stu-id="f9bbc-186">unrestricted</span></span> | <span data-ttu-id="f9bbc-187">Предложения могут относиться к любому времени в любой день недели.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-187">Suggestions can be from all hours of a day, all days of a week.</span></span>|
|<span data-ttu-id="f9bbc-188">unknown</span><span class="sxs-lookup"><span data-stu-id="f9bbc-188">unknown</span></span> | <span data-ttu-id="f9bbc-p116">Не рекомендуем использовать это значение, так как в будущем его поддержка будет прекращена. В настоящее время значение равносильно значению `work`. Измените существующий код, используя соответствующие значения `work`, `personal` или `unrestricted`.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p116">Do not use this value as it will be deprecated in the future. Currently behaves the same as `work`. Change any existing code to use `work`, `personal` or `unrestricted` as appropriate.</span></span>


<span data-ttu-id="f9bbc-p117">В зависимости от указанных параметров, действие **findMeetingTimes** проверяет сведения о доступности в основных календарях организатора и участников. Действие вычисляет наиболее подходящее время собрания и возвращает предложения.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p117">Based on the specified parameters,**findMeetingTimes** checks the free/busy status in the primary calendars of the organizer and attendees. The action calculates the best possible meeting times, and returns any meeting suggestions.</span></span>

## <a name="response"></a><span data-ttu-id="f9bbc-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9bbc-194">Response</span></span>

<span data-ttu-id="f9bbc-195">В случае успеха этот метод возвращает код ответа `200 OK` и объект [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-195">If successful, this method returns `200 OK` response code and a [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) in the response body.</span></span> 

<span data-ttu-id="f9bbc-p118">Объект **meetingTimeSuggestionsResult** включает коллекцию предложений и свойство **emptySuggestionsReason**. Каждое предложение определяется как объект [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), где средняя вероятность присутствия участников составляет 50 % или определенное процентное значение, указанное в параметре **minimumAttendeePercentage**.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p118">A **meetingTimeSuggestionsResult** includes a collection of meeting suggestions and an **emptySuggestionsReason** property. Each suggestion is defined as a [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), with attendees having on the average a confidence level of 50% to attend, or a specific % that you have specified in the **minimumAttendeePercentage** parameter.</span></span> 

<span data-ttu-id="f9bbc-198">По умолчанию каждое предлагаемое время проведения собрания указывается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-198">By default, each meeting time suggestion is returned in UTC.</span></span> 

<span data-ttu-id="f9bbc-p119">Если метод **findMeetingTimes** не может вернуть предложение, то в свойстве **emptySuggestionsReason** будет указана причина. Это значение поможет вам лучше настраивать параметры и снова вызывать метод **findMeetingTimes**.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p119">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

### <a name="the-confidence-of-a-meeting-suggestion"></a><span data-ttu-id="f9bbc-201">Достоверность предложения</span><span class="sxs-lookup"><span data-stu-id="f9bbc-201">The confidence of a meeting suggestion</span></span>

<span data-ttu-id="f9bbc-202">Свойство **confidence** объекта **meetingTimeSuggestion** принимает значения от 0 % до 100 % и представляет вероятность того, что все участники посетят собрание. Она зависит от сведений о доступности каждого участника:</span><span class="sxs-lookup"><span data-stu-id="f9bbc-202">The **confidence** property of a **meetingTimeSuggestion** ranges from 0% to 100%, and represents the chance that all the attendees attend the meeting, based on each of their individual free/busy status:</span></span>

- <span data-ttu-id="f9bbc-203">Если тот или иной участник доступен в указанный период времени, для него задается вероятность посещения 100 %, если его состояние неизвестно — 49 %, а если он занят— 0 %.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-203">For each attendee, a free status for a specified meeting time period corresponds to 100% chance of attendance, unknown status 49%, and busy status 0%.</span></span>
- <span data-ttu-id="f9bbc-204">Достоверность предлагаемого времени собрания вычисляется как средняя вероятность присутствия всех указанных участников собрания.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-204">The confidence of a meeting time suggestion is computed by averaging the chance of attendance over all the attendees specified for that meeting.</span></span>
- <span data-ttu-id="f9bbc-p120">С помощью необязательного параметра **minimumAttendeePercentage** метода **findMeetingTimes** вы можете сделать так, чтобы возвращались предложения со значением достоверности не ниже указанного. Например, вы можете задать для параметра **minimumAttendeePercentage** значение 80 %, если вас интересуют только те предложения, для которых вероятность присутствия всех участников составляет не менее 80 %. Если параметр **minimumAttendeePercentage** не указан, метод **findMeetingTimes** предполагает значение 50 %.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p120">You can use the **minimumAttendeePercentage** optional parameter for **findMeetingTimes** to specify only meeting time suggestions of at least certain confidence level should be returned. For example, you can specify a **minimumAttendeePercentage** of 80% if you want only suggestions that have an 80% chance or more that all the attendees are attending. If you do not specify **minimumAttendeePercentage**, **findMeetingTimes** assumes a value of 50%.</span></span>
- <span data-ttu-id="f9bbc-p121">При наличии нескольких предложений времени действие **findMeetingTimes** сначала сортирует их по убыванию значения достоверности. При наличии нескольких предложений с одинаковой достоверностью это действие сортирует их в хронологическом порядке.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p121">If there are multiple meeting time suggestions, the **findMeetingTimes** action first orders the suggestions by their computed confidence value from high to low. If there are suggestions with the same confidence, the action then orders these suggestions chronologically.</span></span>

<span data-ttu-id="f9bbc-210">Допустим, время проведения собрания предложено с учетом 3 участников со следующими сведениями о доступности:</span><span class="sxs-lookup"><span data-stu-id="f9bbc-210">As an example, if a meeting time suggestion involves 3 attendees with the following free/busy status:</span></span>

|<span data-ttu-id="f9bbc-211">**Участник**</span><span class="sxs-lookup"><span data-stu-id="f9bbc-211">**Attendee**</span></span>|<span data-ttu-id="f9bbc-212">**Сведения о доступности**</span><span class="sxs-lookup"><span data-stu-id="f9bbc-212">**Free/busy status**</span></span>|<span data-ttu-id="f9bbc-213">**Процентная вероятность посещения**</span><span class="sxs-lookup"><span data-stu-id="f9bbc-213">**% Chance of attendance**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f9bbc-214">Дарья</span><span class="sxs-lookup"><span data-stu-id="f9bbc-214">Dana</span></span> | <span data-ttu-id="f9bbc-215">Свободна</span><span class="sxs-lookup"><span data-stu-id="f9bbc-215">Free</span></span> | <span data-ttu-id="f9bbc-216">100 %</span><span class="sxs-lookup"><span data-stu-id="f9bbc-216">100%</span></span> |
|<span data-ttu-id="f9bbc-217">Иван</span><span class="sxs-lookup"><span data-stu-id="f9bbc-217">John</span></span> | <span data-ttu-id="f9bbc-218">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="f9bbc-218">Unknown</span></span> | <span data-ttu-id="f9bbc-219">49 %</span><span class="sxs-lookup"><span data-stu-id="f9bbc-219">49%</span></span> |
|<span data-ttu-id="f9bbc-220">Samantha</span><span class="sxs-lookup"><span data-stu-id="f9bbc-220">Samantha</span></span> | <span data-ttu-id="f9bbc-221">Занята</span><span class="sxs-lookup"><span data-stu-id="f9bbc-221">Busy</span></span> | <span data-ttu-id="f9bbc-222">0 %</span><span class="sxs-lookup"><span data-stu-id="f9bbc-222">0%</span></span> |

<span data-ttu-id="f9bbc-223">В этом случае достоверность предлагаемого времени проведения собрания (средняя вероятность посещения) составляет (100 % + 49 % + 0 %)/3 = 49,66 %.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-223">Then the confidence of the meeting time suggestion, which is the average chance of attendance, is (100% + 49% + 0%)/3 = 49.66%.</span></span>

<span data-ttu-id="f9bbc-224">Если в методе **findMeetingTimes** указать для параметра **minimumAttendeePercentage** значение 80 %, операция не будет предлагать это время в ответе, так как 49,66 % < 80 %.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-224">If you specify a **minimumAttendeePercentage** of 80% in a **findMeetingTimes** operation, because 49.66% < 80%, the operation will not suggest this time in the response.</span></span>

## <a name="example"></a><span data-ttu-id="f9bbc-225">Пример</span><span class="sxs-lookup"><span data-stu-id="f9bbc-225">Example</span></span>

<span data-ttu-id="f9bbc-226">В приведенном ниже примере показано, как найти время для встречи в заранее установленном месте и запросить причину для каждого предложения, указав следующие параметры в тексте запроса:</span><span class="sxs-lookup"><span data-stu-id="f9bbc-226">The following example shows how to find time to meet at a pre-determined location, and request a reason for each suggestion, by specifying the following parameters in the request body:</span></span>

- <span data-ttu-id="f9bbc-227">**attendees**</span><span class="sxs-lookup"><span data-stu-id="f9bbc-227">**attendees**</span></span>
- <span data-ttu-id="f9bbc-228">**locationConstraint**</span><span class="sxs-lookup"><span data-stu-id="f9bbc-228">**locationConstraint**</span></span>
- <span data-ttu-id="f9bbc-229">**timeConstraint**</span><span class="sxs-lookup"><span data-stu-id="f9bbc-229">**timeConstraint**</span></span>
- <span data-ttu-id="f9bbc-230">**meetingDuration**</span><span class="sxs-lookup"><span data-stu-id="f9bbc-230">**meetingDuration**</span></span>
- <span data-ttu-id="f9bbc-231">**returnSuggestionReasons**</span><span class="sxs-lookup"><span data-stu-id="f9bbc-231">**returnSuggestionReasons**</span></span>
- <span data-ttu-id="f9bbc-232">**minimumAttendeePercentage**</span><span class="sxs-lookup"><span data-stu-id="f9bbc-232">**minimumAttendeePercentage**</span></span>

<span data-ttu-id="f9bbc-233">Указав параметр **returnSuggestionReasons**, вы также получите в свойстве **suggestionReason** объяснение для каждого предложения, если метод **findMeetingTimes** возвращает какие-либо предложения.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-233">By setting the **returnSuggestionReasons** parameter, you also get an explanation in the **suggestionReason** property for each suggestion, if **findMeetingTimes** returns any suggestion.</span></span>

<span data-ttu-id="f9bbc-p122">Обратите внимание, что в этом запросе указывается Тихоокеанское время, а в ответе по умолчанию возвращаются предложения времени в формате UTC. С помощью заголовка запроса `Prefer: outlook.timezone` вы можете сделать так, чтобы в ответе тоже возвращалось Тихоокеанское время.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p122">Notice that the request specifies time in the PST time zone, and the response returns meeting time suggestions in UTC, by default. You can use the `Prefer: outlook.timezone` request header to specify PST as well for the time values in the response.</span></span>

##### <a name="request"></a><span data-ttu-id="f9bbc-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9bbc-236">Request</span></span>
<span data-ttu-id="f9bbc-237">Ниже представлен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-237">Here is the example request.</span></span>
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
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
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
    "activityDomain":"unrestricted", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-17T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-19T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": 100.0
}
```

##### <a name="response"></a><span data-ttu-id="f9bbc-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9bbc-238">Response</span></span>
<span data-ttu-id="f9bbc-p123">Ниже представлен пример ответа. Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9bbc-p123">Here is an example response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
Content-Length: 976

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"",
    "meetingTimeSuggestions":[
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-17T18:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-17T20:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        },
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-17T20:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-17T22:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
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
      Failed to parse any rows out of table with headers: |activityDomain value|Suggestions for meeting times|"
  ],
  "tocPath": ""
}-->

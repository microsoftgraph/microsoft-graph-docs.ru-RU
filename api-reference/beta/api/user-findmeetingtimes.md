---
title: 'user: findMeetingTimes'
description: ПредЛожите время и расположения собраний на основе доступности организатора и участников, а также ограничений времени или расположения, заданных в качестве параметров.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 345b42690644fb94a2b6b2bdf6b3cfcc9ead6333
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057059"
---
# <a name="user-findmeetingtimes"></a><span data-ttu-id="cde65-103">user: findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="cde65-103">user: findMeetingTimes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cde65-104">ПредЛожите время и расположения собраний на основе доступности организатора и участников, а также ограничений времени или расположения, заданных в качестве параметров.</span><span class="sxs-lookup"><span data-stu-id="cde65-104">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints specified as parameters.</span></span>

<span data-ttu-id="cde65-p101">Если метод **findMeetingTimes** не может вернуть предложение, то в свойстве **emptySuggestionsReason** будет указана причина. Это значение поможет вам лучше настраивать параметры и снова вызывать метод **findMeetingTimes**.</span><span class="sxs-lookup"><span data-stu-id="cde65-p101">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>


## <a name="permissions"></a><span data-ttu-id="cde65-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cde65-107">Permissions</span></span>
<span data-ttu-id="cde65-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cde65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cde65-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cde65-110">Permission type</span></span>      | <span data-ttu-id="cde65-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cde65-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cde65-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cde65-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cde65-113">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span><span class="sxs-lookup"><span data-stu-id="cde65-113">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span></span>    |
|<span data-ttu-id="cde65-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cde65-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cde65-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cde65-115">Not supported.</span></span>    |
|<span data-ttu-id="cde65-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cde65-116">Application</span></span> | <span data-ttu-id="cde65-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cde65-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cde65-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cde65-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a><span data-ttu-id="cde65-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cde65-119">Request headers</span></span>
| <span data-ttu-id="cde65-120">Имя</span><span class="sxs-lookup"><span data-stu-id="cde65-120">Name</span></span>       | <span data-ttu-id="cde65-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cde65-121">Value</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cde65-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cde65-122">Authorization</span></span>  | <span data-ttu-id="cde65-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cde65-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cde65-125">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="cde65-125">Prefer: outlook.timezone</span></span> | <span data-ttu-id="cde65-p104">Строка, представляющая определенный часовой пояс для ответа, например "Тихоокеанское время США (зима)". Необязательный параметр. Время в формате UTC используется, если этот заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="cde65-p104">A string representing a specific time zone for the response, for example, "Pacific Standard Time". Optional. UTC is used if this header is not specified.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cde65-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cde65-129">Request body</span></span>
<span data-ttu-id="cde65-p105">Ниже перечислены все поддерживаемые параметры. В зависимости от сценария, укажите объект JSON для каждого из обязательных параметров в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="cde65-p105">All the supported parameters are listed below. Depending on your scenario, specify a JSON object for each of the necessary parameters in the request body.</span></span> 


| <span data-ttu-id="cde65-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="cde65-132">Parameter</span></span>    | <span data-ttu-id="cde65-133">Тип</span><span class="sxs-lookup"><span data-stu-id="cde65-133">Type</span></span>   |<span data-ttu-id="cde65-134">Описание</span><span class="sxs-lookup"><span data-stu-id="cde65-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cde65-135">attendees</span><span class="sxs-lookup"><span data-stu-id="cde65-135">attendees</span></span>|<span data-ttu-id="cde65-136">Коллекция [аттендидатамодел](../resources/attendeedatamodel.md)</span><span class="sxs-lookup"><span data-stu-id="cde65-136">[attendeeDataModel](../resources/attendeedatamodel.md) collection</span></span>|<span data-ttu-id="cde65-137">Коллекция участников или ресурсов собрания.</span><span class="sxs-lookup"><span data-stu-id="cde65-137">A collection of attendees or resources for the meeting.</span></span> <span data-ttu-id="cde65-138">В соответствующем свойстве **введите** или `required` `optional` выберите для человека и для `resource` ресурса, например комнаты для собраний.</span><span class="sxs-lookup"><span data-stu-id="cde65-138">In the corresponding **type** property, specify `required` or `optional` for a person and `resource` for a resource like meeting room.</span></span> <span data-ttu-id="cde65-139">Если этот параметр не \*\*\*\* указан, `required` findMeetingTimes предполагается для свойства **Type** .</span><span class="sxs-lookup"><span data-stu-id="cde65-139">If not specified, **findMeetingTimes** assumes `required` for the **type** property.</span></span> <span data-ttu-id="cde65-140">Пустая коллекция приводит к тому, что **findMeetingTimes** ищет свободные интервалы времени только для организатора.</span><span class="sxs-lookup"><span data-stu-id="cde65-140">An empty collection causes **findMeetingTimes** to look for free time slots for only the organizer.</span></span> <span data-ttu-id="cde65-141">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="cde65-141">Optional.</span></span>|
|<span data-ttu-id="cde65-142">isOrganizerOptional</span><span class="sxs-lookup"><span data-stu-id="cde65-142">isOrganizerOptional</span></span>|<span data-ttu-id="cde65-143">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="cde65-143">Edm.Boolean</span></span>|<span data-ttu-id="cde65-p107">Задайте значение `True`, если присутствие организатора не обязательно. Значение по умолчанию: `false`. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cde65-p107">Specify `True` if the organizer doesn't necessarily have to attend. The default is `false`. Optional.</span></span>|
|<span data-ttu-id="cde65-147">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="cde65-147">locationConstraint</span></span>|[<span data-ttu-id="cde65-148">Локатионконстраинтс</span><span class="sxs-lookup"><span data-stu-id="cde65-148">locationConstraints</span></span>](../resources/locationconstraints.md)|<span data-ttu-id="cde65-p108">Требования организатора к месту проведения собрания (например, требуется ли соответствующее предложение или собрание может пройти только в определенных местах). Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cde65-p108">The organizer's requirements about the meeting location, such as whether a suggestion for a meeting location is required, or there are specific locations only where the meeting can take place. Optional.</span></span>|
|<span data-ttu-id="cde65-151">maxCandidates</span><span class="sxs-lookup"><span data-stu-id="cde65-151">maxCandidates</span></span>|<span data-ttu-id="cde65-152">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="cde65-152">Edm.Int32</span></span>|<span data-ttu-id="cde65-p109">Максимальное количество возвращаемых предложений времени проведения собрания. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cde65-p109">The maximum number of meeting time suggestions to be returned. Optional.</span></span>|
|<span data-ttu-id="cde65-155">meetingDuration</span><span class="sxs-lookup"><span data-stu-id="cde65-155">meetingDuration</span></span>|<span data-ttu-id="cde65-156">Edm.Duration</span><span class="sxs-lookup"><span data-stu-id="cde65-156">Edm.Duration</span></span>|<span data-ttu-id="cde65-157">Длительность собрания, обозначенная в формате [ISO 8601](https://www.iso.org/iso/iso8601) .</span><span class="sxs-lookup"><span data-stu-id="cde65-157">The length of the meeting, denoted in [ISO 8601](https://www.iso.org/iso/iso8601) format.</span></span> <span data-ttu-id="cde65-158">Например, 1 час обозначается как "PT1H", где "P" — это обозначение длительности, а "H" — обозначение часа.</span><span class="sxs-lookup"><span data-stu-id="cde65-158">For example, 1 hour is denoted as 'PT1H', where 'P' is the duration designator, 'T' is the time designator, and 'H' is the hour designator.</span></span> <span data-ttu-id="cde65-159">Используйте M, чтобы указать минуты для длительности; Например, 2 часа и 30 минут будут иметь вид "PT2H30M".</span><span class="sxs-lookup"><span data-stu-id="cde65-159">Use M to indicate minutes for the duration; for example, 2 hours and 30 minutes would be 'PT2H30M'.</span></span> <span data-ttu-id="cde65-160">Если длительность собрания не указана, **findMeetingTimes** использует значение по умолчанию, равное 30 минутам.</span><span class="sxs-lookup"><span data-stu-id="cde65-160">If no meeting duration is specified, **findMeetingTimes** uses the default of 30 minutes.</span></span> <span data-ttu-id="cde65-161">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="cde65-161">Optional.</span></span>|
|<span data-ttu-id="cde65-162">minimumAttendeePercentage</span><span class="sxs-lookup"><span data-stu-id="cde65-162">minimumAttendeePercentage</span></span>|<span data-ttu-id="cde65-163">Edm.Double</span><span class="sxs-lookup"><span data-stu-id="cde65-163">Edm.Double</span></span>| <span data-ttu-id="cde65-p111">Минимальная [достоверность](#the-confidence-of-a-meeting-suggestion), необходимая, чтобы вернуть период времени в ответе. Это процентное значение от 0 до 100. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cde65-p111">The minimum required [confidence](#the-confidence-of-a-meeting-suggestion) for a time slot to be returned in the response. It is a % value ranging from 0 to 100. Optional.</span></span>|
|<span data-ttu-id="cde65-167">returnSuggestionReasons</span><span class="sxs-lookup"><span data-stu-id="cde65-167">returnSuggestionReasons</span></span>|<span data-ttu-id="cde65-168">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="cde65-168">Edm.Boolean</span></span>|<span data-ttu-id="cde65-p112">Задайте значение `True`, если требуется вернуть причину каждого предложения в свойстве **suggestionReason**. По умолчанию задано значение `false`, и это свойство не возвращается. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cde65-p112">Specify `True` to return a reason for each meeting suggestion in the **suggestionReason** property. The default is `false` to not return that property. Optional.</span></span>|
|<span data-ttu-id="cde65-172">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="cde65-172">timeConstraint</span></span>|[<span data-ttu-id="cde65-173">Финдмитингтиместимеконстраинтс</span><span class="sxs-lookup"><span data-stu-id="cde65-173">findMeetingTimesTimeConstraints</span></span>](../resources/findmeetingtimestimeconstraints.md)|<span data-ttu-id="cde65-p113">Ограничения по времени для собрания, к которым могут относиться характер собрания (свойство **activityDomain**) и возможное время проведения собрания (свойство **timeSlots**). Если параметр **activityDomain** не задан, метод **findMeetingTimes** считает, что для него установлено значение `work`. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cde65-p113">Any time restrictions for a meeting, which can include the nature of the meeting (**activityDomain** property) and possible meeting time periods (**timeSlots** property). **findMeetingTimes** assumes **activityDomain** as `work` if you don't specify this parameter. Optional.</span></span>|

<span data-ttu-id="cde65-177">В таблице ниже описываются ограничения, которые можно в дальнейшем указать в параметре **timeConstraint**.</span><span class="sxs-lookup"><span data-stu-id="cde65-177">The following table describes the restrictions you can further specify in the **timeConstraint** parameter.</span></span>

|<span data-ttu-id="cde65-178">Значение activityDomain в параметре timeConstraint</span><span class="sxs-lookup"><span data-stu-id="cde65-178">activityDomain value in timeConstraint</span></span>|<span data-ttu-id="cde65-179">Предложения по времени проведения собраний</span><span class="sxs-lookup"><span data-stu-id="cde65-179">Suggestions for meeting times</span></span>|
|:-----|:-----|
|<span data-ttu-id="cde65-180">трудозатраты</span><span class="sxs-lookup"><span data-stu-id="cde65-180">work</span></span>| <span data-ttu-id="cde65-p114">Предложения ограничиваются рамками рабочего времени пользователя, которое определяется настройками его календаря. Пользователь или администратор также могут изменять рабочее время. По умолчанию рабочим считается время с 8:00 до 17:00 (в часовом поясе, установленном для почтового ящика пользователя) с понедельника по пятницу. Это значение является значением по умолчанию, если не задан параметр **activityDomain**.</span><span class="sxs-lookup"><span data-stu-id="cde65-p114">Suggestions are within the user's work hours which are defined in the user’s calendar configuration and can be customized by the user or administrator. The default work hours are Monday to Friday, 8am to 5pm in the time zone set for the mailbox. This is the default value if no **activityDomain** is specified.</span></span> |
|<span data-ttu-id="cde65-184">personal</span><span class="sxs-lookup"><span data-stu-id="cde65-184">personal</span></span>| <span data-ttu-id="cde65-p115">Предложения возможны в рабочее время пользователя, а также в субботу и воскресенье. По умолчанию задано время с 8:00 до 17:00 (в часовом поясе, установленном для почтового ящика пользователя) с понедельника по воскресенье.</span><span class="sxs-lookup"><span data-stu-id="cde65-p115">Suggestions are within the user's work hours, and Saturday and Sunday. The default is Monday to Sunday, 8am to 5pm, in the time zone setting for the mailbox.</span></span>|
|<span data-ttu-id="cde65-187">unrestricted</span><span class="sxs-lookup"><span data-stu-id="cde65-187">unrestricted</span></span> | <span data-ttu-id="cde65-188">Предложения могут относиться к любому времени в любой день недели.</span><span class="sxs-lookup"><span data-stu-id="cde65-188">Suggestions can be from all hours of a day, all days of a week.</span></span>|
|<span data-ttu-id="cde65-189">unknown</span><span class="sxs-lookup"><span data-stu-id="cde65-189">unknown</span></span> | <span data-ttu-id="cde65-p116">Не рекомендуем использовать это значение, так как в будущем его поддержка будет прекращена. В настоящее время значение равносильно значению `work`. Измените существующий код, используя соответствующие значения `work`, `personal` или `unrestricted`.</span><span class="sxs-lookup"><span data-stu-id="cde65-p116">Do not use this value as it will be deprecated in the future. Currently behaves the same as `work`. Change any existing code to use `work`, `personal` or `unrestricted` as appropriate.</span></span>|


<span data-ttu-id="cde65-p117">В зависимости от указанных параметров, действие **findMeetingTimes** проверяет сведения о доступности в основных календарях организатора и участников. Действие вычисляет наиболее подходящее время собрания и возвращает предложения.</span><span class="sxs-lookup"><span data-stu-id="cde65-p117">Based on the specified parameters,**findMeetingTimes** checks the free/busy status in the primary calendars of the organizer and attendees. The action calculates the best possible meeting times, and returns any meeting suggestions.</span></span>

## <a name="response"></a><span data-ttu-id="cde65-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="cde65-195">Response</span></span>

<span data-ttu-id="cde65-196">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [финдмитингтимесреспонсе](../resources/findmeetingtimesresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cde65-196">If successful, this method returns `200 OK` response code and a [findMeetingTimesResponse](../resources/findmeetingtimesresponse.md) in the response body.</span></span> 

<span data-ttu-id="cde65-197">**Финдмитингтимесреспонсе** включает коллекцию предложений о собраниях и свойство **емптисугжестионсреасон** .</span><span class="sxs-lookup"><span data-stu-id="cde65-197">A **findMeetingTimesResponse** includes a collection of meeting suggestions and an **emptySuggestionsReason** property.</span></span> <span data-ttu-id="cde65-198">Каждое предложение определено как [митингтимесугжестион](../resources/meetingtimesuggestion.md), с участниками, у которых средний уровень вероятности 50% для участия, или определенным%, указанным в параметре **minimumAttendeePercentage** .</span><span class="sxs-lookup"><span data-stu-id="cde65-198">Each suggestion is defined as a [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), with attendees having on the average a confidence level of 50% to attend, or a specific % that you have specified in the **minimumAttendeePercentage** parameter.</span></span> 

<span data-ttu-id="cde65-199">По умолчанию каждое предлагаемое время проведения собрания указывается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="cde65-199">By default, each meeting time suggestion is returned in UTC.</span></span> 

<span data-ttu-id="cde65-p119">Если метод **findMeetingTimes** не может вернуть предложение, то в свойстве **emptySuggestionsReason** будет указана причина. Это значение поможет вам лучше настраивать параметры и снова вызывать метод **findMeetingTimes**.</span><span class="sxs-lookup"><span data-stu-id="cde65-p119">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

### <a name="the-confidence-of-a-meeting-suggestion"></a><span data-ttu-id="cde65-202">Достоверность предложения</span><span class="sxs-lookup"><span data-stu-id="cde65-202">The confidence of a meeting suggestion</span></span>

<span data-ttu-id="cde65-203">Свойство **confidence** объекта **meetingTimeSuggestion** принимает значения от 0 % до 100 % и представляет вероятность того, что все участники посетят собрание. Она зависит от сведений о доступности каждого участника:</span><span class="sxs-lookup"><span data-stu-id="cde65-203">The **confidence** property of a **meetingTimeSuggestion** ranges from 0% to 100%, and represents the chance that all the attendees attend the meeting, based on each of their individual free/busy status:</span></span>

- <span data-ttu-id="cde65-204">Если тот или иной участник доступен в указанный период времени, для него задается вероятность посещения 100 %, если его состояние неизвестно — 49 %, а если он занят— 0 %.</span><span class="sxs-lookup"><span data-stu-id="cde65-204">For each attendee, a free status for a specified meeting time period corresponds to 100% chance of attendance, unknown status 49%, and busy status 0%.</span></span>
- <span data-ttu-id="cde65-205">Достоверность предлагаемого времени собрания вычисляется как средняя вероятность присутствия всех указанных участников собрания.</span><span class="sxs-lookup"><span data-stu-id="cde65-205">The confidence of a meeting time suggestion is computed by averaging the chance of attendance over all the attendees specified for that meeting.</span></span>
- <span data-ttu-id="cde65-p120">При наличии нескольких предложений времени действие **findMeetingTimes** сначала сортирует их по убыванию значения достоверности. При наличии нескольких предложений с одинаковой достоверностью это действие сортирует их в хронологическом порядке.</span><span class="sxs-lookup"><span data-stu-id="cde65-p120">If there are multiple meeting time suggestions, the **findMeetingTimes** action first orders the suggestions by their computed confidence value from high to low. If there are suggestions with the same confidence, the action then orders these suggestions chronologically.</span></span>
- <span data-ttu-id="cde65-p121">С помощью необязательного параметра **minimumAttendeePercentage** метода **findMeetingTimes** вы можете сделать так, чтобы возвращались предложения со значением достоверности не ниже указанного. Например, вы можете задать для параметра **minimumAttendeePercentage** значение 80 %, если вас интересуют только те предложения, для которых вероятность присутствия всех участников составляет не менее 80 %. Если параметр **minimumAttendeePercentage** не указан, метод **findMeetingTimes** предполагает значение 50 %.</span><span class="sxs-lookup"><span data-stu-id="cde65-p121">You can use the **minimumAttendeePercentage** optional parameter for **findMeetingTimes** to specify only meeting time suggestions of at least certain confidence level should be returned. For example, you can specify a **minimumAttendeePercentage** of 80% if you want only suggestions that have an 80% chance or more that all the attendees are attending. If you do not specify **minimumAttendeePercentage**, **findMeetingTimes** assumes a value of 50%.</span></span>

<span data-ttu-id="cde65-211">Допустим, время проведения собрания предложено с учетом 3 участников со следующими сведениями о доступности:</span><span class="sxs-lookup"><span data-stu-id="cde65-211">As an example, if a meeting time suggestion involves 3 attendees with the following free/busy status:</span></span>

|<span data-ttu-id="cde65-212">**Участник**</span><span class="sxs-lookup"><span data-stu-id="cde65-212">**Attendee**</span></span>|<span data-ttu-id="cde65-213">**Сведения о доступности**</span><span class="sxs-lookup"><span data-stu-id="cde65-213">**Free/busy status**</span></span>|<span data-ttu-id="cde65-214">**Процентная вероятность посещения**</span><span class="sxs-lookup"><span data-stu-id="cde65-214">**% Chance of attendance**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cde65-215">Дарья</span><span class="sxs-lookup"><span data-stu-id="cde65-215">Dana</span></span> | <span data-ttu-id="cde65-216">Свободна</span><span class="sxs-lookup"><span data-stu-id="cde65-216">Free</span></span> | <span data-ttu-id="cde65-217">100 %</span><span class="sxs-lookup"><span data-stu-id="cde65-217">100%</span></span> |
|<span data-ttu-id="cde65-218">Иван</span><span class="sxs-lookup"><span data-stu-id="cde65-218">John</span></span> | <span data-ttu-id="cde65-219">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="cde65-219">Unknown</span></span> | <span data-ttu-id="cde65-220">49 %</span><span class="sxs-lookup"><span data-stu-id="cde65-220">49%</span></span> |
|<span data-ttu-id="cde65-221">Samantha</span><span class="sxs-lookup"><span data-stu-id="cde65-221">Samantha</span></span> | <span data-ttu-id="cde65-222">Занята</span><span class="sxs-lookup"><span data-stu-id="cde65-222">Busy</span></span> | <span data-ttu-id="cde65-223">0 %</span><span class="sxs-lookup"><span data-stu-id="cde65-223">0%</span></span> |

<span data-ttu-id="cde65-224">В этом случае достоверность предлагаемого времени проведения собрания (средняя вероятность посещения) составляет (100 % + 49 % + 0 %)/3 = 49,66 %.</span><span class="sxs-lookup"><span data-stu-id="cde65-224">Then the confidence of the meeting time suggestion, which is the average chance of attendance, is (100% + 49% + 0%)/3 = 49.66%.</span></span>

<span data-ttu-id="cde65-225">Если в методе **findMeetingTimes** указать для параметра **minimumAttendeePercentage** значение 80 %, операция не будет предлагать это время в ответе, так как 49,66 % < 80 %.</span><span class="sxs-lookup"><span data-stu-id="cde65-225">If you specify a **minimumAttendeePercentage** of 80% in a **findMeetingTimes** operation, because 49.66% < 80%, the operation will not suggest this time in the response.</span></span>

## <a name="example"></a><span data-ttu-id="cde65-226">Пример</span><span class="sxs-lookup"><span data-stu-id="cde65-226">Example</span></span>

<span data-ttu-id="cde65-227">В приведенном ниже примере показано, как найти время для встречи в заранее установленном месте и запросить причину для каждого предложения, указав следующие параметры в тексте запроса:</span><span class="sxs-lookup"><span data-stu-id="cde65-227">The following example shows how to find time to meet at a pre-determined location, and request a reason for each suggestion, by specifying the following parameters in the request body:</span></span>

- <span data-ttu-id="cde65-228">**attendees**</span><span class="sxs-lookup"><span data-stu-id="cde65-228">**attendees**</span></span>
- <span data-ttu-id="cde65-229">**locationConstraint**</span><span class="sxs-lookup"><span data-stu-id="cde65-229">**locationConstraint**</span></span>
- <span data-ttu-id="cde65-230">**timeConstraint**</span><span class="sxs-lookup"><span data-stu-id="cde65-230">**timeConstraint**</span></span>
- <span data-ttu-id="cde65-231">**isOrganizerOptional**</span><span class="sxs-lookup"><span data-stu-id="cde65-231">**isOrganizerOptional**</span></span>
- <span data-ttu-id="cde65-232">**meetingDuration**</span><span class="sxs-lookup"><span data-stu-id="cde65-232">**meetingDuration**</span></span>
- <span data-ttu-id="cde65-233">**returnSuggestionReasons**</span><span class="sxs-lookup"><span data-stu-id="cde65-233">**returnSuggestionReasons**</span></span>
- <span data-ttu-id="cde65-234">**minimumAttendeePercentage**</span><span class="sxs-lookup"><span data-stu-id="cde65-234">**minimumAttendeePercentage**</span></span>

<span data-ttu-id="cde65-235">Указав параметр **returnSuggestionReasons**, вы также получите в свойстве **suggestionReason** объяснение для каждого предложения, если метод **findMeetingTimes** возвращает какие-либо предложения.</span><span class="sxs-lookup"><span data-stu-id="cde65-235">By setting the **returnSuggestionReasons** parameter, you also get an explanation in the **suggestionReason** property for each suggestion, if **findMeetingTimes** returns any suggestion.</span></span>

<span data-ttu-id="cde65-236">Обратите внимание, что в запросе задается время в часовом поясе PST.</span><span class="sxs-lookup"><span data-stu-id="cde65-236">Notice that the request specifies time in the PST time zone.</span></span> <span data-ttu-id="cde65-237">По умолчанию в ответе возвращаются предложения времени собраний в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="cde65-237">By default, the response returns meeting time suggestions in UTC.</span></span> <span data-ttu-id="cde65-238">Вы можете использовать заголовок `Prefer: outlook.timezone` запроса, чтобы указать PST-файл, а также значения времени в отклике.</span><span class="sxs-lookup"><span data-stu-id="cde65-238">You can use the `Prefer: outlook.timezone` request header to specify PST as well for the time values in the response.</span></span>

##### <a name="request"></a><span data-ttu-id="cde65-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="cde65-239">Request</span></span>
<span data-ttu-id="cde65-240">Ниже представлен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cde65-240">Here is the example request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="cde65-241">Ответ</span><span class="sxs-lookup"><span data-stu-id="cde65-241">Response</span></span>
<span data-ttu-id="cde65-p123">Ниже представлен пример ответа. Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cde65-p123">Here is an example response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.findMeetingTimesResponse",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.findMeetingTimesResponse",
    "emptySuggestionsReason": "",
    "meetingTimeSuggestions": [
        {
            "confidence": 100,
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
                    "dateTime": "2019-04-18T12:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T13:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
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
    "Error: /api-reference/beta/api/user-findmeetingtimes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

# <a name="user-findmeetingtimes"></a>user: findMeetingTimes
Предложение времени проведения собрания с учетом доступности организатора и участников, а также ограничений по местоположению или времени, указанных в качестве параметров.

Если метод **findMeetingTimes** не может вернуть предложение, то в свойстве **emptySuggestionsReason** будет указана причина. Это значение поможет вам лучше настраивать параметры и снова вызывать метод **findMeetingTimes**.

**Примечание**

В настоящее время метод **findMeetingTimes** предполагает следующее:

- Любой объект [attendee](../resources/attendee.md), являющийся пользователем (а не ресурсом), — это обязательный участник. Таким образом, укажите значение `required` для пользователя и `resource` для ресурса в соответствующем свойстве **type** в составе параметра коллекции **attendees**.
- Предлагаемое время приходится только на рабочие часы организатора или участника. Вы можете не указывать свойство **activityDomain** объекта [timeConstraint](../resources/timeConstraint.md). 


## <a name="prerequisites"></a>Необходимые компоненты
Для выполнения этого API требуется одна из следующих **областей**: *Calendars.Read.Shared* или *Calendars.ReadWrite.Shared*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Значение|
|:---------------|:----------|
| Авторизация  | <code> носителя|
| Prefer: outlook.timezone | Строка, представляющая определенный часовой пояс для ответа, например "Тихоокеанское время США (зима)". |


## <a name="request-body"></a>Тело запроса
Ниже перечислены все поддерживаемые параметры. В зависимости от сценария, укажите объект JSON для каждого из обязательных параметров в тексте запроса. В зависимости от указанных параметров, действие **findMeetingTimes** проверяет сведения о доступности в основных календарях организатора и участников. Действие вычисляет наиболее подходящее время собрания и возвращает предложения.


| Параметр       | Тип    |Описание|
|:---------------|:--------|:----------|
|attendees|Коллекция объектов [attendeeBase](../resources/attendeebase.md)|Коллекция участников или ресурсов для собрания. Если указана пустая коллекция, действие **findMeetingTimes** ищет свободные периоды времени для организатора.|
|locationConstraint|[locationConstraint](../resources/locationconstraint.md)|Требования организатора к месту проведения собрания (например, требуется ли предложение или собрание может пройти только в определенных местах).|
|timeConstraint|[timeConstraint](../resources/timeconstraint.md)|Время начала и окончания собрания. Вы можете указать часовой пояс в свойствах **start** и **end** для этого параметра. Однако этот часовой пояс влияет только на параметр **timeConstraint**. В ответе значения времени по умолчанию указываются в формате UTC. С помощью заголовка запроса `Prefer: outlook.timezone` вы можете указать определенный часовой пояс для значений времени в ответе. |
|meetingDuration|Edm.Duration|Продолжительность собрания в формате [ISO8601](http://www.iso.org/iso/iso8601). Например, 1 час обозначается как PT1H, где P обозначает продолжительность, T — время, а H — часы. Если продолжительность собрания не указана, метод **findMeetingTimes** использует значение по умолчанию — 30 минут. |
|maxCandidates|Edm.Int32|Максимальное количество возвращаемых предложений времени проведения собрания.|
|isOrganizerOptional|Edm.Boolean|Значение `True`, если присутствие организатора необязательно; в противном случае — значение `false`.|
|returnSuggestionReasons|Edm.Boolean|Значение `True`, если требуется вернуть причину каждого предложения в свойстве **suggestionReason**. По умолчанию задано значение `false`, и это свойство не возвращается.|
|minimumAttendeePercentage|Edm.Double| Минимальная [достоверность](#the-confidence-of-a-meeting-suggestion), необходимая, чтобы вернуть период времени в ответе. Это процентное значение от 0 до 100. |

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа `200, OK` и объект [meetingTimeSuggestionsResult](../resources/meetingTimeSuggestionsResult.md) в тексте ответа. 

Объект **meetingTimeSuggestionsResult** включает коллекцию предложений и свойство **emptySuggestionsReason**. Каждое предложение определяется как объект [meetingTimeSuggestion](../resources/meetingTimeSuggestion.md), где средняя вероятность присутствия участников составляет 50 % или определенное процентное значение, указанное в параметре **minimumAttendeePercentage**. 

По умолчанию каждое предлагаемое время проведения собрания указывается в формате UTC. 

### <a name="the-confidence-of-a-meeting-suggestion"></a>Достоверность предложения

Свойство **confidence** объекта **meetingTimeSuggestion** принимает значения от 0 % до 100 % и представляет вероятность того, что все участники посетят собрание. Она зависит от сведений о доступности каждого участника:

- Если тот или иной участник доступен в указанный период времени, для него задается вероятность посещения 100 %, если его состояние неизвестно — 49 %, а если он занят— 0 %.
- Достоверность предлагаемого времени собрания вычисляется как средняя вероятность присутствия всех указанных участников собрания.
- При наличии нескольких предложений времени действие **findMeetingTimes** сначала сортирует их по убыванию значения достоверности. При наличии нескольких предложений с одинаковой достоверностью это действие сортирует их в хронологическом порядке.
- С помощью необязательного параметра **minimumAttendeePercentage** метода **findMeetingTimes** вы можете сделать так, чтобы возвращались предложения со значением достоверности не ниже указанного. Например, вы можете задать для параметра **minimumAttendeePercentage** значение 80 %, если вас интересуют только те предложения, для которых вероятность присутствия всех участников составляет не менее 80 %. Если параметр **minimumAttendeePercentage** не указан, метод **findMeetingTimes** предполагает значение 50 %.

Допустим, время проведения собрания предложено с учетом 3 участников со следующими сведениями о доступности:

|**Участник**|**Сведения о доступности**|**Процентная вероятность посещения**|
|:-----|:-----|:-----|
|Дарья | Свободна | 100 % |
|Иван | Неизвестно | 49 % |
|Лилия | Занята | 0 % |

В этом случае достоверность предлагаемого времени проведения собрания (средняя вероятность посещения) составляет (100 % + 49 % + 0 %)/3 = 49,66 %.

Если в методе **findMeetingTimes** указать для параметра **minimumAttendeePercentage** значение 80 %, операция не будет предлагать это время в ответе, так как 49,66 % < 80 %.

## <a name="example"></a>Пример

В приведенном ниже примере показано, как найти время для встречи в заранее установленном месте и запросить причину для каждого предложения, указав следующие параметры в тексте запроса:

- **attendees**
- **locationConstraint**
- **timeConstraint**
- **meetingDuration**
- **returnSuggestionReasons**
- **minimumAttendeePercentage**

Указав параметр **returnSuggestionReasons**, вы также получите в свойстве **suggestionReason** объяснение для каждого предложения, если метод **findMeetingTimes** возвращает какие-либо предложения.

Обратите внимание, что в этом запросе указывается Тихоокеанское время, а в ответе по умолчанию возвращаются предложения времени в формате UTC. С помощью заголовка запроса `Prefer: outlook.timezone` вы можете сделать так, чтобы в ответе тоже возвращалось Тихоокеанское время.

##### <a name="request"></a>Запрос
Ниже представлен пример запроса.
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Content-type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Fanny Downs",
        "address": "fannyd@a830edad905084922E16072013.onmicrosoft.com" 
      } 
    },
    { 
      "type": "optional",  
      "emailAddress": { 
        "name": "Dana Swope",
        "address": "danas@a830edad905084922E16072013.onmicrosoft.com" 
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
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2016-10-20T07:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2016-10-20T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": "true",
  "minimumAttendeePercentage": "60"
}
```

##### <a name="response"></a>Отклик
Ниже представлен пример ответа. Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json


{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
   "meetingTimeSuggestions":[
      {
         "meetingTimeSlot":{
            "start":{
               "dateTime":"2016-10-20T15:00:00.0000000",
               "timeZone":"UTC"
            },
            "end":{
               "dateTime":"2016-10-20T17:00:00.0000000",
               "timeZone":"UTC"
            }
         },
         "confidence":100,
         "organizerAvailability":"free",
         "attendeeAvailability":[
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Fanny Downs",
                    "address": "fannyd@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"free"
            },
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Dana Swope",
                    "address": "danas@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"free"
            }
         ],
         "locations":[
            {
               "displayName":"Conf room Hood"
            }
         ],
         "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available."
      },
      {
         "meetingTimeSlot":{
            "start":{
               "dateTime":"2016-10-20T17:00:00.0000000",
               "timeZone":"UTC"
            },
            "end":{
               "dateTime":"2016-10-20T19:00:00.0000000",
               "timeZone":"UTC"
            }
         },
         "confidence":100,
         "organizerAvailability":"free",
         "attendeeAvailability":[
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Fanny Downs",
                    "address": "fannyd@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"free"
            },
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Dana Swope",
                    "address": "danas@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"unknown"
            }
         ],
         "locations":[
            {
               "displayName":"Conf room Hood"
            }
         ],
         "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available."
      }
   ],
   "emptySuggestionsReason":""
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
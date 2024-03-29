---
title: Выбор API в Microsoft Graph для создания онлайн-встреч и подключения к ним
description: Подумайте, когда следует использовать ресурс событий API календаря или ресурс облачных коммуникаций onlineMeeting для Teams и собраний Skype в календаре Outlook.
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 8af02249b97eea35269cbcbf565cd75b74368d7f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436402"
---
# <a name="choose-an-api-in-microsoft-graph-to-create-and-join-online-meetings"></a>Выбор API в Microsoft Graph для создания онлайн-встреч и подключения к ним

В Microsoft Graph предлагаются два набора API, которые позволяют упорядочить онлайн-встречи в Microsoft Teams или Skype или присоединиться к ним:

- [API календаря](outlook-calendar-online-meetings.md): используйте [ресурс](/graph/api/resources/event) события.
- [API облачных коммуникаций](cloud-communications-online-meetings.md): используйте ресурс [onlineMeeting](/graph/api/resources/onlineMeeting).

Вы выбираете между:
- Удобным запрограммированным средством для создания онлайн-встреч в календаре Outlook, где участники могут присоединяться к собранию и продолжать работу в Teams или в Skype.
- Более обширная программная интеграция функций Teams или Skype в приложении для более индивидуального взаимодействия.

## <a name="considerations-when-choosing-an-api-for-your-scenario"></a>Рекомендации по выбору API для вашего сценария

Выберите API календаря для оптимизированной встроенной интеграции с календарем Outlook, что позволит настроить собрание в календаре Outlook: 
- Программная поддержка:
  - Приложения могут _непосредственно создавать и обновлять события в виде онлайн-встречи в календаре Outlook_ с помощью большого двоичного объекта join-Teams-meeting, добавляемого в событие календаря Outlook.
  - Приложения получают свойства для присоединения к собраниям через Интернет или по телефону.
- Пользовательский интерфейс участников с программно созданным событием календаря полностью соответствует интерфейсу события, созданного в пользовательском интерфейсе Outlook:
  - Участники сами выбирают, как встречаться: по сети или лично.
  - Участники могут щелкнуть объект join-Teams-meeting, чтобы присоединяться к собранию через Интернет или по телефону.
  - Участники могут использовать другие широкие возможности Teams, в том числе видеоконференции и "зал собрания", если они настроены.

> [!NOTE]
> Интеграция с календарем Outlook предполагает, что администратор настроил Outlook для собраний по сети. Перед тем как использовать API, [проверяйте](/microsoftteams/exchange-teams-interact) службу поддержки.

Выберите API облачных коммуникаций для получения более гибкой и программной поддержки:
- В приложениях больше возможностей, позволяющих интегрировать результаты API в соответствии с родом занятий и другими приложениями. API не привязан к конкретному календарю и не создает событие ни в одном календаре.
- Ниже описаны возможности, которые приложения могут предоставить участникам.
  - Предоставление объединенной информации на основе языковой среды.
  - Присоединение к собраниям через Интернет или по телефону.
  - Видеоконференции.
  - Дополнительные функции безопасности, такие как "зал собрания" и автоматизация допуска участников (предварительный просмотр).
  - Привязка собрания к чату в Microsoft Teams.

## <a name="comparing-the-apis"></a>Сравнение API

В таблице ниже описаны различия на уровне API. 


| Возможность онлайн-встреч | API календаря (ресурс события) | API облачных коммуникаций (ресурс onlineMeeting)             |
|:-----------------------|:------------------------------|:-------------------------------------------------------------|
| Основные участники API | Ресурс [события](/graph/api/resources/event): <br>Свойство - **isOnlineMeeting** <br>Свойство - **onlineMeeting** типа [onlineMeetingInfo](/graph/api/resources/onlinemeetinginfo) <br>Свойство - **onlineMeetingProvider** <br> Ресурс [календаря](/graph/api/resources/calendar): <br>Свойство - **allowedOnlineMeetingProviders** <br>Свойство - **defaultOnlineMeetingProvider** <br> | Ресурс [onlineMeeting](/graph/api/resources/onlinemeeting) <br> Ресурс [audioConferencing](/graph/api/resources/audioconferencing)
| Интеграция с элементом календаря | <br>- [Создание](/graph/api/user-post-events) или [обновление](/graph/api/event-update) API **события** автоматически задает конечное [событие](/graph/api/resources/event) календаря Outlook в качестве онлайн-встречи.<br>- Использование свойства **isOnlineMeeting**, **onlineMeeting** и **onlineMeetingProvider** возвращенного **события** календаря Outlook.  | - [Создание](/graph/api/application-post-onlinemeetings) API возвращает ресурс [onlineMeeting](/graph/api/resources/onlinemeeting), который не зависит от конкретного типа календаря. <br>- Не создает и не обновляет события Outlook. <br>- Интеграция возвращенной информации ресурса **onlineMeeting** в приложении, которое подходит для вашего сценария. <br>- Использование [createOrGet](/graph/api/onlinemeeting-createorget) для возврата онлайн-встречи с указанным значением **externalId** или его создание в случае отсутствия, чтобы упростить внедрение получившегося собрания в стороннем календаре. |
| Переход к автономному собранию | - Нет. Если вы подключите возможность подключения к **встрече** по сети, вы не сможете изменить его, чтобы сделать собрание автономным.<br>- Невозможно изменить свойство **onlineMeetingProvider** или задать значение **isOnlineMeeting**, `false`чтобы отключить собрание по сети.  | Нет. Если вы создаете ресурс **onlineMeeting**, вы можете удалить его, но не можете сделать так, чтобы оно стало автономным. |
| Предоставление объединенной информации на основе языковой среды | Интеграция прямого API не осуществляется. | - Использование `Accept-Language`заголовка HTTP при создании онлайн-встречи. <br>- См. [пример](/graph/api/application-post-onlinemeetings#example-2-create-an-online-meeting-with-user-token). |
| Соединение по сети (VoIP) | Через свойство **onlineMeeting** получите доступ к **joinUrl**.  | Используйте свойство **joinWebUrl**. |
| Соединение по телефону | Через свойство **onlineMeeting** получите доступ к: <br>- **conferenceId**, **quickDial**, **phones**, **tollFreeNumbers**, **tollNumber**. |Через свойство **audioConferencing** получите доступ к: <br> - **conferenceId**, **tollFreeNumber**, **tollNumber**.<br> Свойство - **dialinUrl** для веб-страницы, доступной извне, с информацией о том, как подключиться по телефону для интеграции со сторонними приложениями. |
| Присоединение по видеоконференции (аудио и видео) | Интеграция прямого API не осуществляется. | Используйте свойство **videoTeleconferenceId**. |
| "Зал собраний" и автоматический доступ участников к онлайн-встречам | - Интеграция прямого API не осуществляется.<br>- Во вставленном в событие объекте join-Teams-meeting участники могут выбрать **Параметры собрания**, чтобы получить доступ к "залу собраний", если такая функция включена администратором. |- API, позволяющий отличать участников организации и федеративные компании, а также других участников, включая анонимных.  <br>- Использование свойства **autoAdmittedUsers** (предварительный просмотр).  |
| Относится к чату в Teams | Интеграция прямого API не осуществляется. | Используйте свойство **chatInfo**. |
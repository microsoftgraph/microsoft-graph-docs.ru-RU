---
title: Службы и компоненты Microsoft Graph
description: Узнайте, как сеть служб и компонентов Microsoft 365 в Microsoft Graph обеспечивает управление, защиту и извлечения данных с поддержкой широкого набора сценариев.
author: angelgolfer-ms
ms.localizationpriority: high
ms.custom: scenarios:getting-started
ms.openlocfilehash: 3b9a6813acd90b39ed19df45f6807e1f79195ee5
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883093"
---
# <a name="major-services-and-features-in-microsoft-graph"></a>Основные службы и компоненты в Microsoft Graph

Microsoft Graph позволяет интегрировать приложение с лучшими службами Microsoft 365, Windows и Enterprise Mobility + Security в Microsoft 365, используя REST API и клиентские библиотеки. Кроме того, в нем имеются функции аналитики системы безопасности, с помощью которых можно повысить эффективность работы пользователей, стимулировать творчество и совместную работу в группах, а также защищать бизнес-ресурсы и данные пользователей.

## <a name="users-and-groups"></a>Пользователи и группы

В основе Microsoft Graph лежит концепция пользователя и группы. 

_Пользователь_ в Microsoft Graph — это один из миллионов людей, которые используют облачные службы Microsoft 365. Это центральная точка, чье удостоверение защищено и доступ к которой хорошо управляется. Данные пользователя — это то, на чем основан бизнес. Службы Microsoft Graph делают эти данные доступными для организаций в функциональных контекстах, обновлениях в режиме реального времени и результатах глубокой аналитики. Доступ к данным всегда предоставляется только при наличии соответствующих разрешений.

_Группа_ Microsoft 365 — это фундаментальный объект, с помощью которого пользователи могут вести совместную работу. Она интегрируется с другими службами, что позволяет использовать более функциональные сценарии при планировании задач, работе в группах, обучении и т. д. 

|Компонент     |Вспомогательные службы  |Описание |Дополнительные сведения |
|:-----------|:--------------------|:-----------|:----------------|
| Пользователи | Azure AD и большая часть служб для повышения производительности труда, совместной работы, аналитики и обучения | Пользователь — это основной объект в Microsoft Graph, для которого во многих службах Microsoft Graph создаются функции, ориентированные на пользователей. | [Обзор пользователей в Microsoft Graph](azuread-users-concept-overview.md)|
|Группы | Azure AD, OneDrive, OneNote, Outlook, Планировщик | Группа Microsoft 365 — это основа для совместной работы. В группах пользователи могут обмениваться беседами, файлами, заметками, календарями планами и т. д. | [Обзор групп Microsoft 365 в Microsoft Graph](office365-groups-concept-overview.md) |

## <a name="connecting-users-data-microsoft-365-services-and-your-apps"></a>Соединение данных пользователей, служб Microsoft 365 и ваших приложений

Используя пользователей и группы в качестве основы, Microsoft Graph создает сеть служб и компонентов Microsoft 365, которые управляют данными, защищают и извлекают их для поддержки широкого спектра сценариев. С помощью Microsoft Graph вы можете получить доступ к огромному количеству данных пользователей, выполнив при этом необходимую авторизацию.

![Microsoft Graph соединяет вас с данными пользователей](images/microsoft-graph-connects-users-data.png)

### <a name="services-and-features"></a>Службы и компоненты

Некоторые службы в Microsoft Graph представлены впервые, другие хорошо известны в качестве автономных служб и сейчас включены в состав Microsoft Graph. Наборы API этих служб имеют оптимизированную конструкцию, описанную в статье [Рекомендации по REST API Майкрософт](https://github.com/Microsoft/api-guidelines), и теперь можно получить доступ к ним через единую конечную точку REST для Microsoft Graph `https://graph.microsoft.com`. В оставшейся части этой статьи перечислены основные службы и компоненты с разбивкой по категориям. 

## <a name="identity-and-access-management"></a>Управление идентификацией и доступом

|Компонент     |Вспомогательные службы  |Описание |Дополнительные сведения |
|:-----------|:--------------------|:-----------|:----------------|
| Управление идентификацией и доступом | Azure AD | Создает ресурсы каталогов, например пользователей, группы и приложения, и управляет ими. Управляет доступом к ресурсам и данным. Предоставляет пользователям доступ к данным о рисках, связанным со входом в систему и учетными записями, в Azure AD.| [Обзор управления идентификацией и доступом в Azure AD](azuread-identity-access-management-concept-overview.md)  |

## <a name="productivity"></a>Эффективность

|Компонент     |Вспомогательные службы  |Описание |Дополнительные сведения |
|:-----------|:--------------------|:-----------|:----------------|
| Календарь | Outlook  | Дает пользователям возможность создавать встречи и собрания в Интернете, на мобильных и настольных устройствах. Является частью центра обмена сообщениями Outlook в Microsoft 365, с помощью которого пользователи также могут управлять своими письмами и контактами. | [Обзор календарей Outlook](outlook-calendar-concept-overview.md)  |
| Файлы | OneDrive и SharePoint | Управление и предоставление доступа к файлам пользователей в OneDrive и SharePoint. | [Обзор хранилища файлов OneDrive](onedrive-concept-overview.md) |
| Почта | Outlook | Дает пользователям возможность общаться, упорядочивать сообщения и управлять приоритетами в их рабочих процессах в Интернете, на мобильных и настольных устройствах. Является частью центра связи Outlook в Microsoft 365, с помощью которого пользователи также могут управлять своими контактами и планировать собрания. | [Обзор почты Outlook](outlook-mail-concept-overview.md) |
| Заметки | OneNote | Дает пользователям возможность планировать и упорядочивать идеи и информацию. | [Обзор заметок OneNote](integrate-with-onenote.md) |
| Личные контакты | Outlook | Диспетчер контактов в Интернете, на мобильных и настольных устройствах. Является частью центра обмена сообщениями Outlook в Microsoft 365, с помощью которого пользователи также могут управлять своими письмами и планировать собрания.  | [Обзор личных контактов в Outlook](outlook-contacts-concept-overview.md) |
| Книги и диаграммы | Excel | Дает пользователям возможность выполнять сложные вычисления, отслеживать, анализировать и визуализировать данные с помощью электронных таблиц Excel, а также создавать профессиональные отчеты. | [Обзор книг и диаграмм Excel](excel-concept-overview.md) |
| Задачи To-Do | To-Do | Помогает пользователям управлять личными задачами на работе и вне ее. Интегрируется с Outlook, Teams, Планировщиком и Кортаной, являясь, таким образом, единым центром для личных задач пользователя в Microsoft 365. | [Обзор задач To Do](todo-concept-overview.md) |

## <a name="collaboration-and-employee-learning"></a>Совместная работа и обучение сотрудников

<!-- Want to update links to concept overviews as they are created over time. 
-->
|Функция     |Вспомогательные службы  |Описание |Дополнительные сведения |
|:-----------|:--------------------|:-----------|:----------------|
| Облачные коммуникации | Microsoft Teams, Skype | Позволяет приложениям и службам взаимодействовать с пользователями с помощью различных функций для работы с сообщениями, например, использование ботов для обработки вызовов, интеграция собраний по сети в бизнес-сценарии, отображение статуса присутствия пользователей (предварительная версия), а также поиск записей звонков и собраний по сети (предварительная версия). | [Обзор облачных коммуникаций](cloud-communications-concept-overview.md) |
| Сайты и списки  | SharePoint | Веб-платформа для пользователей и групп Microsoft 365, на которой можно делиться контентом (в том числе списками, файлами и заметками), упорядочивать и искать его, а также управлять им. | [Обзор сайтов и контента SharePoint](sharepoint-concept-overview.md) | 
|Задачи и планы | Планировщик | Дает пользователям в группах Microsoft 365 возможность создавать планы, назначать задачи и отслеживать ход их выполнения. | [Обзор планов и задач в Планировщике](planner-concept-overview.md) |
|Командная работа |  Microsoft Teams | Цифровой центр и рабочее пространство на основе чатов, в котором участники групп могут обмениваться файлами, заметками, календарями и планами. | [Общие сведения работе в группах в Microsoft Teams](teams-concept-overview.md) |
| Обучение сотрудников | Viva Обучение | Позволяет сотрудникам сделать обучение естественной частью дня, добавляя обучение в поток работы в средствах и платформах Microsoft 365, которые они уже используют. Обнаруживайте и отслеживайте обучение, а также совместно используйте его в различных источниках из центра обучения в Microsoft Teams.  | [Включение обучения сотрудников с помощью возможностей совместной работы в Teams](teams-concept-overview.md#enable-employee-learning-using-the-collaborative-capabilities-in-teams) |

## <a name="people-and-workplace-intelligence"></a>Люди и рабочая аналитика

|Функция     |Вспомогательные службы  |Описание |Дополнительные сведения |
|:-----------|:--------------------|:-----------|:----------------|
| Люди | Azure AD, Outlook, SharePoint и т. д. | Получение информации о людях в порядке их релевантности для пользователя на основе шаблонов общения и совместной работы пользователей, а также их бизнес-связей.  | [Обзор данных о людях и рабочей аналитики в Microsoft Graph](social-intel-concept-overview.md) |
| Профиль (предварительная версия) | Профиль | Представляет собой упрощенный механизм хранения и получения сведений о людях в клиенте. | [Обзор данных о людях и рабочей аналитики в Microsoft Graph](social-intel-concept-overview.md) |
| Настройка карточки профиля (предварительная версия) | Карточка профиля | Предоставляет администратору возможность настроить контент, находящийся на карточке профиля Microsoft 365 в организации. | [Обзор данных о людях и рабочей аналитики в Microsoft Graph](social-intel-concept-overview.md) |
| Аналитика на основе документов  | Delve, OneDrive, Outlook, SharePoint | Использование расширенной аналитики и методов машинного обучения для получения документов, популярных в среде пользователя, просмотренных или измененных пользователем, а также документов, к которым пользователь предоставил общий доступ.  | [Обзор данных о людях и рабочей аналитики в Microsoft Graph](social-intel-concept-overview.md)  |
| Аналитика (предварительная версия) | Viva Аналитика | Использование расширенной аналитики и методов машинного обучения для получения сведений о том, как и с кем пользователи тратят свое время. Эти данные помогают пользователям спланировать свой день, получить аналитику о различных рабочих закономерностях и обеспечить баланс работы и личной жизни.  | [Обзор данных о людях и рабочей аналитики в Microsoft Graph](social-intel-concept-overview.md) |

## <a name="device-and-app-management"></a>Управление устройствами и приложениями

|Функция     |Вспомогательные службы  |Описание |Дополнительные сведения |
|:-----------|:--------------------|:-----------|:----------------|
| Облачная печать | Универсальная печать | Универсальная печать — это облачная инфраструктура печати Microsoft 365, которая обеспечивает простую и безопасную печать для пользователей и снижает трудозатраты ИТ-персонала на администрирование и управление. | [Обзор API облачной среды универсальной печати](universal-print-concept-overview.md) |
|Управление устройствами и приложениями организации | Intune | Регистрация и настройка устройств, а также управление мобильными приложениями в организации. | [Обзор устройств и приложений в Intune](intune-concept-overview.md) |
| Облачный компьютер (предварительная версия) | Windows 365  | Windows 365 — это облачная служба, которая позволяет администраторам легко настраивать облачные ПК с ОС Windows 365 для пользователей в своей организации управлять ими. Отдельные конечные пользователи могут безопасно передавать свои персонализированные приложения Windows из облака Microsoft на любое устройство в любое время с помощью своего облачного ПК. | [Работа с облачными ПК с ОС Windows 365 с использованием программного интерфейса Microsoft Graph](cloudpc-concept-overview.md) |
| Обновления устройств (предварительная версия) | Служба развертывания Windows Update для бизнеса | Обеспечивает контроль над утверждением, планированием, мониторингом и безопасностью содержимого, доставленного из Центра обновления Windows. | [Обновления Windows в Microsoft Graph](windowsupdates-concept-overview.md) |
| Управление несколькими клиентами (предварительная версия) | Microsoft 365 Lighthouse | Позволяет поставщикам управляемых служб удаленно управлять несколькими пользовательскими клиентами для обеспечения соответствия требованиям и обнаружения угроз, а также обеспечивать работоспособное и безопасное состояние устройств клиента. | [Управление несколькими клиентами с помощью Microsoft 365 Lighthouse](managedtenants-concept-overview.md) |
| Работоспособность и взаимодействие служб | Службы Microsoft 365 и Dynamics 365 | Предоставляет доступ к данным о работоспособности и публикациям центра сообщений об облачных службах Майкрософт. Наглядным примером использования API взаимодействия служб является Центр администрирования Microsoft 365. | [Доступ к сведениям о работоспособности и взаимодействии служб в Microsoft Graph](service-communications-concept-overview.md) |

## <a name="security"></a>Безопасность

|Компонент     |Вспомогательные службы  |Описание |Дополнительная информация |
|:-----------|:--------------------|:-----------|:----------------|
| Интеграция с системой безопасности | Защита идентификации Azure AD, Azure Information Protection, Центр безопасности Azure, Microsoft Defender for Cloud Apps, Advanced Threat Protection в Защитнике Windows и [другие](/graph/api/resources/security-api-overview) | Предоставляет единый шлюз для аналитики безопасности и действий в корпорации Майкрософт и компаниях-партнерах по экосистеме. | [Безопасность в Microsoft Graph](security-concept-overview.md) |
| Обнаружение электронных данных (eDiscovery) | eDiscovery (премиум) Microsoft Purview | Обеспечивает доступ к возможностям обнаружения электронных данных, применяемых в процессе определения и предоставления электронной информации, которая может использоваться в качестве доказательств в судебных разбирательствах.|[Безопасность в Microsoft Graph](security-concept-overview.md)|

## <a name="cross-device-experiences"></a>Интерфейсы на различных устройствах

|Компонент     |Вспомогательные службы  |Описание |Дополнительные сведения |
|:-----------|:--------------------|:-----------|:----------------|
| Интерфейсы на различных устройствах | Веб-канал активности, ретрансляции устройства | Дает возможность использовать интерфейсы приложений, выходящие за рамки одного устройства. С помощью этой функции пользователи могут переходить с одного устройства на другое независимо от типов и платформ устройств. | [Обзор использования единого интерфейса на нескольких устройствах](cross-device-concept-overview.md) |

## <a name="user-notifications-deprecated"></a>Уведомления пользователей (не рекомендуется)

> [!IMPORTANT]
> API уведомлений Microsoft Graph не рекомендуется использовать, Он прекратил возвращать данные в январе 2022 г. Дополнительные сведения об уведомлениях см. в [Центрах уведомлений Microsoft Azure](/azure/notification-hubs). Дополнительные сведения см. в [этой записи блога](https://devblogs.microsoft.com/microsoft365dev/retiring-microsoft-graph-notifications/).

|Функция     |Вспомогательные службы  |Описание |Дополнительная информация |
|:-----------|:--------------------|:-----------|:----------------|
| Уведомления пользователей | Уведомления пользователей | Позволяет использовать интерфейсы приложений для создания интерфейсов уведомлений, ориентированных на пользователя, а также кроссплатформенных интерфейсов уведомлений, включая развертывание для пользователей, универсальное закрытие и доступ к журналу уведомлений. | [Включение интерфейсов уведомлений, ориентированных на человека, с использованием уведомлений Microsoft Graph](notifications-concept-overview.md) |

## <a name="usage-reports"></a>Отчеты об использовании

|Компонент     |Вспомогательные службы  |Описание |Дополнительные сведения |
|:-----------|:--------------------|:-----------|:----------------|
| Отчеты | Microsoft Teams, OneDrive, Outlook, SharePoint, Skype для бизнеса, Yammer | Получение сведений об активности и использовании из службы, поддерживающей такие возможности. | [Обзор отчетов об использовании](reportroot-concept-overview.md) |

## <a name="education"></a>Образование

|Компонент     |Вспомогательные службы  |Описание |Дополнительные сведения |
|:-----------|:--------------------|:-----------|:----------------|
| Образование | Azure AD, образование | Предоставление сведений, релевантных для сценариев обучения, включая сведения об учебных заведениях, классах, учащихся и преподавателях. Дает независимым поставщикам программного обеспечения возможность создавать приложения для аудиторий, которые экономят преподавателям время и стимулируют работу в группах и совместную работу.  | [Обзор обучения](education-concept-overview.md) |

## <a name="business-applications"></a>Бизнес-приложения

|Компонент     |Вспомогательные службы  |Описание |Дополнительные сведения |
|:-----------|:--------------------|:-----------|:----------------|
| Резервирование для клиентов (ознакомительная версия) | Microsoft Bookings | Этот продукт предназначен для организаций, чтобы их пользователи и клиенты могли резервировать услуги непосредственно в Интернете, на веб-сайте или в Facebook. Позволяет организациям управлять настройками пользователей, службами и ценами, списками и расписаниями сотрудников, а также другой бизнес-информацией общего характера. | [Обзор API Microsoft Bookings](booking-concept-overview.md) |
| Финансовые показатели (предварительная версия) | Dynamics 365 Business Central | Позволяет управлять финансовыми данными, автоматизацией и защитой цепочки поставок, службой управления продаж и улучшенными возможностями обслуживания клиентов, службой управления проектов и оптимизацией процессов с помощью универсального решения для управления бизнесом.| [Обзор API Business Central](dynamics-business-central-concept-overview.md) |

## <a name="next-steps"></a>Дальнейшие действия

<!-- Need to update the destination page titles and URLs as Matt's v-team finalize on the examples and featured scenarios content 
-->

- См. раздел **Дополнительные сведения** в содержании. В этом разделе содержатся сведения о службах и компонентах, которые _вы_ можете использовать в своих сценариях.
- Опробуйте пример запроса в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- Воспользуйтесь [кратким руководством](https://developer.microsoft.com/graph/quick-start), чтобы настроить готовый к работе пример приложения.

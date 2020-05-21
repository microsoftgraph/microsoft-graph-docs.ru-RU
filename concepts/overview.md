---
title: Обзор Microsoft Graph
description: Microsoft Graph открывает доступ к данным и средствам искусственного интеллекта в Microsoft 365. Microsoft Graph предоставляет единую модель программирования, которую можно использовать для получения преимуществ огромного объема данных в Microsoft 365, Enterprise Mobility + Security и Windows 10.
author: angelgolfer-ms
localization_priority: Priority
ms.custom: scenarios:getting-started
ms.openlocfilehash: 92f165e4b05dd36f99d75e7c17dd6474659f8b83
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290453"
---
# <a name="overview-of-microsoft-graph"></a>Обзор Microsoft Graph

Microsoft Graph открывает доступ к данным и средствам искусственного интеллекта в Microsoft 365. Она предоставляет единую модель программирования, которую можно использовать для доступа к огромному объему данных в Microsoft 365, Windows 10 и Enterprise Mobility + Security. Используйте многочисленные данные в Microsoft Graph и создавайте приложения с миллионной аудиторией для организаций и пользователей.

## <a name="powering-the-microsoft-365-platform"></a>Расширение возможностей платформы Microsoft 365

![Благодаря Microsoft Graph, его соединителям и подключению к данным можно расширить возможности Microsoft 365 и создавать интеллектуальные приложения.](images/microsoft-graph-dataconnect-connectors-rebrand-800.png)

Три основных компонента платформы Microsoft 365 упрощают доступ к данным и их поток:

- API Microsoft Graph обеспечивает единую конечную точку, `https://graph.microsoft.com`, для доступа к ценным данным о пользователях и аналитическим сведениям, которые предоставляют ресурсы служб Microsoft 365. Вы можете использовать REST API или пакеты SDK для доступа к конечным точкам и сборкам приложений, поддерживающих сценарии, которые поддерживаются в ходе работы, совместной работы, образованиях, сведений о людях и рабочих местах и многое другое. Microsoft Graph также включает мощный набор служб, которые управляют идентификацией пользователей и устройств, доступом, соответствием требованиям, безопасностью и помогает защитить организации от утечки данных или потери данных.
- [Соединители Microsoft Graph (предварительная версия)](/microsoftsearch/connectors-overview) работают во входящем направлении, доставляя данные, не входящие в Microsoft Cloud, в службы и приложения Microsoft Graph, чтобы расширить возможности Microsoft 365, такие как Поиск (Майкрософт).
- [Подключение к данным Microsoft Graph](#access-microsoft-graph-data-at-scale-using-microsoft-graph-data-connect) предоставляет набор инструментов для оптимизации безопасности и масштабируемой доставки данных Microsoft Graph в популярные хранилища данных Azure. Эти кэшированные данные используются в качестве источников данных для средств разработки Azure, с помощью которых можно создавать интеллектуальные приложения.

Одновременное использование API Microsoft Graph, соединителей (предварительной версии) и подключения к данным позволяет расширить возможности платформы Microsoft 365. Благодаря доступу к данным Microsoft Graph и другим наборам данных для получения статистики и аналитики вы можете расширить возможности Microsoft 365 и создавать уникальные интеллектуальные приложения.

> [!NOTE]
> Соединители Microsoft Graph доступны в предварительной версии. Чтобы использовать соединители в Поиске (Майкрософт) или создавать соединители, требуется зарегистрироваться в [программе предварительной оценки соединителей](https://docs.microsoft.com/MicrosoftSearch/connectors-preview). Чтобы присоединиться к программе предварительной оценки, отправьте [форму регистрации в программе предварительной оценки соединителей Microsoft Graph](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRxWYgu82J_RFnMMATAS6_chUNVYwNU1CMDNZUDBSSDZKWVo2RDJDRjRLQi4u).

## <a name="whats-in-microsoft-graph"></a>Из чего состоит Microsoft Graph?

Microsoft Graph предоставляет API REST и клиентские библиотеки для доступа к данным в следующих облачных службах Майкрософт:

- Microsoft 365 Services: Delve, Excel, Microsoft Books, Microsoft Teams, OneDrive, OneNote, Outlook/Exchange, планировщик, SharePoint, аналитика рабочего места.
- Enterprise Mobility and Security Services: Advanced Threat Analytics, Advanced Threat Protection, Azure Active Directory, Диспетчер удостоверений и Intune.
- Службы Windows 10: действия, устройства, уведомления, Универсальная печать (Предварительная версия).
- Dynamics 365 Business Central.

Дополнительные сведения см. в статье [Основные службы и компоненты в Microsoft Graph](overview-major-services.md).

![Изображение основных ресурсов и отношений, из которых состоит Graph](images/microsoft-graph.png)

## <a name="what-can-you-do-with-microsoft-graph"></a>Что можно делать с помощью Microsoft Graph?

> [!VIDEO https://www.youtube-nocookie.com/embed/PI9NO5rayiY]

Microsoft Graph позволяет обрабатывать уникальный контекст пользователя и делать его более результативным. Представьте приложение, которое...

- Просматривает следующее собрание и помогает подготовиться к нему, предоставляя информацию об участниках, их должностях и руководителях, а также сведения о последних документах, с которыми работаете вы и ваши сотрудники.
- Проверяет ваш календарь и предлагает оптимальное время для следующего собрания команды.
- Получает диаграмму с перспективной оценкой продаж из файла Excel в OneDrive и позволяет обновлять прогноз в реальном времени с мобильного телефона.
- Подписывается на изменения вашего календаря, отправляет вам оповещение, если вы слишком много времени проводите на собраниях, и рекомендует, какие собрания можно пропустить или поручить кому-нибудь другому (в зависимости от того, насколько их участники важны для вас).
- Помогает вам упорядочивать личные и рабочие данные на телефоне. Например, приложение может группировать изображения, предназначенные для личного хранилища OneDrive, и накладные, которые следует хранить в OneDrive для бизнеса.
- Анализирует все данные Microsoft 365, чтобы лица, принимающие решения, могли разблокировать ценные сведения о распределении времени и шаблонах совместной работы, повышающих продуктивность бизнеса.
- Вносит пользовательские бизнес-данные в Microsoft Graph и индексирует их для поиска наряду с данными из служб Microsoft 365.

В качестве примера выберите первый сценарий поиска участников собрания. С помощью API Microsoft Graph вы можете:

1. Получить адреса электронной почты участников [собрания](/graph/api/resources/event?view=graph-rest-1.0).
2. Просмотреть информацию о каждом из них как о [пользователе](/graph/api/resources/user?view=graph-rest-1.0) в Azure Active Directory и [получить сведения о профиле](/graph/api/user-get?view=graph-rest-1.0).

С помощью связей вы можете перейти к другим ресурсам:

- Связаться с его руководителем через [связь с руководителем](/graph/api/user-list-manager?view=graph-rest-1.0).
- Получить полезные сведения, в том числе о популярных файлах, [которые отслеживает](/graph/api/resources/insights-trending?view=graph-rest-1.0) пользователь.
- [Узнать, какие люди больше всего связаны](/graph/api/user-list-people?view=graph-rest-beta) с пользователем.
- Расширить сценарий с помощью связи [memberOf](/graph/api/user-list-memberof?view=graph-rest-1.0), чтобы узнать, в какие группы входит пользователь
- [Найти других участников в каждой группе](/graph/api/group-list-members?view=graph-rest-1.0).
- Подключиться к другим сценариям, созданным [группами](office365-groups-concept-overview.md), например по [обучению](education-concept-overview.md) и [командной работе](teams-concept-overview.md).

Microsoft Graph продолжает открывать возможности платформы Microsoft 365 для разработчиков, но исключительно при наличии соответствующих разрешений.

> [!NOTE]
> Используя API Microsoft Graph, вы соглашаетесь с [условиями использования API Microsoft](/legal/microsoft-apis/terms-of-use?context=/graph/context) и [заявлением Майкрософт о конфиденциальности](https://go.microsoft.com/fwlink/?LinkId=521839).

### <a name="popular-api-requests"></a>Популярные запросы API

Ознакомьтесь с некоторыми из популярных сценариев работы с API Microsoft Graph. Ссылки ведут на [песочницу Graph](https://developer.microsoft.com/graph/graph-explorer).

| **Операция** | **URL-адрес** |
|:--------------------------|:----------------------------------------|
|   GET мой профиль | [`https://graph.microsoft.com/v1.0/me`](https://developer.microsoft.com/graph/graph-explorer/?request=me&version=v1.0) |
|   Получение своих файлов | [`https://graph.microsoft.com/v1.0/me/drive/root/children`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren&version=v1.0) |
|   Получение своей фотографии | [`https://graph.microsoft.com/v1.0/me/photo/$value`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fphoto%2F%24value&version=v1.0) |
|   Получение своей почты | [`https://graph.microsoft.com/v1.0/me/messages`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0) |
|   GET моя почта высокой важности | [`https://graph.microsoft.com/v1.0/me/messages?$filter=importance%20eq%20'high'`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages%3F%24filter%3Dimportance%2520eq%2520'high'&version=v1.0) |
|   GET события в моем календаре | [`https://graph.microsoft.com/v1.0/me/events`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fevents&version=v1.0) |
|   GET мой руководитель | [`https://graph.microsoft.com/v1.0/me/manager`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmanager&version=v1.0) |
|   GET последний пользователь, изменивший файл foo.txt | [`https://graph.microsoft.com/v1.0/me/drive/root/children/foo.txt/lastModifiedByUser`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren%2Ffoo.txt%2FlastModifiedByUser&version=v1.0) |
|   ПОЛУЧЕНИЕ групп Microsoft 365, участником которых я являюсь| [`https://graph.microsoft.com/v1.0/me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2FmemberOf%2F%24%2Fmicrosoft.graph.group%3F%24filter%3DgroupTypes%2Fany(a%3Aa%2520eq%2520'unified')&version=v1.0) |
|   GET пользователи в моей организации  | [`https://graph.microsoft.com/v1.0/users`](https://developer.microsoft.com/graph/graph-explorer/?request=users&version=v1.0) |
|   GET группы в моей организации | [`https://graph.microsoft.com/v1.0/groups`](https://developer.microsoft.com/graph/graph-explorer/?request=groups&version=v1.0) |
|   GET пользователи, связанные со мной | [`https://graph.microsoft.com/v1.0/me/people`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fpeople&version=beta)  |
|   GET элементы, популярные в моей компании | [`https://graph.microsoft.com/beta/me/insights/trending`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Finsights%2Ftrending&version=v1.0) |
|   GET мои заметки | [`https://graph.microsoft.com/v1.0/me/onenote/notebooks`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fonenote%2Fnotebooks&version=beta) |

## <a name="bring-data-from-an-external-content-source-to-microsoft-graph-preview"></a>Перенос данных из внешнего источника контента в Microsoft Graph (предварительная версия)

Используйте _соединители_ Microsoft Graph для переноса данных, не входящих в Microsoft Cloud, в Microsoft Graph. Примерами таких данных могут быть база данных отдела кадров организации или каталог продуктов, размещенные локально, в общедоступных или частных облаках. 

Соединители Microsoft Graph позволяют создавать подключения к внешним источникам данных, индексировать данные и хранить их как внешние настраиваемые элементы и файлы. После индексирования эти элементы могут отображаться в Поиске (Майкрософт), а также для приложений, использующих [API Поиска (Майкрософт)](search-concept-overview.md).

## <a name="access-microsoft-graph-data-at-scale-using-microsoft-graph-data-connect"></a>Масштабируемый доступ к данным Microsoft Graph с помощью подключения к данным Microsoft Graph

Используйте _подключение к данным_ Microsoft Graph для получения масштабируемого доступа к данным в Microsoft Graph, предоставляя администраторам точечные разрешения и полный доступ к этим данным. Подключение к данным помогает оптимизировать их доставку в Microsoft Azure.

С помощью средств Azure можно создавать интеллектуальные приложения с такими функциями:

- Поиск ближайшего специалиста по вопросу в вашей организации
- Автоматизация создания базы знаний
- Анализ приглашений на собрания для предоставления статистики об использовании конференц-залов
- Выявление мошенничества с данными производительности и взаимодействия

## <a name="when-should-i-use-microsoft-graph-api-or-data-connect"></a>Когда следует использовать API Microsoft Graph или подключение к данным?

Подключение к данным Microsoft Graph обеспечивает новый способ взаимодействия с данными, доступными через API Microsoft Graph. Подключение к данным предоставляет уникальный набор инструментов, которые помогают оптимизировать создание интеллектуальных приложений в рамках облака Майкрософт.

|**Функция**| **API Microsoft Graph** | **Подключение к данным Microsoft Graph** |
|:----------|:------------------------|:--------------------------------------|
| **Область доступа** | Один пользователь или весь клиент | Несколько пользователей или групп |
| **Шаблон доступа** | В режиме реального времени | Повторяющееся расписание |
| **Операции с данными** | Работает с оригиналом данных | Работает с кэшем данных |
| **Защита данных** | Данные защищены в пределах Microsoft 365 | Защита данных распространяется на кэш данных в подписке Azure |
| **Согласие пользователя** | Самостоятельное<br>Типы ресурсов | Нет |
| **Согласие администратора** | Вся организация<br>Типы ресурсов | Выбор групп пользователей<br>Типов и свойства ресурсов<br>Исключает пользователей |
| **Средства доступа** | Веб-запросы с применением REST | Фабрика данных Azure |

 См. статью [Подключение к данным Microsoft Graph](data-connect-overview.md), чтобы получить дополнительные сведения и [приступить к работе с подключением к данным](data-connect-concept-overview.md).

## <a name="next-steps"></a>Дальнейшие действия

- Ознакомьтесь с [представленными сценариями](https://developer.microsoft.com/graph/examples).
- Опробуйте пример запроса в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- Воспользуйтесь [кратким руководством](https://developer.microsoft.com/graph/quick-start), чтобы настроить готовый к работе пример приложения.
- Найдите в оглавлении, в разделе **Обучение**, службы и функции, которые вас интересуют, и почитайте о них.
- Узнайте, как [получить маркер аутентификации](auth/auth-concepts.md) в приложении.
- Начните [использовать API](use-the-api.md).

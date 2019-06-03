---
title: Обзор Microsoft Graph
description: Microsoft Graph открывает доступ к данным и средствам искусственного интеллекта в Microsoft 365. С помощью единой модели программируемости Microsoft Graph можно работать с колоссальным объемом данных в Office 365, Enterprise Mobility + Security и Windows 10.
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: c97f7d681774a6ba6ffa3969cec35f4104c1edbb
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656918"
---
# <a name="overview-of-microsoft-graph"></a>Обзор Microsoft Graph

Microsoft Graph открывает доступ к данным и средствам искусственного интеллекта в Microsoft 365. Вы получите единую модель программируемости, которую можно использовать для доступа к колоссальному объему данных в Office 365, Windows 10 и Enterprise Mobility + Security. Используйте многочисленные данные в Microsoft Graph и создавайте приложения с миллионной аудиторией для организаций и пользователей.

## <a name="powering-the-microsoft-365-platform"></a>Расширение возможностей платформы Microsoft 365

![Благодаря Microsoft Graph, его соединителям и подключению к данным можно расширить возможности Microsoft 365 и создавать интеллектуальные приложения.](images/microsoft-graph-dataconnect-connectors-800.png)

Три основных компонента платформы Microsoft 365 упрощают доступ к данным и их поток:

- API Microsoft Graph обеспечивает единую конечную точку, `https://graph.microsoft.com`, для доступа к ценным данным о пользователях и аналитическим сведениям, которые предоставляют ресурсы служб Microsoft 365. С помощью интерфейсов REST API и пакетов SDK вы можете получить доступ к конечной точке и создавать приложения, которые поддерживают сценарии для повышения продуктивности, улучшения совместной работы и обучения, обеспечения безопасности, проверки удостоверений и прав доступа, управления устройствами и многого другого.
- [Подключение к данным Microsoft Graph](#access-microsoft-graph-data-at-scale-using-microsoft-graph-data-connect) предоставляет набор инструментов для оптимизации безопасности и масштабируемой доставки данных Microsoft Graph в популярные хранилища данных Azure. Эти кэшированные данные используются в качестве источников данных для средств разработки Azure, с помощью которых можно создавать интеллектуальные приложения.
- Соединители Microsoft Graph (закрытая предварительная версия) работают во входящем направлении, доставляя внешние данные в службы и приложения Microsoft Graph, а также улучшая возможности настройки.

Одновременное использование API Microsoft Graph, подключения к данным и соединителей (закрытой предварительной версии) позволяет расширить возможности платформы Microsoft 365. Благодаря доступу к данным Microsoft Graph и другим наборам данных для получения статистики и аналитики вы можете расширить возможности Microsoft 365 и создавать уникальные интеллектуальные приложения.

> [!NOTE]
> Соединители Microsoft Graph доступны в закрытой предварительной версии. Участие в программе предварительного просмотра возможно исключительно по приглашению. Подробнее о соединителях см. в статье [Build 2019: Microsoft Graph powers the Microsoft 365 platform](https://aka.ms/microsoftgraphbuild2019) (Сборка 2019. Microsoft Graph расширяет возможности платформы Microsoft 365).

## <a name="whats-in-microsoft-graph"></a>Из чего состоит Microsoft Graph?

Microsoft Graph предоставляет интерфейсы REST API и клиентские библиотеки для доступа к данным в таких службах Microsoft 365:

- Службы Office 365: Delve, Excel, Microsoft Bookings, Microsoft Teams, OneDrive, OneNote, Outlook/Exchange, Планировщик и SharePoint
- Службы Enterprise Mobility and Security: Advanced Threat Analytics, Advanced Threat Protection, Azure Active Directory, Identity Manager и Intune
- Службы Windows 10: действия, устройства, уведомления
- Dynamics 365 Business Central

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
- Анализирует масштабируемые данные Office 365, чтобы лица, принимающие решения, видели важные закономерности сотрудничества и распределения во времени, необходимые для повышения производительности работы.
- Вносит пользовательские бизнес-данные в Microsoft Graph и индексирует их для поиска наряду с данными из служб Microsoft 365.

В качестве примера выберите первый сценарий поиска участников собрания. С помощью API Microsoft Graph вы можете:

1. Получить адреса электронной почты участников [собрания](/graph/api/resources/event?view=graph-rest-1.0).
2. Просмотреть информацию о каждом из них как о [пользователе](/graph/api/resources/user?view=graph-rest-1.0) в Azure Active Directory и [получить сведения о профиле](/graph/api/user-get?view=graph-rest-1.0).

С помощью связей вы можете перейти к другим ресурсам:

- Связаться с его руководителем через [связь с руководителем](/graph/api/user-list-manager?view=graph-rest-1.0).
- Получить полезные сведения, в том числе о популярных файлах, [которые отслеживает](/graph/api/resources/insights-trending?view=graph-rest-beta) пользователь.
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
|   GET группы Office 365, в которые я вхожу| [`https://graph.microsoft.com/v1.0/me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2FmemberOf%2F%24%2Fmicrosoft.graph.group%3F%24filter%3DgroupTypes%2Fany(a%3Aa%2520eq%2520'unified')&version=v1.0) |
|   GET пользователи в моей организации  | [`https://graph.microsoft.com/v1.0/users`](https://developer.microsoft.com/graph/graph-explorer/?request=users&version=v1.0) |
|   GET группы в моей организации | [`https://graph.microsoft.com/v1.0/groups`](https://developer.microsoft.com/graph/graph-explorer/?request=groups&version=v1.0) |
|   GET пользователи, связанные со мной | [`https://graph.microsoft.com/v1.0/me/people`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fpeople&version=beta)  |
|   GET элементы, популярные в моей компании | [`https://graph.microsoft.com/beta/me/insights/trending`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Finsights%2Ftrending&version=beta) |
|   GET мои заметки | [`https://graph.microsoft.com/v1.0/me/onenote/notebooks`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fonenote%2Fnotebooks&version=beta) |

## <a name="access-microsoft-graph-data-at-scale-using-microsoft-graph-data-connect"></a>Доступ к масштабируемым данным Microsoft Graph с помощью подключения к данным

Подключение к данным Microsoft Graph предоставляет набор инструментов для масштабируемого доступа к данным в Microsoft Graph и в то же время позволяет администраторам регулировать согласие и полностью контролировать данные Microsoft Graph. Подключение к данным помогает оптимизировать их доставку в Microsoft Azure.

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

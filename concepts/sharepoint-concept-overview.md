---
title: Обзор API сайтов и контента SharePoint
description: SharePoint — это ваша мобильная интеллектуальная интрасеть. В SharePoint пользователи могут делиться и управлять контентом, знаниями и приложениями при работе в группах, искать необходимую информацию и вести совместную работу в рамках организации. С помощью REST API для SharePoint в Microsoft Graph вы можете интегрировать свои решения с сайтами и контентом SharePoint.
ms.localizationpriority: high
ms.prod: sharepoint
ms.custom: scenarios:getting-started
ms.openlocfilehash: 2ad423d789585263da8bc0812c78337ed9dee6e3
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214589"
---
# <a name="sharepoint-sites-and-content-api-overview"></a>Обзор API сайтов и контента SharePoint

SharePoint — это ваша мобильная интеллектуальная интрасеть. В SharePoint пользователи могут делиться и управлять контентом, знаниями и приложениями при работе в группах, искать необходимую информацию и вести совместную работу в рамках организации. С помощью REST API для SharePoint в Microsoft Graph вы можете интегрировать свои решения с сайтами и контентом SharePoint.

## <a name="why-integrate-with-sharepoint-sites-and-content"></a>Зачем выполнять интеграцию с сайтами и контентом SharePoint?

Сайты SharePoint используются для связи и совместной работы в группах. В основе групп Microsoft 365, Microsoft Teams и порталов лежит SharePoint, поэтому с помощью Microsoft Graph вы можете получать доступ к данным независимо от того, где они хранятся. С помощью API SharePoint в Microsoft Graph вы можете получать доступ к указанным ниже ресурсам.

- Сайты групп. На них хранится контент, над которым совместно работают пользователи со своими коллегами.
- Информационные сайты и порталы, на которых пользователи публикуют страницы с разнообразным контентом, чтобы поделиться им с другими пользователями в организации.

### <a name="unleash-your-data-with-sharepoint-lists"></a>Раскройте все возможности своих данных с помощью списков SharePoint

[Списки][список] — это основные элементы для хранения данных в SharePoint.
Вы можете [создавать списки][создать], чтобы хранить самые разные бизнес-данные: от простого списка контактных данных клиентов до пользовательского бизнес-приложения с интерфейсом Power Apps.
Когда вы используете [столбцы][], чтобы определить свою схему, SharePoint может защитить целостность ваших данных, а также предоставить мощные функции индексирования, создания запросов и поиска.

### <a name="bring-the-power-of-lists-to-your-teams-files"></a>Применение функций списков к файлам группы

SharePoint хранит файлы в [списках особого типа][], называемых библиотеками документов.
С помощью [API OneDrive][] вы можете работать с библиотекой как с [диском][], а с помощью API SharePoint — как со [списком][].
Как и при работе с обычным списком, с помощью настраиваемых столбцов вы можете расширить схему библиотеки документов для удовлетворения своих бизнес-потребностей.

### <a name="light-up-your-app-with-your-users-sharepoint-intranet-data"></a>Наполнение приложения данными пользователей из интрасети SharePoint

С помощью Microsoft Graph вы можете обеспечить доступ к самым важным данным пользователей в своем приложении.
Обновляйте данные, [отправляя запросы][] к списку, в котором хранятся данные ваших пользователей.
[Создавайте][] собственные списки для приложения и предоставляйте пользователям доступ к данным в других интерфейсах SharePoint либо скрывайте данные.

### <a name="use-microsoft-graph-to-extend-sharepoint"></a>Расширение возможностей SharePoint c помощью Microsoft Graph

В качестве платформы SharePoint обеспечивает несколько указанных ниже моделей расширения и интеграции.

- [SharePoint Framework][] позволяет создавать веб-части с помощью клиентских технологий и средств с открытым кодом, которые можно разместить на страницах SharePoint.
- [Надстройки SharePoint][] — это автономные расширения, которые можно добавить на сайт SharePoint без необходимости выполнения пользовательского кода на сервере.

Если ваше приложение работает на странице SharePoint, вы можете без труда получать доступ к данным в Microsoft 365 c помощью Microsoft Graph.

Подробные сведения об этих моделях см. на веб-страницах [центра разработки SharePoint][] и [документов по разработке в SharePoint][].

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API SharePoint в Microsoft Graph 1.0](/graph/api/resources/sharepoint)
- [API SharePoint в бета-версии Microsoft Graph](/graph/api/resources/sharepoint?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>Следующие шаги

Чтобы приступить к работе с SharePoint в Microsoft Graph, изучите дополнительные сведения о [работе с сайтами](/graph/api/resources/sharepoint).

[list]: /graph/api/resources/list
[столбцы]: /graph/api/resources/columndefinition
[тип списка]: /graph/api/resources/listinfo
[создать]: /graph/api/list-create
[создание запросов]: /graph/api/listitem-get
[диск]: /graph/api/resources/drive
[API OneDrive]: /graph/api/resources/onedrive
[SharePoint Framework]: /sharepoint/dev/spfx/sharepoint-framework-overview
[Надстройки SharePoint]: /sharepoint/dev/sp-add-ins/sharepoint-add-ins
[Центр разработки SharePoint]: https://developer.microsoft.com/sharepoint
[Документы по разработке в SharePoint]: /sharepoint/dev/
[SharePoint]: /graph/api/resources/sharepoint

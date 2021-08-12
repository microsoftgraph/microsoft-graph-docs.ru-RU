---
title: Обзор API OneNote
description: OneNote — это цифровая записная книжка, с помощью которой клиенты могут записывать и отслеживать свои идеи и заметки для дома, учебы и работы, вводя данные, рисуя или диктуя текст в Интернете, на телефоне, планшете или настольном компьютере. Они могут свободно упорядочивать заметки, переключаться между устройствами и продолжать работу с места, на котором они закончили ее в прошлый раз. Кроме того, они могут работать над заметками вместе с другими пользователями в режиме реального времени.
author: Jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.custom: scenarios:getting-started
ms.openlocfilehash: 3e92e05d109ed767db75f015c28ce26049cff5e8b085686ed609d355131fe9d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54208701"
---
# <a name="onenote-api-overview"></a>Обзор API OneNote

OneNote — это цифровая записная книжка, с помощью которой клиенты могут записывать и отслеживать свои идеи и заметки для дома, учебы и работы, вводя данные, рисуя или диктуя текст в Интернете, на телефоне, планшете или настольном компьютере. Они могут свободно упорядочивать заметки, переключаться между устройствами и продолжать работу с места, на котором они закончили ее в прошлый раз. Кроме того, они могут совместно работать над заметками с другими пользователями в режиме реального времени.

> [!VIDEO https://www.youtube-nocookie.com/embed/VXd4OeQU1ek]

## <a name="why-integrate-with-onenote"></a>Зачем нужна интеграция с OneNote?

Интегрируя свои приложения с OneNote, вы можете создавать функциональные интерфейсы на различных платформах, доступных миллионам пользователей по всему миру. С помощью Microsoft Graph вы можете получать доступ к записным книжкам, разделам и страницам в OneNote для создания решений, помогающих пользователям планировать и упорядочивать идеи и сведения.

### <a name="collect-and-organize-notes-and-ideas"></a>Сбор и упорядочение заметок и идей  

OneNote можно использовать как холст, где пользователи будут добавлять и упорядочивать содержимое. Microsoft Graph упрощает создание приложений, с помощью которых можно делать учебные заметки и проводить исследования, делиться планами и идеями с родными и близкими, а также обмениваться фотографиями покупок. Приложение может собирать нужные пользователям сведения, отправлять их в OneNote и помогать упорядочивать их.

### <a name="capture-information-in-many-formats"></a>Запись данных во множестве форматов

Записывайте HTML-код, внедряйте изображения (с локального компьютера или общедоступного URL-адреса), видео, звуковые файлы, электронные сообщения и другие файлы распространенных типов. В OneNote даже могут отображаться веб-страницы и PDF-файлы в виде моментальных снимков. Microsoft Graph поддерживает набор стандартных тегов HTML и CSS для разметки страниц OneNote, позволяющий создавать нужное оформление с помощью таблиц, встроенных рисунков и базового форматирования. 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a>Расширение основных сценариев с помощью экосистемы OneNote

Воспользуйтесь широкими возможностями OneNote. API OneNote в Microsoft Graph выполняют распознавание текста с изображений, поддерживают полнотекстовый поиск, автоматически синхронизируют клиенты, обрабатывают изображения, а также извлекают записанные визитные карточки, описания продукции и рецепты из Интернета. Вы можете использовать OneNote в качестве цифрового хранилища в облаке для заметок и небольших файлов мультимедиа, а также в качестве канала для данных, относящихся к определенным доменам. 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a>Доступ для миллионов пользователей OneNote на всех основных платформах

С помощью OneNote вы можете сделать свое приложение более популярным. Приложение OneNote предустановлено на новых устройствах с Windows и доступно на большинстве платформ, в Интернете и в составе Microsoft 365. При публикации приложений, использующих многофункциональную среду OneNote, вам открывается доступ к обширному кроссплатформенному рынку.

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: featured_scenarios..md You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a>Возможности API OneNote в Microsoft Graph

Ниже приводятся некоторые из наиболее популярных запросов для работы с ресурсами OneNote.

|Операция|URL-адрес|
|:--------|:--|
|Получение записных книжек с помощью запроса GET|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/notebooks&version=v1.0)|
|Получение разделов с помощью запроса GET|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/sections&version=v1.0)|
|Получение страниц с помощью запроса GET|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/pages&version=v1.0)|

## <a name="learn-more-about-onenote-apis"></a>Узнайте больше об API OneNote

Подробно изучите API Microsoft Graph, чтобы узнать о возможностях изменения контента в OneNote. В перечисленных ниже статьях рассказывается, как создавать страницы OneNote и добавлять новый контент на существующие страницы. Кроме того, вы узнаете о рекомендациях по использованию Microsoft Graph для изменения записных книжек OneNote. 


### <a name="work-with-onenote"></a>Работа с OneNote

* [Использование REST API для OneNote](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)
* [Рекомендации](onenote-best-practices.md)
* [Рекомендации по использованию фирменной символики](onenote-branding.md)
* [Открытие клиента OneNote](open-onenote-client.md)
* [Использование тегов заметок на страницах OneNote](onenote-note-tags.md)
* [Коды ошибок для API OneNote в Microsoft Graph](onenote-error-codes.md)

### <a name="work-with-onenote-pages"></a>Работа со страницами OneNote

* [Входной и выходной HTML-код на страницах OneNote](onenote-input-output-html.md)
* [Получение содержимого и структуры OneNote с помощью Microsoft Graph](onenote-get-content.md)
* [Создание страниц OneNote](onenote-create-page.md)
* [Обновление содержимого страницы OneNote](onenote-update-page.md)

### <a name="work-with-onenote-page-content"></a>Работа с содержимым страницы в OneNote

* [Создание элементов с абсолютным положением на страницах OneNote](onenote-abs-pos.md)
* [Добавление изображений, видео и файлов на страницы OneNote](onenote-images-files.md)
* [Использование тегов div API OneNote для извлечения данных из записанного содержимого](onenote-extract-data.md)

## <a name="see-also"></a>См. также
Узнайте о других функциях OneNote, которые предоставляются только на конечной точке REST для службы OneNote.

- [Разработка для OneNote](/previous-versions/office/office-365-api/how-to/onenote-landing)
- [Работа с записными книжками для занятий](/previous-versions/office/office-365-api/how-to/onenote-classnotebook)
- [Работа с асинхронными записными книжками для занятий](/previous-versions/office/office-365-api/how-to/onenote-classnotebook-asynchronous)
- [Работа со служебными записными книжками](/previous-versions/office/office-365-api/how-to/onenote-staffnotebook)
- [Копирование записных книжек, разделов и страниц](/previous-versions/office/office-365-api/how-to/onenote-copy)
- [Управление разрешениями на объекты OneNote](/previous-versions/office/office-365-api/how-to/onenote-manage-perms)
- [Использование диалогового окна сохранения OneNote на веб-страницах](/previous-versions/office/office-365-api/how-to/onenote-save-dialog)
- [Подписка на веб-перехватчики](/previous-versions/office/office-365-api/how-to/onenote-sync)

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API OneNote в Microsoft Graph 1.0](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)
- [API OneNote в бета-версии Microsoft Graph](/graph/api/resources/onenote-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

Используйте [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer), чтобы опробовать API OneNote с собственными записными книжками OneNote.

Чтобы отправлять вызовы API OneNote из песочницы Graph, нажмите **Показать другие примеры** в столбце слева. **Включите** OneNote с помощью меню. Вам также потребуется включить соответствующие разрешения. В меню слева под именем учетной записи выберите **Изменить разрешения**. Дополнительные сведения о разрешениях OneNote см. в разделе [Разрешения для заметок](permissions-reference.md#notes-permissions).

Сведения о том, как приступить к работе с API OneNote в Microsoft Graph, см. в [справочных материалах по OneNote](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0).
---
title: Обзор API для хранилища файлов OneDrive
description: OneDrive является центром файлов в Microsoft 365.
ms.localizationpriority: high
ms.prod: onedrive
ms.custom: scenarios:getting-started
ms.openlocfilehash: 080d05a3fbba08108b14048968dee47fa1cd2dbc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019085"
---
# <a name="onedrive-file-storage-api-overview"></a>Обзор API для хранилища файлов OneDrive

OneDrive является центром файлов в Microsoft 365.
Люди работают с файлами в различных контекстах, например Microsoft Teams, группах, SharePoint и т. д.
С OneDrive пользователи открывать эти файлы независимо от того, где они хранятся, а с Microsoft Graph для работы с ними можно использовать один API.

Файлы в Microsoft 365 хранятся на [дисках][Drive API].
Пользователи могут хранить файлы на личном (своем OneDrive) либо общем диске на базе библиотеки документов [SharePoint][].
Гибкость OneDrive позволяет пользователям работать с коллегами так, как им удобно.
Пользователи могут делиться ссылками на файлы, копировать либо перемещать файлы на диски групп или даже прикреплять файлы OneDrive к почтовым сообщениям в Outlook.

> [!VIDEO https://www.youtube-nocookie.com/embed/vG-hQxFHCAE]

## <a name="why-integrate-with-onedrive-file-storage-in-the-cloud"></a>Преимущества интеграции с облачным файловым хранилищем OneDrive?

### <a name="tap-into-an-ecosystem-with-billions-of-files"></a>Использование экосистемы с миллиардами файлов

Пользователи OneDrive могут получать доступ к своим файлам с любого устройства как подключением, так и без подключения к Интернету, и делиться ими с коллегами, так и с внешними пользователями.
OneDrive позволяет совместно работать над документами в режиме реального времени в знакомых приложениях, таких как Word, Excel и PowerPoint.
Платформа Microsoft Graph обеспечивает информативные эскизы для сотен форматов файлов, потоковой передачи видео, аналитики и многого другого.
Данные в OneDrive защищены передовыми технологиями шифрования, соответствия требованиям и безопасности, которым доверяют клиенты.

Поскольку приложение OneDrive работает на более чем 500 миллионах устройств и более 85 % компаний из списка Fortune 500 используют OneDrive для бизнеса, интеграция вашего приложения с OneDrive позволит вам охватить миллионы потребителей, учащихся и бизнес-пользователей и взаимодействовать с клиентами там, где они уже работают каждый день.

### <a name="store-your-apps-files-in-a-powerful-cloud"></a>Хранение файлов вашего приложения в мощном облаке

Когда вы храните файлы в OneDrive, ваше приложение может использовать возможности облака Майкрософт, а ваши пользователи могут получать доступ к своим файлам, где бы они ни находились.
Используйте пакет SDK для [средства выбора файлов][], чтобы быстро открывать, скачивать и сохранять файлы, хранимые в OneDrive, а также делиться ими из вашего приложения через знакомый интерфейс OneDrive.
Получайте информацию о выбранных файлах прямо из пакета SDK или используйте API Microsoft Graph для более глубокого взаимодействия с файлами.
Используйте [специальные папки][], чтобы хранить файлы в известных папках OneDrive, например `Documents` и `Camera Roll`, или предоставьте своему приложению собственную папку.

### <a name="bring-your-app-straight-to-users-within-onedrive"></a>Подача вашего приложения напрямую пользователям в OneDrive

Клиенты OneDrive могут запускать ваше приложение прямо из OneDrive, чтобы открывать, редактировать или просматривать файлы.
Используйте расширения [обработчика файлов][] OneDrive, чтобы предоставить значки и эскизы для своих расширений файлов; добавьте свое приложение в кнопку **Создать** или даже действия в строку меню для запуска своего приложения.

### <a name="work-with-content-in-formats-your-app-understands"></a>Работа с содержимым в форматах, которые понимает ваше приложение

Ваше приложение может получить содержимое в наиболее удобном для вас формате.
Приложение может отображать [эскизы][] нестандартного размера для сотен различных форматов файлов.
Вы можете скачивать файлы в различных альтернативных [форматах][], например PDF.
Вы даже можете внедрить предварительный просмотр файлов OneDrive в свое приложение, воспользовавшись API [предварительного просмотра][] (бета-версия).

### <a name="work-with-file-content-and-metadata-without-downloading-the-binary"></a>Работа с содержимым и метаданными файла без скачивания двоичных данных

Microsoft Graph открывает доступ к различному содержимому через REST API без необходимости скачивания двоичных данных.
Изучайте извлеченные метаданные из [фотографий][], [аудиофайлов][] и [видеофайлов][].
Используйте [API Excel][] для работы с необработанными данными, хранящимися в книге Excel.
Используйте [API заметок][] для доступа к содержимому записных книжек OneNote.

### <a name="react-to-file-changes"></a>Реагирование на изменения файлов

С помощью [веб-перехватчиков][] ваше приложение может получать уведомления при изменении файлов, чтобы вы могли быстро отреагировать.
Используйте [API изменений][], чтобы посмотреть, что изменилось с момента последней синхронизации вашего приложения с облаком.

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API для хранилища файлов OneDrive в Microsoft Graph 1.0](/graph/api/resources/onedrive?view=graph-rest-1.0)
- [API для хранилища файлов OneDrive в бета-версии Microsoft Graph](/graph/api/resources/onedrive?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

Узнайте больше об [использовании API OneDrive][Drive API] в Microsoft Graph версии 1.0.

[SharePoint]: sharepoint-concept-overview.md
[средство выбора файлов]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[обработчик файлов]: /onedrive/developer/file-handlers
[специальные папки]: /graph/api/drive-get-specialfolder?view=graph-rest-1.0
[API заметок]: integrate-with-onenote.md
[API Excel]: /graph/api/resources/excel?view=graph-rest-1.0
[REST API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[API изменений]: /graph/api/driveitem-delta?view=graph-rest-1.0
[видео]: /graph/api/resources/video?view=graph-rest-1.0
[фото]: /graph/api/resources/photo?view=graph-rest-1.0
[аудио]: /graph/api/resources/audio?view=graph-rest-1.0
[форматы]: /graph/api/driveitem-get-content-format?view=graph-rest-1.0
[эскизы]: /graph/api/driveitem-list-thumbnails?view=graph-rest-1.0
[предварительный просмотр]: /graph/api/driveitem-preview?view=graph-rest-beta
[веб-перехватчики]: /graph/api/resources/webhooks?view=graph-rest-1.0
[Drive API]: /graph/api/resources/onedrive?view=graph-rest-1.0

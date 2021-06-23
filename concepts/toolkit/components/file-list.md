---
title: Компонент списка файлов в microsoft Graph набор средств
description: Компонент списка файлов используется для отображения списка файлов, показывая их значок и имя
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 89f60020fb1db75ed4e79a7402b0aa0518146130
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082176"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a>Компонент списка файлов в microsoft Graph набор средств

Компонент Списка файлов [](/graph/api/resources/onedrive) отображает список нескольких папок и файлов с помощью имени файла или папки, значка и других свойств, которые вы указываете. Этот компонент использует [компонент mgt-file.](./file.md) Вы можете указать определенный диск или сайт, отобразить список файлов, основанный на типе insight (трендовые, используемые или общие), или предоставить запросы в настраиваемый список файлов.

## <a name="example"></a>Пример

В следующем примере отображается файл с помощью `mgt-file-list` компонента. Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file-list--file-list&source=docs" height="250"></iframe>

[Открыть этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-file-list--file-list&source=docs)

## <a name="properties"></a>Свойства

Для настройки компонента можно использовать несколько свойств.

| Атрибут | Свойство | Описание |
| --------- | -------- | ----------- |
| файл-список-запрос | fileListQuery | Полный запрос или путь к диску или сайту, содержащий список отрисовки файлов. |
| файл-запросы | fileQueries | Массив файлового запроса, отрисовываемого компонентом. |
| нет | files | Массив файлов для получения или набора списка файлов, отрисовываний компонентом. Используйте это для доступа к файлам, загруженным компонентом. Установите это значение для загрузки собственных файлов. |
| тип insight | insightType | Установите для демонстрации трендовых, используемых или общих файлов пользователя. |
| drive-id | driveId | ID диска, к которой принадлежит папка. Также необходимо предоставить либо `item-id` `item-path` . |
| group-id | groupId | ID группы, которой принадлежит папка. Также необходимо предоставить либо `item-id` `item-path` . |
| site-id | siteId | ID сайта, к которой принадлежит папка. Также необходимо предоставить либо `{item-id}` `{item-path}` . `{list-id}`Укай, если вы ссылаетесь на файл из определенного списка. |
| item-id | itemId | ID папки. Запрос по умолчанию `/me/drive/items` . Предоставление `{drive-id}` , или запрос `{group-id}` `{site-id}` `{user-id}` определенного расположения. |
| путь элемента | itemPath | Путь элемента папки (относительно корневого). Запрос по умолчанию `/me/drive/root` . Предоставление `{drive-id}` , или запрос `{group-id}` `{site-id}` `{user-id}` определенного расположения. |
| размер страницы | pageSize | Значение числа, чтобы указать максимальное количество файлов, которые необходимо отрисовки на каждой странице. |
| расширения файлов | fileExtensions | Массив расширений файлов, используемых для фильтрации файлов для показа. |
| кнопка hide-more-files-button | hideMoreFilesButton | A boolean to indicate whether to show a button to render more files. |

В следующем примере изменяется поведение компонента для получения списка файлов из определенного запроса.

```html
<mgt-file-list file-list-query="/me/drive/items/01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY/children"></mgt-file-list>
```

В следующем примере изменяется поведение компонента для получения списка файлов из папки, предоставляя id папки.

```html
<mgt-file-list item-id="01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY"></mgt-file-list>
```

В следующем примере изменяется поведение компонента для получения списка файлов из группы, предоставляя групповой id и путь папки.

```html
<mgt-file-list group-id="8090c93e-ba7c-433e-9f39-08c7ba07c0b3" item-path="/Design"></mgt-file-list>
```

В следующем примере изменяется поведение компонента для получения списка файлов от пользователя, предоставляя пользовательский ид папки.

```html
<mgt-file-list user-id="48d31887-5fad-4d73-a9f5-3c356e68a038" item-id="01BYE5RZYFPM65IDVARFELFLNTXR4ZKABD"></mgt-file-list>
```

В следующем примере изменяется поведение компонента для получения списка файлов, предоставляя тип проницательности.

```html
<mgt-file-list insight-type="shared"></mgt-file-list>
```

## <a name="methods"></a>Методы
| Метод | Описание |
| --- | --- |
| перезагрузка (clearCache = false) | Вызывает метод для перезагрузки компонента с потенциальными новыми данными на основе его свойств. Перед перезагрузки необходимо очистить `true` кэш. |

## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

Компонент `mgt-file-list` определяет следующие настраиваемые свойства CSS.

```css
mgt-file-list {
  --font-family: 'Segoe UI';
  --font-size: 14px;

  --file-list-background-color: #ffffff;
  --file-list-border: none;
  --file-list-box-shadow: none;
  --file-list-padding: 4px 0;
  --file-list-margin: 0;

  --file-item-background-color--hover: rgba(0, 0, 0, 0.1);
  --file-item-background-color--active: rgba(0, 0, 0, 0.05);
  --file-item-border-radius: 2px;
  --file-item-margin: 0 4px;

  --file-item-border-top: none;
  --file-item-border-left: none;
  --file-item-border-right: none;
  --file-item-border-bottom: none;

  --show-more-button-background-color: #f3f2f1;
  --show-more-button-background-color--hover: rgba(0, 0, 0, 0.1);
  --show-more-button-font-size: 12px;
  --show-more-button-padding: 6px;
  --show-more-button-border-bottom-right-radius: 4px;
  --show-more-button-border-bottom-left-radius: 4px;
}
```

Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).

## <a name="microsoft-graph-apis-and-permissions"></a>Страница "Разрешения API и приложений Microsoft Graph"

| Настройка | Разрешения | API |
| ------------- | ----------------- | --- |
| По умолчанию (не предоставлены идентификаторы или запросы) | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/root/children` |
| Предоставление `{drive-id}` И `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /drives/{drive-id}/items/{item-id}/children` |
| Предоставление `{group-id}` И `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| Предоставление ТОЛЬКО `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/items/{item-id}/children` |
| Предоставление `{site-id}` И `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| Pprovide `{user-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /users/{user-id}/drive/items/{item-id}/children` |
| Предоставление `{drive-id}` И `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| Предоставление `{group-id}` И `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /groups/{group-id}/root:/{item-path}:/children` |
| Предоставление `{site-id}` И `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/root:/{item-path}:/children` |
| Предоставление `{user-id}` И `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /users/{user-id}/root:/{item-path}:/children` |
| Предоставление только `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/root:/{item-path}:/children` |
| `insight-type` настроена на трендовую | Sites.Read.All | `GET /me/insights/trending` |
| Обеспечить `{user-id or upn}` и `insight-type` установить для `trending` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/trending` |
| `insight-type` установлено, что `used` | Sites.Read.All | `GET /me/insights/used` |
| Обеспечить `{user-id or upn}` и `insight-type` установить для `used` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/used` |
| `insight-type` настроено на общий доступ | Sites.Read.All | `GET /me/insights/shared` |
| Обеспечить `{user-id or upn}` и `insight-type` установить для `shared` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a>События

| Событие | Описание |
| ----- | ----------- |
| `itemClick` | Уволили, когда пользователь щелкнуть файл. Возвращает сведения о файле. |

Дополнительные сведения об обработке событий см. в [этой работе.](../customize-components/events.md)

## <a name="templates"></a>Шаблоны

Компонент `mgt-file-list` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента. Чтобы указать шаблон, включи элемент внутри компонента и закажите значение для одного из типов данных, перечисленных `<template>` `data-type` в следующей таблице.

| Тип данных | Контекст данных | Описание |
| ----------- | -------------- | ------------ |
| default | `files`: список объектов файлов | Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом. |
| file | `file`: объект файла | Шаблон, используемый для отрисовки каждого файла. |
| no-data | Контекст данных не передан | Шаблон, используемый, если данные недоступны. |
| loading | Контекст данных не передан | Шаблон, используемый при загрузке состояния компонента. |

## <a name="authentication"></a>Проверка подлинности

Для получения требуемых данных в средстве управления используется глобальный поставщик проверки подлинности, указанный в [документации по проверке подлинности](../providers/providers.md).

## <a name="cache"></a>Кэш

|Хранилище объектов|Кэшные данные|Примечания|
|---------|-----------|-------|
|`fileLists`|Список списков файлов|Список кэша по умолчанию для хранения списков файлов.|
|`insightfileLists`|Список списков файлов анализа|Используется при `insightType` условии.|

> [!NOTE]
> Компонент `mgt-file-list` также использует хранилище объектов в IndexedDB для `fileQueries` `mgt-file` кэша файлов при `fileQueries` условии.

Сведения о настройке кэша см. в материале [Caching.](../customize-components/cache.md)
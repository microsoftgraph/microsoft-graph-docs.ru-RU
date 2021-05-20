---
title: Компонент файла в microsoft Graph набор средств
description: Компонент файла используется для отображения файла, показывая значок и имя
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 314f08d396421c3b0afe0cf049e91cca9daa03fd
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579858"
---
# <a name="file-component-in-the-microsoft-graph-toolkit"></a>Компонент файла в microsoft Graph набор средств

Компонент File используется для представления отдельного файла или папки из OneDrive или [SharePoint](/graph/onedrive-concept-overview) путем отображения таких сведений, как имя файла или папки, значок с указанием типа файла и других свойств, таких как автор, последняя измененная дата или другие сведения. Вы можете предоставить идентификаторы для файла, и компонент будет создавать запрос для получения файла на основе предоставленных идентификаторов. Этот компонент можно использовать самостоятельно или в составе компонентов [mgt-file-list.](./file-list.md)

## <a name="example"></a>Пример

В следующем примере отображается файл с помощью `mgt-file` компонента. Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file--file&source=docs" height="250"></iframe>

[Открыть этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-file--file&source=docs)

## <a name="properties"></a>Свойства

Для настройки компонента можно использовать несколько свойств.

| Атрибут | Свойство | Описание |
| --------- | -------- | ----------- |
| файл-запрос | fileQuery | Полный запрос или путь к файлу, который будет извлечен. |
| drive-id | driveId | ID диска, к которой принадлежит файл. Также необходимо предоставить либо `item-id` `item-path` . |
| group-id | groupId | ID группы, которой принадлежит файл. Также необходимо предоставить либо `item-id` `item-path` . |
| site-id | siteId | ID сайта, на который принадлежит файл. Также необходимо предоставить либо `{item-id}` `{item-path}` . `{list-id}`Предокапь также, если вы ссылаетесь на файл из определенного списка. |
| list-id | listId | ID списка, к которой принадлежит файл. Также необходимо предоставить `{site-id}` и `{item-id}` . |
| item-id | itemId | ID файла. Запрос по умолчанию `/me/drive/items` . Предоставление `{drive-id}` , или запрос `{group-id}` `{site-id}` `{user-id}` определенного расположения. |
| путь элемента | itemPath | Путь элемента файла. Запрос по умолчанию `/me/drive/root` . Предоставление `{drive-id}` , или запрос `{group-id}` `{site-id}` `{user-id}` определенного расположения. |
| тип insight | insightType | Тип анализа файла, извлеченного из. Может быть `trending` `used` , или `shared` . |
| insight-id | insightId | ID ресурса insight. |
| сведения о файле | fileDetails | Настройка объекта, представляющего файл |
| значок file-icon | fileIcon | Настройка значка для показа файла |
| представление | представление | Установите для управления тем, как отрисовка файла. Значение по умолчанию: `oneline`. <br>`image` - показать только значок <br>`oneline` - покажите значок и одну строку текста (по умолчанию — `name` файл) <br>`twolines` - покажите значок и две строки текста `name` (и `lastModifiedDateTime` по умолчанию)<br> `threelines` - покажите значок и три строки текста `name` `lastModifiedDateTime` (и `displayName` автора по умолчанию) |
| line1-property | line1Property | Задает свойство `fileDetails` использовать для первой строки текста. По умолчанию `name` это файл. |
| line2-property | line2Property | Задает свойство `fileDetails` использовать для второй строки текста. Значение по умолчанию: `lastModifiedDateTime`. |
| line3-property | line3Property | Задает свойство `fileDetails` для использования для третьей строки текста. По умолчанию `size` это файл. |

Следующий пример демонстрирует изменение поведения компонента для извлечения данных из определенного запроса.

```html
<mgt-file file-query="/me/drive/items/01BYE5RZZFWGWWVNHHKVHYXE3OUJHGWCT2"></mgt-file>
```

В следующем примере изменяется поведение компонента для получения данных из определенного запроса, покажите три строки информации — имя файла, время последней измененной даты и размер файла по умолчанию — и задайте значок файла.

```html
<mgt-file file-query="/me/drive/items/01BYE5RZZFWGWWVNHHKVHYXE3OUJHGWCT2" view="threeLines" file-icon="ICON_PATH"></mgt-file>
```

В следующем примере изменяется поведение компонента для получения данных с определенного диска.

```html
<mgt-file drive-id="b!-RIj2DuyvEyV1T4NlOaMHk8XkS_I8MdFlUCq1BlcjgmhRfAj3-Z8RY2VpuvV_tpd" item-id="01BYE5RZ5MYLM2SMX75ZBIPQZIHT6OAYPB"></mgt-file>
```

В следующем примере изменяется behabior компонента для получения данных с SharePoint сайта и пути.

```html
  <mgt-file site-id="m365x214355.sharepoint.com,5a58bb09-1fba-41c1-8125-69da264370a0,9f2ec1da-0be4-4a74-9254-973f0add78fd" item-Path="/DemoDocs/AdminDemo"></mgt-file>
```

В следующем примере изменяется поведение компонента для получения данных по типу insight.

```html
<mgt-file insight-type="shared" insight-id="AW1GxMvkOztMkJX-SCppUSRPF5EvyPDHRZVAqtQZXI4JoUXwI9_mfEWNlabr1f7aXRBWDMt2C2FDop4fP1vsUw9tRsTL5Ds7TJCV_kgqaVEkBA"></mgt-file>
```

## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

Компонент `mgt-file` определяет следующие настраиваемые свойства CSS.

```css
mgt-file {
  --file-type-icon-size: 28px;
  --file-border: none;
  --file-box-shadow: none;
  --file-background-color: #ffffff;

  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 400;
  --text-transform: none;
  --color: #323130;

  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: #797775;
  --line2-text-transform: none;

  --line3-font-size: 12px;
  --line3-font-weight: 400;
  --line3-color: #797775;
  --line3-text-transform: none;
}
```

Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).

## <a name="microsoft-graph-apis-and-permissions"></a>Страница "Разрешения API и приложений Microsoft Graph"

Этот элемент управления использует следующие API и разрешения Microsoft Graph.

| Конфигурация | Области разрешений | API |
| ------------- | ----------------- | --- |
| Разработчик предоставляет `{drive-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /drives/{drive-id}/items/{item-id}` |
| Разработчик предоставляет `{drive-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /drives/{drive-id}/root:/{item-path}` |
| Разработчик предоставляет `{group-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /groups/{group-id}/drive/items/{item-id}` |
| Разработчик предоставляет `{group-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /groups/{group-id}/drive/root:/{item-path}` |
| Разработчик предоставляет ONLY `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/items/{item-id}` |
| Разработчик предоставляет ONLY `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/root:/{item-path}` |
| Разработчик предоставляет `{site-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/drive/items/{item-id}` |
| Разработчик предоставляет `{site-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/drive/root:/{item-path}` |
| Разработчик предоставляет `{site-id}` AND `{list-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/lists/{list-id}/items/{item-id}/driveItem` |
| Разработчик предоставляет `{user-id}` AND `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /users/{user-id}/drive/items/{item-id}` |
| Разработчик предоставляет `{user-id}` AND `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /users/{user-id}/drive/root:/{item-path}` |
| `insight-type` настроена на `trending` И разработчик предоставляет `{insight-id}` | Sites.Read.All | `GET /me/insights/trending/{insight-id}/resource` |
| Разработчик предоставляет `{user-id or upn}` `{insight-id}` И И `insight-type` заме- `trending` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/trending/{insight-id}/resource` |
| `insight-type` настроена на `used` И разработчик предоставляет `{insight-id}` | Sites.Read.All | `GET /me/insights/used/{id}/resource` |
| Разработчик предоставляет `{user-id or upn}` `{insight-id}` И И `insight-type` заме- `used` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/used/{id}/resource` |
| `insight-type` предоставляет `shared` разработчик AND `{insight-id}` | Sites.Read.All | `GET /me/insights/shared/{id}/resource` |
| Разработчик предоставляет `{user-id or upn}` `{insight-id}` И И `insight-type` заме- `shared` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/shared/{id}/resource` |

## <a name="templates"></a>Шаблоны

Компонент `mgt-file` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить его определенные части. Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.

| Тип данных | Контекст данных | Описание |
| ----------- | -------------- | ------------- |
| загрузка | Нет | Шаблон для отображения состояния загрузки компонента. |
| no-data | Нет | Шаблон, который необходимо отрисовки, если нет данных файла. |
| default | файл: объект сведений о файле | Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом. |

## <a name="authentication"></a>Проверка подлинности

Для получения требуемых данных в средстве управления используется глобальный поставщик проверки подлинности, указанный в [документации по проверке подлинности](../providers/providers.md).

## <a name="cache"></a>Кэш

|Хранилище объектов|Кэшные данные|Примечания|
|---------|-----------|-------|
|`driveFiles`|Список файлов по дисковой id|Используется при `driveId` условии|
|`groupFiles`|Список файлов по групповому id|Используется при `groupId` условии|
|`siteFiles`|Список файлов по id сайта|Используется при `siteId` условии|
|`userFiles`|Список файлов по пользовательскому id|Используется при `userId` условии|
|`insightFiles`|Список файлов по сведениям|Используется, `insightType` `insightId` когда и предоставляется|
|`fileQueries`|Список файлов по запросам|Используется при `fileQuery` условии|

Сведения о настройке кэша см. в материале [Caching.](../customize-components/cache.md)
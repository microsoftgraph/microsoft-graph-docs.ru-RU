---
title: Компонент списка файлов в microsoft Graph набор средств
description: Компонент списка файлов используется для отображения списка файлов, показывая их значок и имя
ms.localizationpriority: medium
author: beth-panx
ms.openlocfilehash: 1f3aea2c4d012cd4627167523540fcfeaaaf7651
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035348"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a>Компонент списка файлов в microsoft Graph набор средств

Компонент Списка файлов [](/graph/api/resources/onedrive) отображает список нескольких папок и файлов с помощью имени файла или папки, значка и других свойств, которые вы указываете. Этот компонент использует [компонент mgt-file.](./file.md) Вы можете указать определенный диск или сайт, отобразить список файлов, основанный на типе insight (трендовые, используемые или общие), или предоставить запросы в настраиваемый список файлов. Компонент также предоставляет возможность разрешить пользователям загружать файлы в указанное расположение в One Drive или SharePoint.

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
| Нет | files | Массив файлов для получения или набора списка файлов, отрисовываний компонентом. Используйте это для доступа к файлам, загруженным компонентом. Установите это значение для загрузки собственных файлов. |
| тип insight | insightType | Установите для демонстрации трендовых, используемых или общих файлов пользователя. |
| drive-id | driveId | ID диска, к которой принадлежит папка. Также необходимо предоставить либо `item-id` `item-path` . |
| group-id | groupId | ID группы, которой принадлежит папка. Также необходимо предоставить либо `item-id` `item-path` . |
| site-id | siteId | ID сайта, к которой принадлежит папка. Также необходимо предоставить либо `{item-id}` `{item-path}` . `{list-id}`Укай, если вы ссылаетесь на файл из определенного списка. |
| item-id | itemId | ID папки. Запрос по умолчанию `/me/drive/items` . Предоставление `{drive-id}` , или запрос `{group-id}` `{site-id}` `{user-id}` определенного расположения. |
| путь элемента | itemPath | Путь элемента папки (относительно корневого). Запрос по умолчанию `/me/drive/root` . Предоставление `{drive-id}` , или запрос `{group-id}` `{site-id}` `{user-id}` определенного расположения. |
| размер страницы | pageSize | Значение числа, чтобы указать максимальное количество файлов, которые необходимо отрисовки на каждой странице. **Примечание:** `page-size` не поддерживается `insight-type` . |
| расширения файлов | fileExtensions | Массив расширений файлов, используемых для фильтрации файлов для показа. |
| кнопка hide-more-files-button | hideMoreFilesButton | Boolean, чтобы указать, следует ли показывать кнопку, чтобы отрисовывать больше файлов. |
| загрузка файлов с помощью enable-file | enableFileUpload | Boolean, чтобы включить или отключить функции загрузки файлов. Значение по умолчанию — `false`.  |
| исключенные расширения файлов | excludedFileExtensions | Строковая массива расширений файлов, которые будут исключены из загрузки файлов. Должен также установить `enable-file-upload` атрибут `true` . |
| max-file-size | maxFileSize | Число, представляющее максимальный размер загрузки файла (KB). Должен также установить `enable-file-upload` атрибут `true` . |
| max-upload-file | maxUploadFile | Число, представляющее максимальное количество файлов, разрешенных к отправке. По умолчанию значение — `10` файлы. Должен также установить `enable-file-upload` атрибут `true` . |

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

В следующем примере включается функция загрузки файлов.

```html
<mgt-file-list enable-file-upload></mgt-file-list>
```

В следующем примере максимальное число файлов, которые можно загрузить, ограничивается 5.

```html
<mgt-file-list max-upload-file="5" enable-file-upload></mgt-file-list>
```

В следующем примере максимальный размер файла может быть загружен до 10000 КБ.

```html
<mgt-file-list max-file-size="10000" enable-file-upload></mgt-file-list>
```

В следующем примере исключается отправка файлов с расширениями файлов ".doc .pdf".

```html
<mgt-file-list excluded-file-extensions=".doc,.pdf" enable-file-upload></mgt-file-list>
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

  --file-upload-border: 4px dotted #ffbdc3;
  --file-upload-background-color: rgba(255, 0, 0, 0.1);
  --file-upload-button-float: left;
  --file-upload-button-color: #323130;
  --file-upload-button-background-color: #fef8dd;
  --file-upload-dialog-content-background-color: #ffe7c7;
  --file-upload-dialog-primarybutton-background-color: #ffe7c7;
  --file-upload-dialog-primarybutton-color: #323130;
}
```

Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).

## <a name="microsoft-graph-apis-and-permissions"></a>Страница "Разрешения API и приложений Microsoft Graph"

| Настройка | Разрешения | API |
| ------------- | ----------------- | --- |
| По умолчанию (не предоставлены идентификаторы или запросы) | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/root/children` |
| Предоставление `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /me/drive/root/children` <br /> `PUT /me/drive/root:/{filename}:/content` <br /> `POST /me/drive/root:/{filename}:/createUploadSession` |
| Предоставление `{drive-id}` И `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /drives/{drive-id}/items/{item-id}/children`|
| Предоставление `{drive-id}` и `{item-id}` и `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /drives/{drive-id}/items/{item-id}/children` <br /> `PUT /drives/{drive-id}/items/{item-id}:/{filename}:/content` <br /> `POST /drives/{drive-id}/items/{item-id}:/{filename}:/createUploadSession` |
| Предоставление `{group-id}` И `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| Предоставление `{group-id}` и `{item-id}` и `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /groups/{group-id}/drive/items/{item-id}/children` <br /> `PUT /groups/{group-id}/drive/items/{item-id}:/{filename}:/content` <br /> `POST /groups/{group-id}/drive/items/{item-id}:/{filename}:/createUploadSession` |
| Предоставление ТОЛЬКО `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/items/{item-id}/children` |
| Предоставление ТОЛЬКО `{item-id}` И `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /me/drive/items/{item-id}/children` <br /> `PUT /me/drive/items/{item-id}:/{filename}:/content` <br /> `POST /me/drive/items/{item-id}:/{filename}:/createUploadSession` |
| Предоставление `{site-id}` И `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| Предоставление `{site-id}` и `{item-id}` и `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /sites/{site-id}/drive/items/{item-id}/children` <br /> `PUT /sites/{site-id}/drive/items/{item-id}:/{filename}:/content` <br /> `POST /sites/{site-id}/drive/items/{item-id}:/{filename}:/createUploadSession` |
| Предоставление `{user-id}` И `{item-id}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /users/{user-id}/drive/items/{item-id}/children` |
| Предоставление `{user-id}` и `{item-id}` и `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /users/{user-id}/drive/items/{item-id}/children` <br /> `PUT /users/{user-id}/drive/items/{item-id}:/{filename}:/content` <br /> `POST /users/{user-id}/drive/items/{item-id}:/{filename}:/createUploadSession` |
| Предоставление `{drive-id}` И `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| Предоставление `{drive-id}` и `{item-path}` и `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /drives/{drive-id}/root:/{item-path}:/children` <br /> `PUT /drives/{drive-id}/root:/{item-path}/{filename}:/content` <br /> `POST /drives/{drive-id}/root:/{item-path}/{filename}:/createUploadSession` |
| Предоставление `{group-id}` И `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /groups/{group-id}/root:/{item-path}:/children` |
| Предоставление `{group-id}` и `{item-path}` и `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /groups/{group-id}/root:/{item-path}:/children` <br /> `PUT /groups/{group-id}/root:/{item-path}/{filename}:/content` <br /> `POST /groups/{group-id}/root:/{item-path}/{filename}:/createUploadSession` |
| Предоставление `{site-id}` И `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /sites/{site-id}/root:/{item-path}:/children` |
| Предоставление `{site-id}` и `{item-path}` и `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /sites/{site-id}/root:/{item-path}:/children` <br /> `PUT /sites/{site-id}/root:/{item-path}/{filename}:/content` <br /> `POST /sites/{site-id}/root:/{item-path}/{filename}:/createUploadSession` |
| Предоставление `{user-id}` И `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /users/{user-id}/root:/{item-path}:/children` |
| Предоставление `{user-id}` и `{item-path}` и `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /users/{user-id}/root:/{item-path}:/children` <br /> `PUT /users/{user-id}/root:/{item-path}/{filename}:/content` <br /> `POST /users/{user-id}/root:/{item-path}/{filename}:/createUploadSession` |
| Предоставление только `{item-path}` | Files.Read, Files.Read.All, Sites.Read.All | `GET /me/drive/root:/{item-path}:/children` |
| Предоставление только `{item-path}` И `enable-file-upload` | Files.Read, Files.Read.All, Sites.Read.All, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All | `GET /me/drive/root:/{item-path}:/children` <br /> `PUT /me/drive/root:/{item-path}/{filename}:/content` <br /> `POST /me/drive/root:/{item-path}/{filename}:/createUploadSession` |
| `insight-type` настроена на трендовую | Sites.Read.All | `GET /me/insights/trending` |
| Обеспечить `{user-id or upn}` и `insight-type` установить для `trending` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/trending` |
| `insight-type` установлено, что `used` | Sites.Read.All | `GET /me/insights/used` |
| Обеспечить `{user-id or upn}` и `insight-type` установить для `used` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/used` |
| `insight-type` настроено на общий доступ | Sites.Read.All | `GET /me/insights/shared` |
| Обеспечить `{user-id or upn}` и `insight-type` установить для `shared` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a>События

Событие | Когда он излучается | Настраиваемые данные | Отмена | Пузыри | Работает с настраиваемой шаблонной
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`itemClick` | Уволили, когда пользователь щелкнуть файл. | Выбранный [файл](/graph/api/resources/driveItem) | Нет | Нет | Да, с пользовательским **шаблоном файла**

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

|Хранилище объектов|Кэшные данные|Замечания|
|---------|-----------|-------|
|`fileLists`|Список списков файлов|Список кэша по умолчанию для хранения списков файлов.|
|`insightfileLists`|Список списков файлов анализа|Используется при `insightType` условии.|

> [!NOTE]
> Компонент `mgt-file-list` также использует хранилище объектов в IndexedDB для `fileQueries` `mgt-file` кэша файлов при `fileQueries` условии.

Сведения о настройке кэша см. в материале [Caching.](../customize-components/cache.md)

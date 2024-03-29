---
title: Работа с файлами в Microsoft Graph
description: С помощью Microsoft Graph можно создать приложение, которое подключается к файлам в OneDrive, OneDrive для бизнеса и библиотеках документов SharePoint.
ms.localizationpriority: high
ms.prod: sharepoint
author: jewan-microsoft
doc_type: conceptualPageType
ms.openlocfilehash: cc7c4554ebc877d87590547f14d2cfd0d52a01bb
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647100"
---
# <a name="working-with-files-in-microsoft-graph"></a>Работа с файлами в Microsoft Graph

С помощью Microsoft Graph можно создать приложение, которое подключается к файлам в OneDrive, OneDrive для бизнеса и библиотеках документов SharePoint. Используя Microsoft Graph, вы можете создавать различные решения для работы с файлами в Microsoft 365. Возможны варианты как для простого хранения документов пользователей, так и сложные сценарии совместного использования файлов.

В Microsoft Graph доступны два типа ресурсов для работы с файлами:

* [Drive](drive.md). Представляет логический контейнер для файлов, например библиотеку документов или пользовательское хранилище OneDrive.
* [DriveItem](driveitem.md). Представляет элемент на диске, например документ, фотографию, видео или папку.

Большинство операций с файлами выполняется путем взаимодействия с ресурсами **DriveItem**. Ниже представлен пример ресурса DriveItem.

```json
{
  "@content.downloadUrl":"https://public-sn3302.files.1drv.com/y2pcT7OaUEExF7EHOlpTjCE55mIUoiX7H3sx1ff6I-nP35XUTBqZlnkh9FJhWb_pf9sZ7LEpEchvDznIbQig0hWBeidpwFkOqSKCwQylisarN6T0ecAeMvantizBUzM2PA1",
  "createdDateTime": "2016-09-16T03:37:04.72Z",
  "cTag": "aYzpENDY0OEYwNkM5MUQ5RDNEITU0OTI3LjI1Ng",
  "eTag": "aRDQ2NDhGMDZDOTFEOUQzRCE1NDkyNy4w",
  "id":"D4648F06C91D9D3D!54927",
  "lastModifiedBy": {
    "user": {
      "displayName": "Daron Spektor",
      "id": "d4648f06c91d9d3d"
    }
  },
  "name":"BritishShorthair.jpg",
  "size":35212,
  "image":{
    "height":398,
    "width":273
  },
  "file": {
    "hashes":{
      "sha1Hash":"wmgPQ6jrSeMX7JP1XmstQEGM2fc="
    }
  }
}
```

В ресурсах **Drive** и **DriveItem** данные доступны в трех вариантах.

* Как _свойства_ (например, **id** и **name**), которые представляют простые значения (строки, числа, логические значения).
* Как _аспекты_ (например, **file** и **photo**), которые представляют сложные значения. Наличие аспекта **file** или **folder** указывает поведение и свойства ресурса **DriveItem**.
* Как _ссылки_ (например, **children** и **thumbnails**), которые указывают на коллекции других ресурсов.

## <a name="commonly-accessed-resources"></a>Часто используемые ресурсы

В большинстве запросов API для работы с файлами используется один из указанных ниже базовых ресурсов, позволяющих получить доступ к ресурсу **Drive** или **DriveItem**.

| Путь                               | Ресурс
|------------------------------------|-----------------------------------------
| `/me/drive`                        | Хранилище OneDrive пользователя
| `/me/drives`                       | Перечисление ресурсов OneDrive, доступных пользователю.
| `/drives/{drive-id}`               | Доступ к определенному ресурсу **Drive** по идентификатору диска.
| `/drives/{drive-id}/root/children` | Перечисление ресурсов **DriveItem** в корне определенного ресурса **Drive**.
| `/me/drive/items/{item-id}`        | Доступ к ресурсу **DriveItem** в пользовательском хранилище OneDrive по его уникальному идентификатору.
| `/me/drive/special/{special-id}`   | Доступ к специальной (именованной) папке в пользовательском хранилище OneDrive по ее известному имени.
| `/users/{user-id}/drive`           | Доступ к хранилищу OneDrive другого пользователя по уникальному идентификатору этого пользователя.
| `/groups/{group-id}/drive`         | Доступ к стандартной библиотеке документов группы по уникальному идентификатору этой группы.
| `/shares/{share-id}`               | Доступ к ресурсу **DriveItem** по свойству **sharedId** или URL-адресу для совместного доступа.
| `/sites/{site-id}/drive`           | Доступ к ресурсу **Drive** (библиотеке документов) для указанного [сайта][] [SharePoint][].
| `/sites/{site-id}/drives`          | Перечисление ресурсов **drive** (библиотек документов) для [сайта][] [SharePoint][]

Ваше приложение может получать доступ к **DriveItem** в ресурсе **Drive** не только по уникальному идентификатору, но и по относительному пути от известного ресурса. Чтобы путь не был относительным, используйте двоеточие (`:`). В этой таблице представлены примеры различных применений двоеточия для обращения к элементу по пути.

| Path | Ресурс |
|---|---|
| `/me/drive/root:/path/to/file` | Доступ к ресурсу **DriveItem** по относительному пути для корневой папки OneDrive пользователя. |
| `/me/drive/items/{item-id}:/path/to/file` | Доступ к ресурсу **DriveItem** по относительному пути для другого элемента (экземпляра **DriveItem** с аспектом **folder**). |
| `/me/drive/root:/path/to/folder:/children` | Получение списка дочерних экземпляров ресурса **DriveItem** по относительному пути для корневого каталога OneDrive пользователя. |
| `/me/drive/items/{item-id}:/path/to/folder:/children` | Получение списка дочерних экземпляров ресурса **DriveItem** по относительному пути для другого элемента. |

Дополнительные сведения см. в разделе об [адресации driveItems](/graph/concepts/onedrive-addressing-driveitems.md).

## <a name="drive-resource"></a>Ресурс Drive

[Ресурс Drive](drive.md) — это объект верхнего уровня в хранилище OneDrive или библиотеке документов [SharePoint][] пользователя. Почти все операции с файлами начинаются с обращения к определенному ресурсу диска.

К ресурсу диска можно обратиться по уникальному идентификатору диска или с помощью диска по умолчанию для [User](user.md), [Group](group.md) или организации.

## <a name="driveitem-resource"></a>Ресурс DriveItem

Ресурсы [DriveItem](driveitem.md) — это объекты в файловой системе диска. К ним можно обращаться по свойству **id** с использованием синтаксиса `/items/{item-id}` или по пути в файловой системе с использованием синтаксиса `/root:/path/to/item/`.

У ресурсов DriveItem есть _аспекты_, предоставляющие данные об особенностях и возможностях элемента.

Ресурсы DriveItem с аспектом **folder** действуют как контейнеры элементов и содержат ссылку **children**, указывающую на коллекцию элементов в папке.

## <a name="shared-folders-and-remote-items"></a>Общие папки и удаленные элементы

Пользователь, у которого есть личная (не рабочая или учебная) учетная запись OneDrive, может добавить один или несколько общих элементов с другого диска в свое хранилище OneDrive. Эти общие элементы отображаются в коллекции **children** как экземпляры **DriveItem** с аспектом [remoteItem](remoteitem.md).

Дополнительные сведения о работе с общими папками и удаленными элементами см. в [статье, посвященной общим папкам и удаленным элементам](remoteitem.md).

## <a name="sharing-and-permissions"></a>Совместный доступ и разрешения

Одно из самых распространенных действий для OneDrive и библиотек документов SharePoint — предоставление общего доступа к содержимому. С помощью Microsoft Graph ваше приложение может [создавать ссылки для совместного доступа](../api/driveitem-createlink.md), [добавлять разрешения и отправлять приглашения](../api/driveitem-invite.md) для совместного доступа к элементам на диске.

Кроме того, с помощью Microsoft Graph ваше приложение может [получать доступ к общему содержимому](../api/shares-get.md) непосредственно по ссылке для совместного доступа.

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

[SharePoint]: sharepoint.md
[site]: site.md
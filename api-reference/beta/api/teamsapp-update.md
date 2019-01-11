---
title: Permissions
description: 'Обновление приложения ранее опубликованы в каталоге приложений группами Майкрософт. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 125d078b5882e08ff5053acee372d8f352f6a2b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861672"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a>Обновление приложений, опубликованной в каталоге приложений организации

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Обновление [приложения](../resources/teamsapp.md) ранее опубликованы в каталоге приложений группами Майкрософт. Этот интерфейс API специально обновляет приложение, опубликованной в каталоге приложений организации (каталог приложений клиента). Чтобы опубликовать в каталоге приложений организации, укажите `organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

>**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)|
|:----------------------------------     |:-------------|
| Делегированные (рабочая или учебная учетная запись)     | AppCatalog.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается|
| Для приложений                            | Не поддерживается|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение           |
|:--------------|:--------------  |
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type  | приложение/zip |

## <a name="request-body"></a>Тело запроса

Zip полезных команд манифеста: Для приложения группы ZIP-файл, [перейдите в раздел Create пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)

>**Примечание:** Используйте код, возвращенный вызова [списка публикации приложений](./teamsapp-list.md) для ссылок на приложением, которое вы хотите обновить. Не используйте код из манифеста приложения ZIP-архив.

## <a name="response"></a>Ответ

```
HTTP/1.1 204 No Content
```

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Для приложения группы ZIP-файл [видеть создать пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)

### <a name="response"></a>Ответ

```
HTTP/1.1 204 No Content
```

---
title: Разрешения
description: 'Обновление приложения, опубликованного ранее в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2b9a16dc64557776eb6571ba3740249593684ba2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536856"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a>Обновление приложений, опубликованных в каталоге приложений вашей организации

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление [приложения](../resources/teamsapp.md) , опубликованного ранее в каталоге приложений Microsoft Teams. Этот API-интерфейс специально обновляет приложение, опубликованное в каталоге приложений вашей организации (Каталог приложений клиента). Чтобы опубликовать в каталоге приложений вашей организации, укажите `organization` в качестве **distributionMethod** в ресурсе [теамскаталогапп](../resources/teamsapp.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

>**Примечание:** Только глобальные администраторы могут вызывать этот API.

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
| Content-Type  | приложение/ZIP-индекс |

## <a name="request-body"></a>Текст запроса

Полезные данные манифеста ZIP для teams: в ZIP-файле приложения Teams [см. Создание пакета приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)

>**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите обновить. Не используйте идентификатор из манифеста пакета приложения ZIP.

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

Для ZIP-файла приложения Teams [см. Создание пакета приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)

### <a name="response"></a>Отклик

```
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

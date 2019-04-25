---
title: Разрешения
description: 'Опубликуйте приложение в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7acd916aa04200c626d8045e7da5a6d00be8a951
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544561"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a>Публикация приложений в каталоге приложений Организации

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Опубликуйте [приложение](../resources/teamsapp.md) в каталоге приложений Microsoft Teams. В частности, этот API публикует приложение в каталоге организации (Каталог приложений клиента); созданный ресурс будет иметь `distributionMethod`  =  `organization`.

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
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение           |
|:--------------|:--------------  |
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type  | приложение/ZIP-индекс |

## <a name="request-body"></a>Текст запроса

Полезные данные манифеста ZIP Teams. Для ZIP-файла приложения Teams [в разделе Create a App Package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). Вы не можете создать приложение для Организации с таким же ИДЕНТИФИКАТОРом манифеста, что и у другого приложения в этой Организации.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [теамскаталогапп](../resources/teamsapp.md) .

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Сведения о том, как создать ZIP-файл приложения Microsoft Teams, можно найти в разделе [Создание пакета приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). 

### <a name="response"></a>Отклик

```
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

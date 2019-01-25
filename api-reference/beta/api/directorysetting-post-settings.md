---
title: Создайте параметр каталога
description: Используйте этот интерфейс API для создания нового параметра, на основе шаблонов, доступных в directorySettingTemplates. Эти параметры можно на уровне клиента или на уровне объекта (в настоящее время только для групп). Запрос на создание необходимо задать settingValues для всех параметров, определенных в шаблоне. Для определенных параметров может устанавливаться только параметр Управление ли членов группы можно приглашать пользователей гостя. Преимущественную это поведение после общедоступной возможность добавления гостевых пользователей в группу.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f74c449f02726adc4ba0993f450a8a4351ec8f2a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520755"
---
# <a name="create-a-directory-setting"></a>Создайте параметр каталога

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте этот интерфейс API для создания нового параметра, на основе шаблонов, доступных в directorySettingTemplates. Эти параметры можно на уровне клиента или на уровне объекта (в настоящее время только для групп). Запрос на создание необходимо задать settingValues для всех параметров, определенных в шаблоне. Для определенных параметров может устанавливаться только параметр Управление ли членов группы можно приглашать пользователей гостя. Преимущественную это поведение после общедоступной возможность добавления гостевых пользователей в группу.

> **Примечание**: версия /beta этот интерфейс API является только относится к группам. Версия /v1.0 этот интерфейс API переименовано в *Создание groupSettings*.

Список шаблонов и свойств, которые они поддерживают в бета-версии используйте [directorySettingTemplate запроса](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta). (Для конечных точек версии 1.0, вызовите [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление JSON объекта [directorySetting](../resources/directorysetting.md) .  Тем не менее отображаемое имя для параметра задается в соответствии на имя шаблона параметров, который указывает ссылка.

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `201 Created` объект [directorySetting](../resources/directorysetting.md) и кода ответа в теле ответа.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}-->
```http
POST https://graph.microsoft.com/beta/settings
Content-type: application/json
Content-length: 222

{
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
В тексте запроса укажите представление JSON объекта [directorySetting](../resources/directorysetting.md) .
##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
    "@odata.context": "https://graph.microsoft.com/stagingbeta/$metadata#settings/$entity",
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-post-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: Создание параметра группы
description: Этот API позволяет создавать новые параметры на базе шаблонов, доступных в объектах groupSettingTemplate. Эти параметры можно использовать как на уровне клиента, так и на уровне группы. Запрос на создание должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне. Специально для групп можно задавать только параметр, разрешающий или запрещающий членам группы приглашать пользователей-гостей. Возможность добавлять пользователей-гостей в группу общедоступна, поэтому данный параметр позволит контролировать подобное поведение.
localization_priority: Normal
ms.openlocfilehash: c5ba428380e6503f8d54682709d36e12b7ff4de3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894539"
---
# <a name="create-a-group-setting"></a>Создание параметра группы

Этот API позволяет создавать новые параметры на базе шаблонов, доступных в объектах [groupSettingTemplate](../resources/groupsettingtemplate.md). Эти параметры можно использовать как на уровне клиента, так и на уровне группы. Запрос на создание должен предоставлять объекты [settingValue](../resources/settingvalue.md) для всех параметров, определенных в шаблоне. Специально для групп можно задавать только параметр, разрешающий или запрещающий членам группы приглашать пользователей-гостей. Возможность добавлять пользователей-гостей в группу общедоступна, поэтому данный параметр позволит контролировать подобное поведение.

Список шаблонов и свойств, которые они поддерживают в версии 1.0 используйте [groupSettingTemplate запроса](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0) (для бета-версии конечных точек, вызов [directorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)

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
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---------------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type | application/json |

## <a name="request-body"></a>Тело запроса
В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON. Отображаемое имя для параметра будет задано с учетом имени указанного шаблона параметров.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [groupSetting](../resources/groupsetting.md) в теле отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
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
В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON.
##### <a name="response"></a>Отклик

Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 238

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

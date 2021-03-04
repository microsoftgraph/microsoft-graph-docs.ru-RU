---
title: Создание параметра каталога
description: Используйте этот API для создания нового параметра на основе шаблонов, доступных в directorySettingTemplates.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a4dec36d0932870b7d8601223b71aa4340175c47
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436641"
---
# <a name="create-a-directory-setting"></a>Создание параметра каталога

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте этот API для создания нового параметра на основе шаблонов, доступных в directorySettingTemplates. Эти параметры могут быть на уровне клиента или на уровне объекта (в настоящее время только для групп). Запрос на создание должен предоставить параметрValues для всех параметров, определенных в шаблоне. Для параметров, определенных для группы, можно установить только параметр, регуляющий, могут ли члены группы приглашать гостевых пользователей. Это будет регулировать такое поведение после того, как будет доступна возможность добавлять гостевых пользователей в группу.

> **Примечание.** Бета-версия этого API применяется только к группам. Версия /v1.0 этого API переименована в *Create groupSettings.*

Для списка шаблонов и свойств, которые они поддерживают в бета-версии, используйте [запрос directorySettingTemplate](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta). (Для конечных точек v1.0 вызываемая [группаSettingTemplates.)](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Directory.ReadWrite.All |

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

## <a name="request-body"></a>Тело запроса
В теле запроса поставляем представление JSON объекта [directorySetting.](../resources/directorysetting.md)  Однако имя отображения для параметра будет устанавливаться на основе имени шаблона ссылок параметров.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект directorySetting](../resources/directorysetting.md) в тексте ответа.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directorysetting-from-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directorysetting-from-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

В теле запроса поставляем представление JSON объекта [directorySetting.](../resources/directorysetting.md)
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
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
  ]
}
-->



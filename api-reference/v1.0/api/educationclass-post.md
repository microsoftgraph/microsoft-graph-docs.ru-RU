---
title: Создание educationClass
description: Создание нового объекта educationClass.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: db8cedc35b48478edd58a9beb2e29d742c4b5cb2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147439"
---
# <a name="create-educationclass"></a>Создание educationClass

Пространство имен: microsoft.graph

Создание нового [объекта educationClass.](../resources/educationclass.md)

> [!NOTE]
> При этом будет также создана универсальная группа. При использовании этого API для создания класса в группу будут добавлены специальные свойства, которые будут добавлять такие функции, как назначения и специальная обработка в Microsoft Teams при создании групп с помощью группы. Обратите внимание, что этот API создает только универсальную группу и не создает команду. Microsoft Teams предоставляет пользовательский интерфейс для преподавателей для создания групп для своих классов с помощью групп, созданных этим API.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается.                              |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | EduRoster.ReadWrite.All                     |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/classes
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [educationClass.](../resources/educationclass.md)

В следующей таблице показаны свойства, необходимые при создании [educationClass.](../resources/educationclass.md)

| Свойство             | Тип                                           | Описание                                                        |
| :------------------- | :--------------------------------------------- | :----------------------------------------------------------------- |
| id                   | String                                         | Идентификатор объекта. Унаследованный от [сущности](../resources/entity.md) |
| displayName          | String                                         | Название курса.                                                 |
| mailNickname         | String                                         | Почтовое имя для отправки почты всем участникам, если это возможно.    |
| description          | String                                         | Описание курса.                                          |
| createdBy            | [identitySet](../resources/identityset.md)     | Объект, который создал курс.                                       |
| classCode            | String                                         | Код курса, используемый учебным заведением для идентификации курса.               |
| externalName         | String                                         | Название курса в системе синхронизации.                           |
| externalId           | String                                         | Идентификатор курса из системы синхронизации.                           |
| externalSource       | educationExternalSource                        | Способ создания этого курса. Возможные значения: `sis` , `manual`   |
| externalSourceDetail | String                                         | Имя внешнего источника, из которого были созданы эти ресурсы. |
| оценка                | String                                         | Уровень класса.                                          |
| term                 | [educationTerm](../resources/educationterm.md) | Срок для этого курса.                                               |

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationClass](../resources/educationclass.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/classes
Content-Type: application/json
Content-length: 533

{
  "@odata.type": "#microsoft.graph.educationClass",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```

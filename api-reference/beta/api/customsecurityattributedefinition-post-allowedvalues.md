---
title: Создание allowedValue
description: Создайте новый объект allowedValue.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a647525b112059c271a74cd691a2eaec4db6e724
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077720"
---
# <a name="create-allowedvalue"></a>Создание allowedValue
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект allowedValue.](../resources/allowedvalue.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CustomSecAttributeDefinition.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|CustomSecAttributeDefinition.ReadWrite.All|

Пользователю, заявиму, также должна быть назначена роль администратора [определения атрибутов.](/azure/active-directory/roles/permissions-reference) По умолчанию глобальные роли администратора и других администраторов не имеют разрешений на чтение, определение или назначение настраиваемого атрибута безопасности.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}/allowedValues
```


## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [allowedValue.](../resources/allowedvalue.md)

В следующей таблице показаны свойства, необходимые при создании [allowedValue.](../resources/allowedvalue.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор для предопределяемой величины. Может иметь длину до 64 символов и включать символы Unicode. Может включать пробелы, но некоторые специальные символы не допускаются. Не удается изменить позже. Деликатный. Обязательный.|
|isActive|Логическое|Указывает, активна ли заранее заранее активная или деактивированная величина. Если установлено значение, это предварительное значение не может быть назначено дополнительным поддерживаемым `false` объектам каталога. Обязательный.|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект allowedValue](../resources/allowedvalue.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-add-a-predefined-value"></a>Пример: Добавление предопределяемой величины

В следующем примере в настраиваемом определении атрибута безопасности добавляется предопределенный параметр.

+ Набор атрибутов: `Engineering`
+ Атрибут: `Project`
+ Предопределяемая величина: `Alpine`

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_allowedvalue"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_Project/allowedValues
Content-Type: application/json

{
    "id":"Alpine",
    "isActive":"true"
}
```


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.allowedValue"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/customSecurityAttributeDefinitions('Engineering_Project')/allowedValues/$entity",
    "id": "Alpine",
    "isActive": true
}
```

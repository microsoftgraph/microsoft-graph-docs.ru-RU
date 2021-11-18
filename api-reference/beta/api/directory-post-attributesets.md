---
title: Создание attributeSet
description: Создайте новый объект attributeSet.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4143ae0ccd8fa6fa9f0a9b682e78c20d0baa08d1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077567"
---
# <a name="create-attributeset"></a>Создание attributeSet
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект attributeSet.](../resources/attributeset.md)

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
POST /directory/attributeSets
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [attributeSet.](../resources/attributeset.md)

В следующей таблице показаны свойства, которые можно настроить при создании [attributeSet.](../resources/attributeset.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Описание набора атрибутов. Может иметь длину до 128 символов и включать символы Unicode. Можно изменить позже. Необязательный параметр.|
|id|String|Идентификатор для уникального набора атрибутов в клиенте. Может иметь длину до 32 символов и включать символы Unicode. Не может содержать пробелы или специальные символы. Не удается изменить позже. Случай нечувствительный. Обязательный.|
|maxAttributesPerSet|Int32|Максимальное количество пользовательских атрибутов безопасности, которые можно определить в этом наборе атрибутов. Значение по умолчанию — `null`. Если не указано, администратор может добавить не более 500 активных атрибутов на каждого клиента. Можно изменить позже. Необязательный параметр.|


## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект attributeSet](../resources/attributeset.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-add-an-attribute-set"></a>Пример: Добавление набора атрибутов

В следующем примере добавляется новый набор атрибутов с именем `Engineering` .

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_attributeset"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/attributeSets
Content-Type: application/json

{
    "id":"Engineering",
    "description":"Attributes for engineering team",
    "maxAttributesPerSet":25
}
```


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attributeSet"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/attributeSets/$entity",
    "description": "Attributes for engineering team",
    "id": "Engineering",
    "maxAttributesPerSet": 25
}
```

---
title: тип ресурса fido2AuthenticationMethod
description: Представление ключа безопасности FIDO2, зарегистрированного для пользователя. FIDO2 — это метод проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0c79a704d9a2aa899ffc2a3f4592f76a30d30126
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964965"
---
# <a name="fido2authenticationmethod-resource-type"></a>тип ресурса fido2AuthenticationMethod

Пространство имен: microsoft.graph

Представление ключа безопасности FIDO2, зарегистрированного для пользователя. FIDO2 — это метод проверки подлинности.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список](../api/fido2authenticationmethod-list.md)|[коллекция fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Извлечение списка объектов fido2AuthenticationMethod пользователя и их свойств.|
|[получение](../api/fido2authenticationmethod-get.md);|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Ознакомьтесь с свойствами и отношениями объекта fido2AuthenticationMethod пользователя.|
|[удаление](../api/fido2authenticationmethod-delete.md);|Нет|Удаляет объект fido2AuthenticationMethod пользователя.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор метода проверки подлинности.|
|displayName|String|Отображает имя ключа, заданное пользователем.|
|createdDateTime|DateTimeOffset|Время регистрации этого ключа пользователю.|
|aaGuid|String|GUID проверки подлинности, идентификатор, который указывает тип (например, make и model) аутентиста.|
|model|String|Назначенная производителем модель ключа безопасности FIDO2.|
|attestationCertificates|Коллекция строк|Сертификат аттестации(ы), присоединенный к этому ключу безопасности.|
|attestationLevel|attestationLevel|Уровень проверки этого ключа безопасности FIDO2. Возможные значения: `attested` или `notAttested` .|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fido2AuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)",
  "aaGuid": "String",
  "model": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String"
}
```


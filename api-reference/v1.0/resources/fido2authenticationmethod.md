---
title: тип ресурса fido2AuthenticationMethod
description: Представление ключа безопасности FIDO2, зарегистрированного для пользователя. FIDO2 — это метод проверки подлинности.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8af931dba72daba05c8c548cc53d130d6f3f182b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062721"
---
# <a name="fido2authenticationmethod-resource-type"></a>тип ресурса fido2AuthenticationMethod

Пространство имен: microsoft.graph

Представление ключа безопасности FIDO2, зарегистрированного для пользователя. FIDO2 — это метод проверки подлинности.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление](../api/fido2authenticationmethod-list.md)|[коллекция fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Извлечение списка объектов fido2AuthenticationMethod пользователя и их свойств.|
|[получение](../api/fido2authenticationmethod-get.md);|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Ознакомьтесь с свойствами и отношениями объекта fido2AuthenticationMethod пользователя.|
|[удаление](../api/fido2authenticationmethod-delete.md);|Нет|Удаляет объект fido2AuthenticationMethod пользователя.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор метода проверки подлинности.|
|displayName|Строка|Отображает имя ключа, заданное пользователем.|
|createdDateTime|DateTimeOffset|Время регистрации этого ключа пользователю.|
|aaGuid|Строка|Authenticator GuID-идентификатор attestation, который указывает тип (например, make и model) аутентиста.|
|model|String|Назначенная производителем модель ключа безопасности FIDO2.|
|attestationCertificates|Коллекция String|Сертификат аттестации(ы), присоединенный к этому ключу безопасности.|
|attestationLevel|attestationLevel|Уровень проверки этого ключа безопасности FIDO2. Возможные значения: `attested` или `notAttested` .|


## <a name="relationships"></a>Отношения
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
  "createdDateTime": "String (timestamp)",
  "aaGuid": "String",
  "model": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String"
}
```


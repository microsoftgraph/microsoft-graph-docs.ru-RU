---
title: Тип ресурса fido2AuthenticationMethod
description: Представление ключа безопасности FIDO2, зарегистрированного для пользователя. FIDO2 — метод проверки подлинности при входе.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c4d10252201781d1339e6baa26aea248429ae462
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418435"
---
# <a name="fido2authenticationmethod-resource-type"></a>Тип ресурса fido2AuthenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление ключа безопасности FIDO2, зарегистрированного для пользователя. FIDO2 — метод проверки подлинности при входе.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление](../api/fido2authenticationmethod-list.md)|Коллекция [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Получение списка объектов fido2AuthenticationMethod пользователя и их свойств.|
|[Получение](../api/fido2authenticationmethod-get.md)|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Чтение свойств и связей объекта fido2AuthenticationMethod пользователя.|
|[Удаление](../api/fido2authenticationmethod-delete.md)|Нет|Удаляет объект fido2AuthenticationMethod пользователя.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор метода проверки подлинности.|
|displayName|String|Отображаемое имя ключа, заданное пользователем.|
|креатиондатетиме|DateTimeOffset|Временная метка, когда этот ключ был зарегистрирован для пользователя.|
|аагуид|String|GUID аттестации для проверки подлинности, идентификатор, указывающий тип (например, создание и модель) средства проверки подлинности.|
|model|String|Модель ключа безопасности FIDO2, назначенная производителем.|
|аттестатионцертификатес|Коллекция String|Сертификаты аттестации, вложенные в этот ключ безопасности.|
|аттестатионлевел|аттестатионлевел|Уровень аттестации этого ключа безопасности FIDO2. Возможные значения: `attested` , или `notAttested` .|


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


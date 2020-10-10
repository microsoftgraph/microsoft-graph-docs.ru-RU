---
title: Тип ресурса fido2AuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности FIDO2
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 62aa22fa22b70235f5221bc820cee5178b55b51b
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418431"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a>Тип ресурса fido2AuthenticationMethodConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику методов проверки подлинности FIDO2. Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или группы, для которых разрешено использование метода проверки подлинности.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение](../api/fido2authenticationmethodconfiguration-get.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|Чтение свойств и связей объекта fido2AuthenticationMethodConfiguration.|
|[Обновление](../api/fido2authenticationmethodconfiguration-update.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|Обновление свойств объекта fido2AuthenticationMethodConfiguration.|
|[Удаление](../api/fido2authenticationmethodconfiguration-delete.md)|Нет|Возвращает объект fido2AuthenticationMethodConfiguration в конфигурацию по умолчанию.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности.|
|исаттестатионенфорцед|Boolean|Определяет, следует ли применять аттестацию для регистрации ключа безопасности FIDO2.|
|исселфсервицерегистратионалловед|Boolean|Определяет, могут ли пользователи регистрировать новые ключи безопасности FIDO2.|
|кэйрестриктионс|[fido2KeyRestrictions](../resources/fido2keyrestrictions.md)|Определяет, применяются ли ограничения ключей к ключам безопасности FIDO2, разрешать или запрещать определенные типы ключей, как определено идентификатором GUID аттестации (ААГУИД), идентификатором, указывающим тип (например, make and model) средства проверки подлинности.|
|state|аусентикатионмесодстате|Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|инклудетаржетс|Коллекция [аусентикатионмесодтаржет](../resources/authenticationmethodtarget.md)|Коллекция пользователей или групп, которым разрешено использовать метод проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "isSelfServiceRegistrationAllowed": "Boolean",
  "isAttestationEnforced": "Boolean",
  "keyRestrictions": {
    "@odata.type": "microsoft.graph.fido2KeyRestrictions"
  },
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```

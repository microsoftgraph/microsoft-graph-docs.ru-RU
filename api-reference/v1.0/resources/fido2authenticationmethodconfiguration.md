---
title: тип ресурса fido2AuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности FIDO2
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3be6525cc09b2932541efa722e1cc140d42739a0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062700"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a>тип ресурса fido2AuthenticationMethodConfiguration

Пространство имен: microsoft.graph

Представляет политику методов проверки подлинности FIDO2. Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или групп, которым включен метод проверки подлинности.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[получение](../api/fido2authenticationmethodconfiguration-get.md);|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|Ознакомьтесь с свойствами и отношениями объекта fido2AuthenticationMethodConfiguration.|
|[Обновление](../api/fido2authenticationmethodconfiguration-update.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|Обновление свойств объекта fido2AuthenticationMethodConfiguration.|
|[удаление](../api/fido2authenticationmethodconfiguration-delete.md);|Нет|Возвращает объект fido2AuthenticationMethodConfiguration к конфигурации по умолчанию.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор политики метода проверки подлинности.|
|isAttestationEnforced|Логический|Определяет, необходимо ли применять проверку для регистрации ключей безопасности FIDO2.|
|isSelfServiceRegistrationAllowed|Boolean|Определяет, могут ли пользователи зарегистрировать новые ключи безопасности FIDO2.|
|keyRestrictions|[fido2KeyRestrictions](../resources/fido2keyrestrictions.md)|Контролирует, применяются ли ключевые ограничения для ключей безопасности FIDO2, разрешая или отменяя определенные типы ключей в зависимости от Authenticator Attestation GUID (AAGUID), идентификатора, который указывает тип (например, make и model) аутентиста.|
|state|authenticationMethodState|Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|includeTargets|[коллекция authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.|

## <a name="json-representation"></a>Представление в формате JSON
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

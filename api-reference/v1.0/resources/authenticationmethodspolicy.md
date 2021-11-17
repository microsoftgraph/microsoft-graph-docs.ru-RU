---
title: тип ресурса authenticationMethodsPolicy
description: Определяет методы проверки подлинности и пользователей, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA).
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 036f4dce3d3192005a9b99124965830a5b38194a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015806"
---
# <a name="authenticationmethodspolicy-resource-type"></a>тип ресурса authenticationMethodsPolicy

Пространство имен: microsoft.graph

Определяет методы проверки подлинности и пользователей, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получить проверку подлинностиMethodsPolicy](../api/authenticationmethodspolicy-get.md)|[authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md)|Ознакомьтесь с свойствами и отношениями объекта [authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)|
|[Обновление проверки подлинностиMethodsPolicy](../api/authenticationmethodspolicy-update.md)|[authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md)|Обновление свойств объекта [authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Описание политики. Только для чтения.|
|displayName|Строка|Имя политики. Только для чтения.|
|id|Строка|Идентификатор политики. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего обновления политики. Только для чтения.|
|policyVersion|String|Версия используемой политики. Только для чтения.|
|registrationEnforcement|[registrationEnforcement](../resources/registrationenforcement.md)|Принудительное выполнение регистрации во время регистрации. Это свойство можно использовать для напоминания пользователям о том, как настроить целевые методы проверки подлинности.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|authenticationMethodConfigurations|[коллекция authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)|Представляет параметры для каждого метода проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "policyVersion": "String",
  "registrationEnforcement": {
    "@odata.type": "microsoft.graph.registrationEnforcement"
  } 
}
```

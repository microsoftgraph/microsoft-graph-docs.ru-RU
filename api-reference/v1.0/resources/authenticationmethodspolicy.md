---
title: тип ресурса authenticationMethodsPolicy
description: Определяет методы проверки подлинности и пользователей, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA).
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cea7a72bce9a87d199b71d7e5c91d8f91f9c8e51
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2022
ms.locfileid: "62239101"
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
|id|String|Идентификатор политики. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего обновления политики. Только для чтения.|
|policyVersion|Строка|Версия используемой политики. Только для чтения.|
|registrationEnforcement|[registrationEnforcement](../resources/registrationenforcement.md)|Принудительное выполнение регистрации во время регистрации. Это свойство можно использовать для напоминания пользователям о том, как настроить целевые методы проверки подлинности.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|authenticationMethodConfigurations|[коллекция authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)|Представляет параметры для каждого метода проверки подлинности. Автоматически расширяется в `GET /policies/authenticationMethodsPolicy`.|

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

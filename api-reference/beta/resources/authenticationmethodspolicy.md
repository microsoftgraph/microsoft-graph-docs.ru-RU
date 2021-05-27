---
title: тип ресурса authenticationMethodsPolicy
description: Определяет методы проверки подлинности и пользователей, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA).
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: fdf86929b4098d9fb62f1426883b55d95c669f32
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682936"
---
# <a name="authenticationmethodspolicy-resource-type"></a>тип ресурса authenticationMethodsPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет методы проверки подлинности и пользователей, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получить проверку подлинностиMethodsPolicy](../api/authenticationmethodspolicy-get.md)|[authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md)|Ознакомьтесь с свойствами и отношениями объекта [authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)|
|[Обновление проверки подлинностиMethodsPolicy](../api/authenticationmethodspolicy-update.md)|[authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md)|Обновление свойств объекта [authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание политики.|
|displayName|String|Имя политики.|
|id|String|Идентификатор политики. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего обновления политики.|
|policyVersion|String|Версия используемой политики.|
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

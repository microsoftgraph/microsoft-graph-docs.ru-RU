---
title: тип ресурса authenticationMethodsPolicy
description: Определяет методы проверки подлинности и пользователей, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA).
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9abab0af31a67465db9989b42186759b12f746bb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126963"
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
|displayName|String|Имя политики. Только для чтения.|
|id|String|Идентификатор политики. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего обновления политики. Только для чтения.|
|policyVersion|Строка|Версия используемой политики. Только для чтения.|

## <a name="relationships"></a>Отношения
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
}
```

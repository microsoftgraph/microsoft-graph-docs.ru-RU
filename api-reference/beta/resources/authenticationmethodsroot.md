---
title: тип ресурса authenticationMethodsRoot
description: Контейнер для свойств навигации для ресурсов методов проверки подлинности Azure AD.
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: def78eddd43cdb7ea738d32e25c8d90adb23fbc4
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201689"
---
# <a name="authenticationmethodsroot-resource-type"></a>тип ресурса authenticationMethodsRoot

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для свойств навигации для ресурсов методов проверки подлинности Azure AD.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String| Уникальный идентификатор. Наследуется от [сущности](../resources/entity.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|userRegistrationDetails|[userRegistrationDetails](../resources/userRegistrationDetails.md)| Представляет состояние методов проверки подлинности пользователя, в том числе зарегистрированных методов и функций, на которые зарегистрирован и способен пользователь (например, многофакторная проверка подлинности, сброс пароля самообслуживления и проверка подлинности без паролей).|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodsRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRoot",
  "id": "String (identifier)"
}
```
---
title: Тип ресурса authenticationMethodsRoot
description: Контейнер для свойств навигации для Azure AD методов проверки подлинности.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: cc86e2ff67f7c628406aa90aca5bd00d03101272
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820485"
---
# <a name="authenticationmethodsroot-resource-type"></a>Тип ресурса authenticationMethodsRoot

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для свойств навигации для Azure AD методов проверки подлинности.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка| Уникальный идентификатор. Наследуется от [сущности](../resources/entity.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|userRegistrationDetails|[userRegistrationDetails](../resources/userRegistrationDetails.md)| Представляет состояние методов проверки подлинности пользователя, включая, какие методы зарегистрированы и какие функции зарегистрированы и поддерживаются пользователем (например, многофакторная проверка подлинности, самостоятельный сброс пароля и проверка подлинности без пароля).|

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
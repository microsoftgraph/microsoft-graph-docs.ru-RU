---
title: тип ресурса passwordCredentialConfiguration
description: Сложный тип конфигурации учетных данных паролей для настройки ограничения учетных данных пароля, maxLifetime и даты принудения
author: madansr7
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8a67dfd1bf6ee717f279cb27bf08f819daba1645
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660461"
---
# <a name="passwordcredentialconfiguration-resource-type"></a>тип ресурса passwordCredentialConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект конфигурации учетных данных паролей, содержащий свойства для настройки ограничений, таких как блокировка или ограничение срока служб секретов паролей.

## <a name="properties"></a>Свойства

| Свойство                            | Тип                                                                               | Описание                                                                                                                                                                                                                                                                                   |
| :---------------------------------- | :--------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| restrictionType                     | appCredentialRestrictionType | Тип применяемого ограничения. Возможные значения: `passwordAddition` или `passwordLifetime`. Каждое значение restrictionType можно использовать только один раз в политику.                                                                                                                        |
| maxLifeTime                         | Длительность                                                                           | Значение, которое можно использовать в качестве максимального числа для установки срока действия пароля в днях, часах, минутах или секундах. Например, "P4DT12H30M5S" представляет собой продолжительность четырех дней, двенадцать часов, тридцать минут и пять секунд. Это свойство необходимо, если установлен тип ограничения `passwordLifetime` . |
| restrictForAppsCreatedAfterDateTime | DateTimeOffset                                                                     | Применяет политику для приложения, созданного в течение или после даты применения. Для существующих приложений дата применения будет датирована. Чтобы применяться к всем приложениям, дата принудения будет null.                                                                               |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.passwordCredentialConfiguration"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.passwordCredentialConfiguration",
  "restrictionType": {
    "@odata.type": "microsoft.graph.appCredentialRestrictionType"
  },
  "maxLifetime": "String (duration)",
  "restrictForAppsCreatedAfterDateTime": "DateTimeOffset"
}
```

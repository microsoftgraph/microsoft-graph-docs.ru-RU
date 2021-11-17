---
title: тип ресурса passwordCredentialConfiguration
description: Сложный тип конфигурации учетных данных паролей для настройки ограничения учетных данных пароля, maxLifetime и даты принудения
author: madansr7
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5f62d6bf87453a99b11c6888edc5feadb52456f4
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044654"
---
# <a name="passwordcredentialconfiguration-resource-type"></a>тип ресурса passwordCredentialConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект конфигурации учетных данных паролей, содержащий свойства для настройки ограничений, таких как блокировка или ограничение срока служб секретов паролей.

## <a name="properties"></a>Свойства

| Свойство                            | Тип                                                                               | Описание                                                                                                                                                                                                                                                                                   |
| :---------------------------------- | :--------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| restrictionType                     | appCredentialRestrictionType |  Тип применяемого ограничения. Допустимые значения: `passwordAddition`, `passwordLifetime`, `symmetricKeyAddition`, `symmetricKeyLifetime`, `unknownFutureValue`. Каждое значение restrictionType можно использовать только один раз в политику. |
| maxLifeTime                         | Длительность                                                                           | Значение, которое можно использовать в качестве максимального числа для установки срока действия пароля в днях, часах, минутах или секундах. Определено в формате ISO 8601 для Durations. Например, "P4DT12H30M5S" представляет собой продолжительность четырех дней, двенадцать часов, тридцать минут и пять секунд. Это свойство необходимо, если установлен тип ограничения `passwordLifetime` . |
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

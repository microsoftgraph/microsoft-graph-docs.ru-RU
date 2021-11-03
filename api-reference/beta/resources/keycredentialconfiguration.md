---
title: тип ресурса keyCredentialConfiguration
description: Сложный тип конфигурации учетных данных для настройки ограничения ключевых учетных данных, maxLifetime и даты принудения
ms.localizationpriority: medium
author: madansr7
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: dbc208ec616f0b865cd848acdf932b045d215bf1
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688292"
---
# <a name="keycredentialconfiguration-resource-type"></a>тип ресурса keyCredentialConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект конфигурации учетных данных, содержащий свойства для настройки ограничений, таких как ограничение срока службы секретов ключей.

## <a name="properties"></a>Свойства

| Свойство                            | Тип                                                                               | Описание                                                                                                                                                                                                                                                                                   |
| :---------------------------------- | :--------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| restrictionType                     | appKeyCredentialRestrictionType | Тип применяемого ограничения. Возможные значения `asymmetricKeyLifetime` : `unknownFutureValue` . Каждое значение restrictionType можно использовать только один раз в политику.                                                                                                                        |
| maxLifeTime                         | Длительность                                                                           |Значение, которое может использоваться в качестве максимальной продолжительности в днях, часах, минутах или секундах от даты создания ключа, для которой ключ действителен. Например, `P4DT12H30M5S` продолжительность 4 дня, 12 часов, 30 минут и 5 секунд. Это свойство необходимо, когда **установлено ограничениеType.** `keyLifetime` |
| restrictForAppsCreatedAfterDateTime | DateTimeOffset                                                                     | Timestamp, когда политика будет применяться для всех приложений, созданных в указанной дате или после нее. Для существующих приложений дата применения будет датирована. Чтобы применяться к всем приложениям независимо от даты их создания, это свойство будет `null` . Допускается значение null. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyCredentialConfiguration"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.keyCredentialConfiguration",
  "restrictionType": {
    "@odata.type": "microsoft.graph.appKeyCredentialRestrictionType"
  },
  "maxLifetime": "String (duration)",
  "restrictForAppsCreatedAfterDateTime": "DateTimeOffset"
}
```

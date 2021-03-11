---
title: тип ресурса hybridAgentUpdaterConfiguration
description: тип ресурса hybridAgentUpdaterConfiguration.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c81d48053e7fb26eaee678da4e4b33708717e3c1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722402"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a>тип ресурса hybridAgentUpdaterConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Администратор клиента может настроить для каждого onPremisesPublishingProfile время, в течение которого агенты могут получать обновления или откладывать обновления агентам. ГибридAgentUpdaterConfiguration, заданный для onPremisesPublishingProfile, применим ко всем агентам в этом onPremisesPublishingProfile.

Например, для агентов в onPremisesPublishingProfile типа "подготовка" шаги могут быть как ниже.

1) Администратор клиента может настроить, чтобы не получать какие-либо обновления для агентов предварительного обеспечения в течение следующих n дней.
2) Администратор клиента может настроить окно обновления (время начала и окончания), в течение которого агенты могут отыскировать обновления.
3) Администратор клиента может включить allowUpdateConfigurationOverride, переопределяющий configutration updater для агентов provisioning и alows, чтобы получить следующее доступное обновление.

Сведения DateTime/Time, указанные в конфигурации обновления, будут преобразованы в локальный часовой пояс, о чем агент сообщает во время evaluvation.

Обновление агента будет выполняться в приведенном ниже списке приоритетов

1) Если установлено значение allowUpdateConfigurationOverride, конфигурация обновления, заданная клиентом, будет пропущена, а агент получит обновление при наличии следующей версии агента (приоритет 1).
2) Если задается обновление отсрочки, агент не будет обновляться до времени отсрочки обновления (приоритет 2).
3) Если установлено окно обновления, агент будет обновляться только в течение этого 24-часового дня (приоритет 3).
4) Если клиент не задает допустимую конфигурацию обновления, агент получит обновление при наличии следующей версии агента.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|allowUpdateConfigurationOverride|Boolean|Указывает, будет ли пропущена конфигурация обновления, и агент получит обновление, когда будет доступна следующая версия агента.|
|deferUpdateDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|updateWindow|[updateWindow](updatewindow.md)||

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
  "baseType": null
}-->

```json
{
  "allowUpdateConfigurationOverride": true,
  "deferUpdateDateTime": "String (timestamp)",
  "updateWindow": {"@odata.type": "microsoft.graph.updateWindow"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hybridAgentUpdaterConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



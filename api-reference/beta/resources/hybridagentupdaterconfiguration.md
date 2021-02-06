---
title: Тип ресурса hybridAgentUpdaterConfiguration
description: Тип ресурса hybridAgentUpdaterConfiguration.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 39b378397b18337c660e76b815a80c9db398f950
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128605"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a>Тип ресурса hybridAgentUpdaterConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Администратор клиента может настроить для каждого onPremisesPublishingProfile период времени, в течение которого агенты могут получать обновления или откладывать обновления для агентов. Гибридная системаAgentUpdaterConfiguration, указанная для onPremisesPublishingProfile, применима ко всем агентам в этом onPremisesPublishingProfile.

Например, для агентов в onPremisesPublishingProfile типа "подготовка" шаги могут быть, как пошаговом примере ниже.

1) Администратор клиента может настроить не получать обновления агентов предоставления в течение следующих n дней.
2) Администратор клиента может настроить окно обновления (время начала и окончания), в течение которого агенты могут пересылать обновления.
3) Администратор клиента может включить allowUpdateConfigurationOverride, который переопределит конфигурирование средства обновления для агентов предоставления и отобразит для них получение следующего доступного обновления.

Сведения о времени и времени, указанные в конфигурации средства обновления, будут преобразованы в локальный часовой пояс, сообщаемой агентом во время evaluvation.

Обновление агента будет выполняться в списке приоритетов ниже

1) Если для allowUpdateConfigurationOverride установлено значение true, конфигурация обновления, установленная клиентом, будет пропущена, и агент получит обновление при наличии следующей версии агента (приоритет 1).
2) Если задается отсрочка обновления, агент не будет обновлен до даты отсрочки обновления (приоритет 2).
3) Если установлено окно обновления, агент будет обновлен только в течение этого 24-часового дня (приоритет 3).
4) Если клиент не настроит допустимую конфигурацию средства обновления, агент получит обновление при наличии следующей версии агента.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|allowUpdateConfigurationOverride|Boolean|Указывает, будет ли пропущена конфигурация обновления, и агент получит обновление при наличии следующей версии агента.|
|deferUpdateDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|updateWindow|[updateWindow](updatewindow.md)||

## <a name="json-representation"></a>Представление в формате JSON

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



---
title: Тип ресурса securityAction
description: Принимайте незамедлительные действия по защите от угроз с помощью объекта securityAction Microsoft Graph Security. Если аналитик безопасности обнаруживает новый индикатор, например вредоносный файл, URL-адрес, домен или IP-адрес, можно сразу же включить защиту в решении по обеспечению безопасности от корпорации Майкрософт. Вызывайте действие для определенного поставщика услуг, просматривайте все выполненные действия и отменяйте действие при необходимости. Воспользуйтесь действиями по обеспечению безопасности с помощью ATP в Защитнике Windows (ожидается в ближайшее время), чтобы заблокировать вредоносную активность в конечных точках Windows с использованием свойств, отображаемых в оповещениях или выявленных при изучении.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 5aa99119f23baa4cd9450d48ee4955d7ce91f60d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583685"
---
# <a name="securityaction-resource-type"></a>Тип ресурса securityAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Принимайте незамедлительные действия по защите от угроз с помощью объекта securityAction Microsoft Graph Security. Если аналитик безопасности обнаруживает новый индикатор, например вредоносный файл, URL-адрес, домен или IP-адрес, можно сразу же включить защиту в решении по обеспечению безопасности от корпорации Майкрософт. Вызывайте действие для определенного поставщика услуг, просматривайте все выполненные действия и отменяйте действие при необходимости. Выполните действия по обеспечению безопасности с помощью [защитника Windows ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) , чтобы заблокировать вредоносные действия в конечных точках Windows, используя свойства, проявляющиеся в оповещениях или определенных во время расследования

  > **Примечание:** В настоящее время действия безопасности поддерживают только разрешения приложения.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение действия по обеспечению безопасности](../api/securityaction-get.md) | [securityAction](securityaction.md) | Чтение свойств и связей объекта securityAction. |
| [Создание действия по обеспечению безопасности](../api/securityactions-post.md) | [securityAction](securityaction.md) | Создание нового securityAction путем отправки в коллекцию Секуритяктионс. |
| [Перечисление действий по обеспечению безопасности](../api/securityactions-list.md) | Коллекция [securityAction](securityaction.md) | Получение коллекции объектов securityAction. |
|[Отмена действия по обеспечению безопасности](../api/securityaction-cancelsecurityaction.md)|Нет|Отмена операции безопасности.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|Актионреасон|String|Причина для вызова этого действия.|
|appId|String|Идентификатор приложения, который передал действие (POST). AppId необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.|
|Азуретенантид|String|Идентификатор клиента Azure объекта, который определяет, к какому клиенту относится данная сущность (поддержка с поддержкой нескольких клиентов). Азуретенантид необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.|
|completedDateTime|DateTimeOffset|Временная метка выполнения действия. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|createdDateTime|DateTimeOffset|Временная метка при создании действия. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|errorInfo|[resultInfo](resultinfo.md)| Сведения об ошибке при сбое действия.|
|id|Строка| Создается системой при выполнении действия. Созданный GUID/уникальный идентификатор. Только для чтения.|
|Ластактиондатетиме|DateTimeOffset| Временная метка при последнем обновлении этого действия. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|name|String| Имя действия.|
|parameters|Коллекция [keyValuePair](keyvaluepair.md)| Коллекция параметров (пар "ключ-значение"), необходимых для вызова действия, например URL-адрес или fileHash для блокировки и т. д.). **Required**|
|состояния|Коллекция [секуритяктионстате](securityactionstate.md)|Коллекция Секуритяктионстате, в которой будет храниться журнал действия.|
|status|string| Состояние действия. Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.|
|user|String| Имя участника-пользователя, который выполнил вход в действие (POST). Пользователь должен быть извлечен из маркера проверки подлинности и не был введен вручную вызывающим приложением вручную.|
|Вендоринформатион|[Секуритивендоринформатион](securityvendorinformation.md)|Сложный тип, содержащий сведения о продуктах, поставщиках и подчиненных поставщиках системы безопасности (например, Vendor = Microsoft; Provider = защитник Windows ATP; подчиненный поставщик = AppLocker).|

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "actionReason": "String",
  "appId": "String",
  "azureTenantId": "String",
  "clientContext": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "errorInfo": {"@odata.type": "microsoft.graph.resultInfo"},
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "states": [{"@odata.type": "microsoft.graph.securityActionState"}],
  "status": "string",
  "user": "String",
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
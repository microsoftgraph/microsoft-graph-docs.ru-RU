---
title: тип ресурса securityAction
description: Принимайте незамедлительные действия по защите от угроз с помощью объекта securityAction Microsoft Graph Security. Если аналитик безопасности обнаруживает новый индикатор, например вредоносный файл, URL-адрес, домен или IP-адрес, можно сразу же включить защиту в решении по обеспечению безопасности от корпорации Майкрософт. Вызывайте действие для определенного поставщика услуг, просматривайте все выполненные действия и отменяйте действие при необходимости. Попробуйте действия по безопасности Защитник Windows endpoint (скоро) для блокировки вредоносных действий на конечных точках Windows с использованием свойств, замеченных в оповещениях или идентифицированных во время расследований.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: dc1a196fbd6da8f0e7464c3991c710917f8e807f
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424441"
---
# <a name="securityaction-resource-type"></a>тип ресурса securityAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Принимайте незамедлительные действия по защите от угроз с помощью объекта securityAction Microsoft Graph Security. Если аналитик безопасности обнаруживает новый индикатор, например вредоносный файл, URL-адрес, домен или IP-адрес, можно сразу же включить защиту в решении по обеспечению безопасности от корпорации Майкрософт. Вызывайте действие для определенного поставщика услуг, просматривайте все выполненные действия и отменяйте действие при необходимости. Попробуйте действия по Защитник Windows для [конечной](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) точки, чтобы заблокировать вредоносные действия на конечных точках Windows с помощью свойств, замеченных в оповещениях или выявленных во время расследований.

  > **Примечание.** В настоящее время действия по обеспечению безопасности поддерживают только разрешения для приложений.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение действия по обеспечению безопасности](../api/securityaction-get.md) | [securityAction](securityaction.md) | Чтение свойств и связей объекта securityAction. |
| [Создание действия по обеспечению безопасности](../api/securityactions-post.md) | [securityAction](securityaction.md) | Создайте новую службу безопасности, разместив ее в коллекции securityActions. |
| [Перечисление действий по обеспечению безопасности](../api/securityactions-list.md) | [коллекция securityAction](securityaction.md) | Получите коллекцию объектов securityAction. |
|[Отмена действия по обеспечению безопасности](../api/securityaction-cancelsecurityaction.md)|Нет|Отмена операции безопасности.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|actionReason|Строка|Причина для этого действия.|
|appId|String|ID приложения вызываемого приложения, которое представило (POST) действие. AppId должен быть извлечен из маркера auth и не вошел вручную в вызываемом приложении.|
|azureTenantId|String|ID клиента Azure для субъекта, чтобы определить, к какову клиенту принадлежит объект (поддержка с несколькими арендами). AzureTenantId должен быть извлечен из маркера auth и не вошел вручную с помощью вызываемого приложения.|
|completedDateTime|DateTimeOffset|Timestamp, когда действие было завершено. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|createdDateTime|DateTimeOffset|Timestamp, когда действие создано. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|errorInfo|[resultInfo](resultinfo.md)| Сведения об ошибках при сбойе действия.|
|id|Строка| Создается системой при прохо- Созданный GUID/уникальный идентификатор. Только для чтения.|
|lastActionDateTime|DateTimeOffset| Timestamp при последнем обновлении этого действия. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|name|String| Имя действия.|
|parameters|Коллекция [keyValuePair](keyvaluepair.md)| Набор параметров (пары значений ключа), необходимых для вызова действия, например URL-адреса или fileHash для блокировки.). **Обязательное поле**.|
|состояния|[коллекция securityActionState](securityactionstate.md)|Коллекция securityActionState для сохраняемой истории действия.|
|status|string| Состояние действия. Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.|
|пользователь|Строка| Основное имя пользователя пользователя, который отправил (POST) действие. Пользователь должен быть извлечен из маркера auth и не вошел вручную с помощью вызываемого приложения.|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|Сложный тип, содержащий сведения о поставщике продукта и службы безопасности, поставщике и суб-поставщике (например, поставщик=Microsoft; provider=Защитник Windows ATP; sub-provider=AppLocker).|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
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

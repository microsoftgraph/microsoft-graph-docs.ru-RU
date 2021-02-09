---
title: Тип ресурса securityAction
description: Принимайте незамедлительные действия по защите от угроз с помощью объекта securityAction Microsoft Graph Security. Если аналитик безопасности обнаруживает новый индикатор, например вредоносный файл, URL-адрес, домен или IP-адрес, можно сразу же включить защиту в решении по обеспечению безопасности от корпорации Майкрософт. Вызывайте действие для определенного поставщика услуг, просматривайте все выполненные действия и отменяйте действие при необходимости. Воспользуйтесь действиями по обеспечению безопасности с помощью ATP в Защитнике Windows (ожидается в ближайшее время), чтобы заблокировать вредоносную активность в конечных точках Windows с использованием свойств, отображаемых в оповещениях или выявленных при изучении.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9bd20ddb5a228cf6764dc2ecf6ff770218ca916a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159443"
---
# <a name="securityaction-resource-type"></a>Тип ресурса securityAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Принимайте незамедлительные действия по защите от угроз с помощью объекта securityAction Microsoft Graph Security. Если аналитик безопасности обнаруживает новый индикатор, например вредоносный файл, URL-адрес, домен или IP-адрес, можно сразу же включить защиту в решении по обеспечению безопасности от корпорации Майкрософт. Вызывайте действие для определенного поставщика услуг, просматривайте все выполненные действия и отменяйте действие при необходимости. Воспользуйтесь действиями по обеспечению безопасности с помощью [ATP в Защитнике Windows](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection), чтобы заблокировать вредоносную активность в конечных точках Windows с использованием свойств, отображаемых в оповещениях или выявленных при изучении.

  > **Примечание.** В настоящее время действия по обеспечению безопасности поддерживают только разрешения для приложений.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение действия по обеспечению безопасности](../api/securityaction-get.md) | [securityAction](securityaction.md) | Чтение свойств и связей объекта securityAction. |
| [Создание действия по обеспечению безопасности](../api/securityactions-post.md) | [securityAction](securityaction.md) | Создание нового securityAction путем публикации в коллекции securityActions. |
| [Перечисление действий по обеспечению безопасности](../api/securityactions-list.md) | [коллекция securityAction](securityaction.md) | Получите коллекцию объектов securityAction. |
|[Отмена действия по обеспечению безопасности](../api/securityaction-cancelsecurityaction.md)|Нет|Отмена операции безопасности.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|actionReason|String|Причина для этого действия.|
|appId|String|ИД вызываемого приложения, которое отправило действие (POST). AppId должен быть извлечен из маркера проверки, а не введен приложением вызова вручную.|
|azureTenantId|String|Azure tenant ID of the entity to determine which tenant the entity belongs to (multi-tenancy support). AzureTenantId должен извлекаться из маркера проверки и не ввели вручную вызывающей приложением.|
|completedDateTime|DateTimeOffset|Timestamp when the action was completed. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|createdDateTime|DateTimeOffset|Timestamp when the action is created. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|errorInfo|[resultInfo](resultinfo.md)| Сведения об ошибке при сбойе действия.|
|id|String| Создается системой при в отношении действия. Созданный ИДЕНТИФИКАТОР GUID/уникальный идентификатор. Только для чтения.|
|lastActionDateTime|DateTimeOffset| Timestamp when this action was last updated. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|name|String| Имя действия.|
|parameters|Коллекция [keyValuePair](keyvaluepair.md)| Коллекция параметров (пар "ключ-значение"), необходимых для вызова действия, например URL-адрес или fileHash для блокировки и т. д.). **Required**|
|states|[Коллекция securityActionState](securityactionstate.md)|Коллекция securityActionState для сохраняемого истории действия.|
|status|string| Состояние действия. Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.|
|user|String| Имя вошел пользователя, который отправил (POST) действие. Пользователь должен быть извлечен из маркера проверки и не введен приложением- вызовом вручную.|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|Сложный тип, содержащий сведения о поставщике продукта или службы безопасности, поставщике и вложенных поставщиках (например, vendor=Microsoft; provider=Защитник Windows ATP; sub-provider=AppLocker).|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

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
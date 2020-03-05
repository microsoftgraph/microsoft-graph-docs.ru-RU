---
title: Тип ресурса Воркфорцеинтегратион
description: Экземпляр интеграции сотрудников с сменами.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1e836a4346fe5e31f39c1f6383acbf78530ae9e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519087"
---
# <a name="workforceintegration-resource-type"></a>Тип ресурса Воркфорцеинтегратион

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Экземпляр интеграции сотрудников с сменами.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/workforceintegration-get.md); | [воркфорцеинтегратион](workforceintegration.md) | Чтение свойств и связей объекта **воркфорцеинтегратион** . |
| [обновление](../api/workforceintegration-update.md). | [воркфорцеинтегратион](workforceintegration.md) | Обновление объекта **воркфорцеинтегратион** . |
| [удаление](../api/workforceintegration-delete.md); | Нет | Удаление объекта **воркфорцеинтегратион** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|апиверсион|Int32|Версия API для URL-адреса обратного вызова. Начните с 1.|
|displayName|String|Имя интеграции трудовых ресурсов.|
|шифрования|[воркфорцеинтегратионенкриптион](workforceintegrationencryption.md)|Ресурс для шифрования взаимодействия сотрудников.|
|isActive|Логический|Указывает, активна ли эта интеграция сотрудников в настоящее время и доступна ли она.|
|имеется|строка| Возможные значения: `none`, `shift`, `swapRequest`, `openshift`,, `openShiftRequest``userShiftPreferences`|
|url|String| URL-адрес интеграции сотрудников для обратных вызовов из службы смены.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegration",
  "baseType": ""
}-->

```json
{
  "apiVersion": 1024,
  "displayName": "String",
  "encryption": {"@odata.type": "microsoft.graph.workforceIntegrationEncryption"},
  "isActive": true,
  "supports": "string",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

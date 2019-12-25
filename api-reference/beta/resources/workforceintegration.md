---
title: Тип ресурса Воркфорцеинтегратион
description: Экземпляр интеграции сотрудников с сменами.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 631f2cc52b9327d77edd6fc5ad48292cf044570f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866492"
---
# <a name="workforceintegration-resource-type"></a>Тип ресурса Воркфорцеинтегратион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Экземпляр интеграции сотрудников с сменами.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/workforceintegration-get.md); | [воркфорцеинтегратион](workforceintegration.md) | Чтение свойств и связей объекта **воркфорцеинтегратион** . |
| [обновление](../api/workforceintegration-update.md). | [воркфорцеинтегратион](workforceintegration.md) | Обновление объекта **воркфорцеинтегратион** . |
| [удаление](../api/workforceintegration-delete.md); | Нет. | Удаление объекта **воркфорцеинтегратион** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|апиверсион|Int32|Версия API для URL-адреса обратного вызова. Начните с 1.|
|displayName|String|Имя интеграции трудовых ресурсов.|
|шифрования|[воркфорцеинтегратионенкриптион](workforceintegrationencryption.md)|Ресурс для шифрования взаимодействия сотрудников.|
|isActive|Логический|Указывает, активна ли эта интеграция сотрудников в настоящее время и доступна ли она.|
|имеется|string| Возможные значения: `none`, `shift`, `swapRequest`, `openshift`,, `openShiftRequest``userShiftPreferences`|
|url|String| URL-адрес интеграции сотрудников для обратных вызовов из службы смены.|

## <a name="relationships"></a>Отношения

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

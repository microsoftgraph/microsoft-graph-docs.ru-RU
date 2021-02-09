---
title: Тип ресурса workforceIntegration
description: Экземпляр интеграции сотрудников со сменами.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9b9e8678a009dab1f6e6cceae8b9ce98d1849cbd
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158312"
---
# <a name="workforceintegration-resource-type"></a>Тип ресурса workforceIntegration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Экземпляр интеграции сотрудников со сменами.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/workforceintegration-list.md) | [коллекция workforceIntegration](workforceintegration.md) | Получите список объектов **workforceIntegration,** связанных с этим расписанием.|
| [Создание](../api/workforceintegration-post.md) | [workforceIntegration](workforceintegration.md) | Создание объекта **workforceIntegration.**|
| [Получение](../api/workforceintegration-get.md) | [workforceIntegration](workforceintegration.md) | Чтение свойств и связей объекта **workforceIntegration.** |
| [Обновление](../api/workforceintegration-update.md) | [workforceIntegration](workforceintegration.md) | Обновление объекта **workforceIntegration.** |
| [удаление](../api/workforceintegration-delete.md); | Нет | Удаление объекта **workforceIntegration.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|apiVersion|Int32|Версия API для URL-адреса обратного вызова. Начните с 1.|
|displayName|String|Имя интеграции сотрудников.|
|шифрование|[workforceIntegrationEncryption](workforceintegrationencryption.md)|Ресурс шифрования интеграции сотрудников.|
|isActive|Boolean|Указывает, активна ли в настоящее время интеграция с сотрудниками.|
|поддерживает|string| Объекты Shifts, поддерживаемые для синхронных уведомлений об изменениях. Смены будут возвращать URL-адрес, предоставленный при изменениях клиентов для добавленных здесь сущностями. По умолчанию уведомления об изменениях не поддерживаются никакими сущностями. Возможные значения: `none` , , , `shift` `swapRequest` `openshift` `openShiftRequest` , `userShiftPreferences`|
|supportedEntities|string| Это свойство заменит **поддержку** в v1.0. Рекомендуется использовать это свойство вместо **поддержки.** В **настоящее время** свойство supports будет по-прежнему поддерживаться в бета-версии. Возможные значения: `none` , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` . Если выбрано несколько значений, все значения должны начинаться с первой буквы в верхнем регистре.|
|url|String| URL-адрес интеграции сотрудников для переключеных вызовов из службы shifts.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegration"
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



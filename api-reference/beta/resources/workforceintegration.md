---
title: тип ресурса workforceIntegration
description: Пример интеграции рабочей силы со сменами.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7e53497b3edb017a9c1e7ada7493bc5fa4505680
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665895"
---
# <a name="workforceintegration-resource-type"></a>тип ресурса workforceIntegration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Пример интеграции рабочей силы со сменами.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/workforceintegration-list.md) | [коллекция workforceIntegration](workforceintegration.md) | Получите список объектов **workforceIntegration,** связанных с этим расписанием.|
| [Создание](../api/workforceintegration-post.md) | [workforceIntegration](workforceintegration.md) | Создание нового **объекта workforceIntegration.**|
| [Получение](../api/workforceintegration-get.md) | [workforceIntegration](workforceintegration.md) | Ознакомьтесь с свойствами и отношениями объекта **workforceIntegration.** |
| [Обновление](../api/workforceintegration-update.md) | [workforceIntegration](workforceintegration.md) | Обновление объекта **workforceIntegration.** |
| [Удаление](../api/workforceintegration-delete.md) | Нет | Удаление объекта **workforceIntegration.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|apiVersion|Int32|Версия API для URL-адреса обратного вызова. Начните с 1.|
|displayName|String|Имя интеграции рабочей силы.|
|шифрование|[workforceIntegrationEncryption](workforceintegrationencryption.md)|Ресурс шифрования интеграции рабочей силы.|
|isActive|Логический|Указывает, является ли эта интеграция рабочей силы активной и доступной в настоящее время.|
|поддерживает|workforceIntegrationSupportedEntities | Объекты Shifts, поддерживаемые для синхронных уведомлений об изменении. Shifts сделает вызов обратно на URL-адрес, предоставленный при изменениях клиента для добавленных здесь сущностями. По умолчанию для уведомлений об изменении не поддерживаются никакие сущностями. <br><br>Возможные значения: `none` , , , , , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` `offerShiftRequest` `unknownFutureValue` `timeCard` `timeOffReason` `timeOff` `timeOffRequest` . Обратите внимание, что для получения следующих значений в этом развиваемом переуме- `Prefer: include-unknown-enum-members` [](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `timeCard` `timeOffReason` `timeOff` `timeOffRequest` <br><br>Если выбрано несколько значений, все значения должны начинаться с первой буквы в верхнем шкафу.|
|supportedEntities|workforceIntegrationSupportedEntities | Это свойство заменило **поддержки** в v1.0. Рекомендуется использовать это свойство вместо **поддержки.** Свойство **поддерживается** до сих пор в бета-версии. <br><br>Возможные значения: `none` , , , , , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` `offerShiftRequest` `unknownFutureValue` `timeCard` `timeOffReason` `timeOff` `timeOffRequest` . Обратите внимание, что для получения следующих значений в этом развиваемом переуме- `Prefer: include-unknown-enum-members` [](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `timeCard` `timeOffReason` `timeOff` `timeOffRequest` <br><br>Если выбрано несколько значений, все значения должны начинаться с первой буквы в верхнем шкафу.|
|url|String| URL-адрес интеграции рабочей силы для откатов из службы Shifts.|

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
  "supportedEntities": "string",
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



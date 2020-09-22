---
title: Тип ресурса Воркфорцеинтегратион
description: Экземпляр интеграции сотрудников с сменами.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 715c78e8cb412f11b7b336680e3c433369c9e608
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015101"
---
# <a name="workforceintegration-resource-type"></a>Тип ресурса Воркфорцеинтегратион

Пространство имен: microsoft.graph

Экземпляр интеграции сотрудников с сменами.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/workforceintegration-post.md) | [воркфорцеинтегратион](workforceintegration.md) | Создание нового объекта **воркфорцеинтегратион** .|
| [List](../api/workforceintegration-list.md) | Коллекция [воркфорцеинтегратион](workforceintegration.md) | Получение списка объектов **воркфорцеинтегратион** , связанных с этим расписанием.|
| [получение](../api/workforceintegration-get.md); | [воркфорцеинтегратион](workforceintegration.md) | Чтение свойств и связей объекта **воркфорцеинтегратион** . |
| [обновление](../api/workforceintegration-update.md). | [воркфорцеинтегратион](workforceintegration.md) | Обновление объекта **воркфорцеинтегратион** . |
| [удаление](../api/workforceintegration-delete.md); | Нет | Удаление объекта **воркфорцеинтегратион** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|апиверсион|Int32|Версия API для URL-адреса обратного вызова. Начните с 1.|
|displayName|String|Имя интеграции трудовых ресурсов.|
|шифрования|[воркфорцеинтегратионенкриптион](workforceintegrationencryption.md)|Ресурс для шифрования взаимодействия сотрудников.|
|isActive|Boolean|Указывает, активна ли эта интеграция сотрудников в настоящее время и доступна ли она.|
|суппортедентитиес|string| Сущности сдвигов, поддерживаемые для синхронных уведомлений об изменении. Смены потребуют обратного вызова на URL-адрес, указанный в изменениях клиентов для этих сущностей, добавленных здесь. По умолчанию для уведомлений об изменениях не поддерживаются никакие сущности. Возможные значения: `none` , `shift` ,, `swapRequest` , `openshift` `openShiftRequest` , `userShiftPreferences`|
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


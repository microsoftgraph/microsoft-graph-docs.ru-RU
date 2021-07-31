---
title: тип ресурса workforceIntegration
description: Пример интеграции рабочей силы со сменами.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e8c05e82ccf92a46f9d3e511de000d2d36cd38db
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665874"
---
# <a name="workforceintegration-resource-type"></a>тип ресурса workforceIntegration

Пространство имен: microsoft.graph

Пример интеграции рабочей силы со сменами.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/workforceintegration-post.md) | [workforceIntegration](workforceintegration.md) | Создание нового **объекта workforceIntegration.**|
| [Список](../api/workforceintegration-list.md) | [коллекция workforceIntegration](workforceintegration.md) | Получите список объектов **workforceIntegration,** связанных с этим расписанием.|
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
|supportedEntities|workforceIntegrationSupportedEntities | Объекты Shifts, поддерживаемые для синхронных уведомлений об изменении. Shifts сделает вызов обратно на URL-адрес, предоставленный при изменениях клиента для добавленных здесь сущностями. По умолчанию для уведомлений об изменении не поддерживаются никакие сущностями. Возможные значения: `none`, `shift`, `swapRequest`, `userShiftPreferences`, `openshift`, `openShiftRequest`, `offerShiftRequest`, `unknownFutureValue`.|
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


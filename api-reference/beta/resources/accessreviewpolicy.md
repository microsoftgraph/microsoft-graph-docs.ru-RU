---
title: тип ресурсов accessReviewPolicy
description: Политика обзоров доступа — это одинтон, который позволяет организациям управлять политикой проверки доступа на уровне каталогов.
author: kafen
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 02940987682d84aa3fc3dbb076c998abfe24bf8e
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068160"
---
# <a name="accessreviewpolicy-resource-type"></a>тип ресурсов accessReviewPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Политика проверки доступа — это одинтон, который позволяет администраторам управлять политиками проверки доступа на уровне каталогов. Например, администраторы могут использовать политику проверки доступа, чтобы включить и отключить возможность владельцев групп создавать отзывы о доступе в группах, которые им принадлежат.


Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получить accessReviewPolicy](../api/accessreviewpolicy-get.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewPolicy.](../resources/accessreviewpolicy.md)|
|[Обновление accessReviewPolicy](../api/accessreviewpolicy-update.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Обновление свойств объекта [accessReviewPolicy.](../resources/accessreviewpolicy.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание этой политики. Только для чтения.|
|displayName|String|Отображение имени для этой политики. Только для чтения.|
|isGroupOwnerManagementEnabled|Логический|Если `true` владельцы групп могут создавать и управлять отзывами доступа в группах, которые им принадлежат.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewPolicy",
  "displayName": "Access Review Policy",
  "description": "Policy contains directory-level access review settings.",
  "isGroupOwnerManagementEnabled": false
}
```

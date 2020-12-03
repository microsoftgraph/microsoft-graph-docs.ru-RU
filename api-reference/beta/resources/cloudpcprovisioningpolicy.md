---
title: Тип ресурса Клаудпкпровисионингполици
description: Представляет политику подготовки облачных ПК.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 58fa7ff74086d39d124f3d4701f5951636fd8eda
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563760"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>Тип ресурса Клаудпкпровисионингполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику подготовки облачных ПК.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список ПровисионингполиЦиес](../api/virtualendpoint-list-provisioningpolicies.md)|Коллекция [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md)|Список свойств и связей объектов [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .|
|[Получение Клаудпкпровисионингполици](../api/cloudpcprovisioningpolicy-get.md)|[клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md)|Чтение свойств и связей объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .|
|[Создание Клаудпкпровисионингполици](../api/virtualendpoint-post-provisioningpolicies.md)|[клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md)|Создание нового объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .|
|[Обновление Клаудпкпровисионингполици](../api/cloudpcprovisioningpolicy-update.md)|[клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md)|Обновление свойств объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .|
|[Удаление Клаудпкпровисионингполици](../api/cloudpcprovisioningpolicy-delete.md)|Нет|Удаление объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .|
|[Назначение Клаудпкпровисионингполици](../api/cloudpcprovisioningpolicy-assign.md)|Нет |Назначьте [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) группам пользователей.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для политики подготовки облачных ПК. Только для чтения.|
|displayName|String|Отображаемое имя политики подготовки.|
|description|String|Описание политики подготовки.|
|онпремисесконнектионид|String|Идентификатор Клаудпконпремисесконнектион. Чтобы обеспечить сетевое подключение к облачным компьютерам и присоединение к домену, выберите подключение с виртуальной сетью, проверенной службой Cloud PC.|
|имажеид|String|Идентификатор образа ОС, который вы хотите подготовить к работе на облачных компьютерах. Формат изображения для типа галереи: {publisher_offer_sku}.|
|имажедисплайнаме|String|Отображаемое имя для образа ОС, который вы собираетесь заготовить.|
|имажетипе|клаудпкпровисионингполициимажетипе|Тип образа ОС (настраиваемого или галереи), который необходимо подготовить к работе на облачных компьютерах. Возможные значения: `gallery`, `custom`.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [клаудпкпровисионингполициассигнмент](../resources/cloudpcprovisioningpolicyassignment.md)|Определенная коллекция назначений политик подготовки. Возвращается только на `$expand`. В этом [примере](../api/cloudpcprovisioningpolicy-get.md) показано, как получить отношение назначений. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "onPremisesConnectionId": "String",
  "imageId": "String",
  "imageDisplayName": "String",
  "imageType": "String"
}
```

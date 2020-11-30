---
title: Тип ресурса Клаудпкпровисионингполици
description: Представляет политику подготовки облачных ПК.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 32a4116d6fa26109b8df57786545a0726aa7dd4e
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378491"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>Тип ресурса Клаудпкпровисионингполици

Пространство имен: microsoft.graph

Представляет политику подготовки облачных ПК.

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
|id|Строка|Уникальный идентификатор для политики подготовки облачных ПК. Только для чтения.|
|displayName|Строка|Отображаемое имя политики подготовки.|
|description|Строка|Описание политики подготовки.|
|онпремисесконнектионид|Строка|Идентификатор Клаудпконпремисесконнектион. Чтобы обеспечить сетевое подключение к облачным компьютерам и присоединение к домену, выберите подключение с виртуальной сетью, проверенной службой Cloud PC.|
|имажеид|Строка|Идентификатор образа ОС, который вы хотите подготовить к работе на облачных компьютерах. Формат изображения для типа галереи: {publisher_offer_sku}.|
|имажедисплайнаме|Строка|Отображаемое имя для образа ОС, который вы собираетесь заготовить.|
|имажетипе|клаудпкпровисионингполициимажетипе|Тип образа ОС (настраиваемого или галереи), который необходимо подготовить к работе на облачных компьютерах. Возможные значения: `gallery`, `custom`.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [клаудпкпровисионингполициассигнмент](../resources/cloudpcprovisioningpolicyassignment.md)|Определенная коллекция назначений политик подготовки. Возвращается только с помощью оператора `$expand`. В этом [примере](../api/cloudpcprovisioningpolicy-get.md) показано, как получить отношение назначений. |

## <a name="json-representation"></a>Представление в формате JSON

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

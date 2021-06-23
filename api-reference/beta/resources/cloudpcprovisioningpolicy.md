---
title: тип ресурса cloudPcProvisioningPolicy
description: Представляет политику продюсинга облачных компьютеров.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: b1f5a447c373e64b747fc77ec93c54d8adc09c60
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082078"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>тип ресурса cloudPcProvisioningPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику продюсинга облачных компьютеров.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[коллекция cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Список свойств и связей объектов [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Get cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-get.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Создание cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Создайте новый [объект cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Обновление cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-update.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Обновление свойств объекта [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Удаление cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-delete.md)|Нет|Удаление [объекта cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Назначение cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-assign.md)|Нет |Назначение [cloudPcProvisioningPolicy группам](../resources/cloudpcprovisioningpolicy.md) пользователей.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор политики обеспечения облачного компьютера. Только для чтения.|
|displayName|String|Имя отображения политики обеспечения.|
|description|String|Описание политики обеспечения.|
|onPremisesConnectionId|String|ID cloudPcOnPremisesConnection. Чтобы обеспечить подключение к облачным компьютерам и подключение к домену, выберите подключение к виртуальной сети, проверенное службой облачных ПК.|
|imageId|String|ID изображения ОС, которое необходимо уладить на облачных ПК. Формат изображения типа галереи: {publisher_offer_sku}.|
|imageDisplayName|String|Имя отображения образа ОС, которое вы закаповыватель.|
|imageType|cloudPcProvisioningPolicyImageType|Тип изображения ОС (настраиваемый или галерейный) для предоставления на облачных ПК. Возможные значения: `gallery`, `custom`.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md)|Определенный набор назначений политики обеспечения. Представляет набор групп Microsoft 365 и групп безопасности в Azure AD, которые имеют назначенную политику обеспечения. Возвращается только с помощью оператора `$expand`. Пример [получения](../api/cloudpcprovisioningpolicy-get.md) отношений назначений. |

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

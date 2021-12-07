---
title: тип ресурса cloudPcProvisioningPolicy
description: Представляет политику продюсинга облачных КОМПЬЮТЕРов.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 64a793151e685e008999b87eeea32dc5e79a7d0a
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322223"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>тип ресурса cloudPcProvisioningPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику продюсинга облачных КОМПЬЮТЕРов.

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
|id|String|Уникальный идентификатор для политики продюсинга облачных ПК. Только для чтения.|
|displayName|String|Имя отображения политики обеспечения.|
|description|Строка|Описание политики обеспечения.|
|onPremisesConnectionId|Строка|ID cloudPcOnPremisesConnection. Чтобы обеспечить подключение к облачным компьютерам и подключение к домену, выберите подключение к виртуальной сети, проверенной службой облачных ПК.|
|imageId|String|ID изображения ОС, которое необходимо уладить на облачных ПК. Формат изображения типа галереи: {publisher_offer_sku}. Поддерживаемые значения для каждого из параметров:<ul><li>издатель: Microsoftwindowsdesktop.</li> <li>предложение: windows-ent-cpc.</li> <li>sku: 21h1-ent-cpc-m365, 21h1-ent-cpc-os, 20h2-ent-cpc-m365, 20h2-ent-cpc-os, 20h1-ent-cpc-m365, 20h1-ent-cpc-os, 19h2-ent-cpc-os.</li></ul>|
|imageDisplayName|Строка|Имя отображения образа ОС, которое вы закаповыватель.|
|imageType|cloudPcProvisioningPolicyImageType|Тип изображения ОС (настраиваемый или галерейный) для предоставления на облачных ПК. Возможные значения: `gallery`, `custom`.|
|MicrosoftManagedDesktop|[MicrosoftManagedDesktop](../resources/microsoftManagedDesktop.md)|Конкретные параметры для компьютеры, управляемые Майкрософт, которые позволяют клиентам получать управляемое устройство для облачного КОМПЬЮТЕРА. Прежде чем включить компьютеры, управляемые Майкрософт, администратор должен настроить его.|
|domainJoinConfiguration|[cloudPcDomainJoinConfiguration](../resources/cloudpcdomainjoinconfiguration.md)|Указывает, как облачные ПК присоединятся к Azure Active Directory.|

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
  "imageType": "String",
  "microsoftManagedDesktop": {
    "type": "String",
    "profile": "String"
  },
  "domainJoinConfiguration": {
    "@odata.type": "microsoft.graph.cloudPcDomainJoinConfiguration"
  }
}
```

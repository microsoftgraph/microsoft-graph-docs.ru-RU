---
title: тип ресурса cloudPcProvisioningPolicy
description: Представляет политику продюсинга облачных КОМПЬЮТЕРов.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: b16d4a95bf791b387958605b64e7a370e1c3971f
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014287"
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
|description|Строка|Описание политики обеспечения.|
|displayName|Строка|Имя отображения политики обеспечения.|
|domainJoinConfiguration|[cloudPcDomainJoinConfiguration](../resources/cloudpcdomainjoinconfiguration.md)|Указывает, как облачные ПК присоединятся к Azure Active Directory.|
|id|Строка|Уникальный идентификатор для политики продюсинга облачных ПК. Только для чтения.|
|imageDisplayName|Строка|Имя отображения образа ОС, которое вы закаповыватель.|
|imageId|Строка|ID изображения ОС, которое необходимо уладить на облачных ПК. Формат изображения типа галереи: {publisher_offer_sku}. Поддерживаемые значения для каждого из параметров:<ul><li>издатель: Microsoftwindowsdesktop.</li> <li>предложение: windows-ent-cpc.</li> <li>sku: 21h1-ent-cpc-m365, 21h1-ent-cpc-os, 20h2-ent-cpc-m365, 20h2-ent-cpc-os, 20h1-ent-cpc-m365, 20h1-ent-cpc-os, 19h2-ent-cpc-os.</li></ul>|
|imageType|cloudPcProvisioningPolicyImageType|Тип изображения ОС (настраиваемый или галерейный) для предоставления на облачных ПК. Возможные значения: `gallery`, `custom`.|
|MicrosoftManagedDesktop|[MicrosoftManagedDesktop](../resources/microsoftManagedDesktop.md)|Конкретные параметры для компьютеры, управляемые Майкрософт, которые позволяют клиентам получать управляемое устройство для облачного КОМПЬЮТЕРА. Прежде чем включить компьютеры, управляемые Майкрософт, администратор должен настроить его.|
|onPremisesConnectionId|String|ID cloudPcOnPremisesConnection. Чтобы обеспечить подключение к облачным компьютерам и подключение к домену, выберите подключение к виртуальной сети, проверенной службой облачных ПК.|

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
  "description": "String",
  "displayName": "String",
  "domainJoinConfiguration": {
    "@odata.type": "microsoft.graph.cloudPcDomainJoinConfiguration"
  },
  "id": "String (identifier)",
  "imageDisplayName": "String",
  "imageId": "String",
  "imageType": "String",
  "microsoftManagedDesktop": {
    "type": "String",
    "profile": "String"
  },
  "onPremisesConnectionId": "String"
}
```

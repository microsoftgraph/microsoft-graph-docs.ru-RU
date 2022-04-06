---
title: тип ресурса cloudPcProvisioningPolicy
description: Представляет политику продюсинга облачных КОМПЬЮТЕРов.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d17c16005c812152bc8d009508782db37faf7e89
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63721825"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>тип ресурса cloudPcProvisioningPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику продюсинга облачных КОМПЬЮТЕРов.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[коллекция cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Список свойств и связей объектов [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Get cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-get.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Создание cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Создайте новый [объект cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Обновление cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-update.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Обновление свойств объекта [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Удаление cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-delete.md)|Отсутствует|Удаление [объекта cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Назначение cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-assign.md)|Отсутствует |Назначение [cloudPcProvisioningPolicy группам](../resources/cloudpcprovisioningpolicy.md) пользователей.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание политики обеспечения.|
|displayName|String|Имя отображения политики обеспечения.|
|domainJoinConfiguration|[cloudPcDomainJoinConfiguration](../resources/cloudpcdomainjoinconfiguration.md)|Указывает, как облачные компьютеры присоединятся к Azure Active Directory.|
|id|String|Уникальный идентификатор для политики продюсинга облачных ПК. Только для чтения.|
|imageDisplayName|String|Имя отображения образа ОС, которое вы закаповыватель.|
|imageId|String|ID изображения ОС, которое необходимо уладить на облачных ПК. Формат изображения типа галереи: {publisher_offer_sku}. Поддерживаемые значения для каждого из параметров:<ul><li>издатель: Microsoftwindowsdesktop.</li> <li>предложение: windows-ent-cpc.</li> <li>sku: 21h1-ent-cpc-m365, 21h1-ent-cpc-os, 20h2-ent-cpc-m365, 20h2-ent-cpc-os, 20h1-ent-cpc-m365, 20h1-ent-cpc-os, 19h2-ent-cpc-os.</li></ul>|
|imageType|cloudPcProvisioningPolicyImageType|Тип изображения ОС (настраиваемый или галерейный) для предоставления на облачных ПК. Возможные значения: `gallery`, `custom`.|
|MicrosoftManagedDesktop|[MicrosoftManagedDesktop](../resources/microsoftManagedDesktop.md)|Конкретные параметры для компьютеры, управляемые Майкрософт, которые позволяют клиентам получать управляемое устройство для облачного КОМПЬЮТЕРА. Прежде чем включить компьютеры, управляемые Майкрософт, администратор должен настроить его.|
|onPremisesConnectionId|String|ID cloudPcOnPremisesConnection. Чтобы обеспечить подключение к облачным компьютерам и подключение к домену, выберите подключение к виртуальной сети, проверенной службой облачных ПК.|
|WindowsSettings|[cloudPcWindowsSettings](../resources/cloudpcwindowssettings.md)|Определенные Windows настройки при создании облачных компьютеров для этой политики обеспечения.|

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
  "domainJoinConfiguration": {
    "@odata.type": "microsoft.graph.cloudPcDomainJoinConfiguration"
  },
  "onPremisesConnectionId": "String",
  "windowsSettings": {
    "@odata.type": "microsoft.graph.cloudPcWindowsSettings"
  }
}
```

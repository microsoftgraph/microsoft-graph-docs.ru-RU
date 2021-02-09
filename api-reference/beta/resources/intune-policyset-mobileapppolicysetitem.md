---
title: Тип ресурса mobileAppPolicySetItem
description: Класс, содержащий свойства, используемые для объекта PolicySetItem мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7e05859971181518d9ab457f612df7e2400206b2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156772"
---
# <a name="mobileapppolicysetitem-resource-type"></a>Тип ресурса mobileAppPolicySetItem

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для объекта PolicySetItem мобильного приложения.


Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileAppPolicySetItems](../api/intune-policyset-mobileapppolicysetitem-list.md)|[Коллекция mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Список свойств и связей объектов [mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)|
|[Get mobileAppPolicySetItem](../api/intune-policyset-mobileapppolicysetitem-get.md)|[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Чтение свойств и связей объекта [mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)|
|[Создание mobileAppPolicySetItem](../api/intune-policyset-mobileapppolicysetitem-create.md)|[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Создание объекта [mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)|
|[Удаление mobileAppPolicySetItem](../api/intune-policyset-mobileapppolicysetitem-delete.md)|Нет|Удаляет [mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)|
|[Обновление mobileAppPolicySetItem](../api/intune-policyset-mobileapppolicysetitem-update.md)|[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Обновление свойств объекта [mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ MobileAppPolicySetItem. Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Время создания policySetItem. Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения policySetItem. Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|String|PayloadId для PolicySetItem. Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|String|policySetType для PolicySetItem. Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|String|DisplayName для PolicySetItem. Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Состояние policySetItem. Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md). Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Код ошибки, если она произошла. Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|Коллекция String|Теги управляемого развертывания. Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)|
|intent|[installIntent](../resources/intune-shared-installintent.md)|Установка намерения MobileAppPolicySetItem. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|settings|[mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)|Параметры MobileAppPolicySetItem.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ],
  "intent": "String",
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "String",
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  }
}
```





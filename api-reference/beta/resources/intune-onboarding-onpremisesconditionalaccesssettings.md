---
title: Тип ресурса onPremisesConditionalAccessSettings
description: Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fe4dd79722392ea5c0e5e6487c3c3dbc3587d4e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566454"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a>Тип ресурса onPremisesConditionalAccessSettings

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта onPremisesConditionalAccessSettings](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md);|Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).|
|[Обновление объекта onPremisesConditionalAccessSettings](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Обновление свойств объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Н/Д|
|enabled|Boolean|Указывает, включен ли в этой организации условный доступ к локальной среде|
|includedGroups|Коллекция объектов Guid|Группы пользователей, для которых включается условный доступ к локальной среде. У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.|
|excludedGroups|Коллекция объектов Guid|Группы пользователей, на которые не распространяется условный доступ к локальной среде. На всех пользователей из этих группах не будет распространяться политика условного доступа.|
|overrideDefaultRule|Boolean|Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```






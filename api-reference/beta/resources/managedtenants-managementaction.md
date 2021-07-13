---
title: тип ресурса managementAction
description: Представляет базовое действие управления для данного управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 156d4ff0d7ffb9574793ccdd5d56bc2a89cd3b22
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403169"
---
# <a name="managementaction-resource-type"></a>тип ресурса managementAction

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет базовое действие управления для данного управляемого клиента. Примерами действий управления являются шифрование устройств, выполнение конфигураций для Azure Active Directory регистрации устройства и многофакторная проверка подлинности для администраторов.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Управление спискамиActions](../api/managedtenants-managedtenant-list-managementactions.md)|[коллекция microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md)|Получите список объектов [managementAction](../resources/managedtenants-managementaction.md) и их свойств.|
|[Get managementAction](../api/managedtenants-managementaction-get.md)|[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md)|Ознакомьтесь с свойствами и отношениями объекта [managementAction.](../resources/managedtenants-managementaction.md)|
|[применение](../api/managedtenants-managementaction-apply.md)|[microsoft.graph.managedTenants.managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md)|Применяет действия управления к управляемому клиенту.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|category|managementCategory|Категория для действия управления. Возможные значения: `custom`, `devices`, `identity`, `unknownFutureValue`. Необязательно. Только для чтения.|
|description|String|Описание действия управления. Необязательно. Только для чтения.|
|displayName|String|Отображает имя для действия управления. Необязательно. Только для чтения.|
|id|String|Уникальный идентификатор для действия управления. Обязательный. Только для чтения.|
|referenceTemplateId|String|Ссылка на шаблон управления, используемый для создания действия управления. Обязательный. Только для чтения.|
|workloadActions|[коллекция microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md)|Набор действий рабочей нагрузки, связанных с действием управления. Обязательный. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementAction",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementAction",
  "id": "String (identifier)",
  "referenceTemplateId": "String",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```

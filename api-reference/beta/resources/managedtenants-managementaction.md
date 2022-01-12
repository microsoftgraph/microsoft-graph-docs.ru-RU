---
title: тип ресурса managementAction
description: Представляет базовое действие управления для данного управляемого клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: f45bcabe1ab488bc5c19e83d7d34e52b92742a43
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61832606"
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
|workloadActions|[коллекция microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md)|Набор действий рабочей нагрузки, связанных с действием управления. Обязательное. Только для чтения.|

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

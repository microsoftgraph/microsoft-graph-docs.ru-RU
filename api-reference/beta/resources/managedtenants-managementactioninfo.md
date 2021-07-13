---
title: тип ресурсов managementActionInfo
description: Представляет справочные сведения для действия управления.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: cde8e52b8329d03169eb5953dd92b897b3b8272e
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402712"
---
# <a name="managementactioninfo-resource-type"></a>тип ресурсов managementActionInfo

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет справочные сведения для действия управления.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|managementActionId|String|Идентификатор для действия управления. Обязательный. Только для чтения.|
|managementTemplateId|String|Идентификатор шаблона управления. Обязательный. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementActionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionInfo",
  "managementTemplateId": "String",
  "managementActionId": "String"
}
```

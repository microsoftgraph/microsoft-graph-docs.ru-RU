---
title: Тип ресурса adminReportSettings
description: Представляет параметры уровня клиента для отчетов Microsoft 365.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: reports
author: qiwhuang
ms.openlocfilehash: faa1073175ca09ef4aee52ecfe55d92d24409687
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856740"
---
# <a name="adminreportsettings-resource-type"></a>Тип ресурса adminReportSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры уровня клиента для отчетов Microsoft 365.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение adminReportSettings](../api/adminreportsettings-get.md)|[adminReportSettings](../resources/adminreportsettings.md)|Получение параметров уровня клиента для отчетов Microsoft 365.|
|[Обновление adminReportSettings](../api/adminreportsettings-update.md)|[adminReportSettings](../resources/adminreportsettings.md)|Обновление параметров уровня клиента для отчетов Microsoft 365.|

## <a name="properties"></a>Свойства

| Свойство       | Тип           | Описание                                 |
| -------------- | -------------- | ------------------------------------------- |
| displayConcealedNames | Логический | Если задано значение , `true`все отчеты будут скрывать сведения о пользователе, такие как имена пользователей, группы и сайты. Если `false`это так, все отчеты будут отображать идентифицируемые сведения. Это свойство представляет параметр в Центр администрирования Microsoft 365. Обязательный элемент. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminReportSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminReportSettings",
  "displayConcealedNames": "Boolean"
}
```

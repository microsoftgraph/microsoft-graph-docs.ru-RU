---
title: тип ресурса tenantDetailedInformation
description: Представляет подробные сведения для управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 40aa157b12ccef64b6eb7ab6c92349a3e74745f8
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402694"
---
# <a name="tenantdetailedinformation-resource-type"></a>тип ресурса tenantDetailedInformation

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения для управляемого клиента.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список tenantDetailedInformation](../api/managedtenants-managedtenant-list-tenantsdetailedinformation.md)|[коллекция microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md)|Получите список объектов [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) и их свойств.|
|[Get tenantDetailedInformation](../api/managedtenants-tenantdetailedinformation-get.md)|[microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md)|Ознакомьтесь с свойствами и отношениями объекта [tenantDetailedInformation.](../resources/managedtenants-tenantdetailedinformation.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|city|String|Город, в котором расположен управляемый клиент. Необязательно. Только для чтения.|
|countryCode|String|Код для страны, в которой расположен управляемый клиент. Необязательно. Только для чтения.|
|countryName|String|Имя страны, в которой расположен управляемый клиент. Необязательно. Только для чтения.|
|defaultDomainName|String|Доменное имя по умолчанию для управляемого клиента. Необязательно. Только для чтения.|
|displayName|String|Имя отображения управляемого клиента.|
|id|String|Уникальный идентификатор для этого объекта. Обязательный. Только для чтения.|
|industryName|String|Бизнес-индустрия, связанная с управляемым клиентом. Необязательно. Только для чтения.|
|регион|String|Регион, в котором расположен управляемый клиент. Необязательно. Только для чтения.|
|segmentName|String|Бизнес-сегмент, связанный с управляемым клиентом. Необязательно. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)|
|verticalName|String|Вертикаль, связанная с управляемым клиентом. Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantDetailedInformation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantDetailedInformation",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String",
  "defaultDomainName": "String",
  "countryName": "String",
  "countryCode": "String",
  "city": "String",
  "region": "String",
  "verticalName": "String",
  "industryName": "String",
  "segmentName": "String"
}
```


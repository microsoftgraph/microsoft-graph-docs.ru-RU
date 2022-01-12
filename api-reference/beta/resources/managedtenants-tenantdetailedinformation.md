---
title: тип ресурса tenantDetailedInformation
description: Представляет подробные сведения для управляемого клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d896492c05223fdf4711842340df5032589913d9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61828847"
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
|id|String|Уникальный идентификатор для этого объекта. Обязательное. Только для чтения.|
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


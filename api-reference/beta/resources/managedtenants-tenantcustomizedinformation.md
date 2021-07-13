---
title: tenantCustomizedInformation resource type
description: Представляет настраиваемые сведения для управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 580479e6fd710eef7a0907ea51cd5605ef445e40
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403156"
---
# <a name="tenantcustomizedinformation-resource-type"></a>tenantCustomizedInformation resource type

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет настраиваемые сведения для управляемого клиента.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список tenantCustomizedInformations](../api/managedtenants-managedtenant-list-tenantscustomizedinformation.md)|[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) collection|Получите список объектов [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) и их свойств.|
|[Get tenantCustomizedInformation](../api/managedtenants-tenantcustomizedinformation-get.md)|[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md)|Ознакомьтесь с свойствами и отношениями объекта [tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)|
|[Обновление tenantCustomizedInformation](../api/managedtenants-tenantcustomizedinformation-update.md)|[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md)|Обновление свойств объекта [tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|contacts|[коллекция microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md)|Коллекция контактов для управляемого клиента. Необязательное свойство.|
|displayName|String|Имя отображения управляемого клиента. Обязательный. Только для чтения.|
|id|String|Идентификатор Azure Active Directory клиента для управляемого клиента. Обязательный. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md) Необязательно. Только для чтения.|
|веб-сайт|String|Веб-сайт управляемого клиента. Обязательный.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantCustomizedInformation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "contacts": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
    }
  ],
  "website": "String"
}
```

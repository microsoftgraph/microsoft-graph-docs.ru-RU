---
title: тип ресурса tenantRelationship
description: Представляете различные типы отношений с клиентами.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 5873f7b2740b342619755ea3bdda3cdd587837ea
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587310"
---
# <a name="tenantrelationship-resource-type"></a>тип ресурса tenantRelationship

Пространство имен: microsoft.graph

Представляете различные типы отношений с клиентами.

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|delegatedAdminCustomers|[delegatedAdminCustomer](../resources/delegatedadmincustomer.md) collection|Клиент, у которого есть делегированная связь администратора с партнером Майкрософт.|
|delegatedAdminRelationships|[delegatedAdminRelationship collection](../resources/delegatedadminrelationship.md)|Сведения о делегированных административных привилегиях, которые партнер Майкрософт имеет в клиенте клиента.|
|managedTenants|[microsoft.graph.managedTenants.managedTenant](../resources/managedtenants-managedtenant.md)|Операции, доступные для взаимодействия с платформой управления с несколькими клиентами.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantRelationship",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tenantRelationship"
}
```

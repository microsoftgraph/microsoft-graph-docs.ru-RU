---
title: Тип ресурса delegatedAdminServiceManagementDetail
description: Содержит сведения об управлении службой в клиенте клиента, управляемом делегированным администрированием.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 53eca1c8d8d60ea78e080caede5ed7096a6ff825
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704197"
---
# <a name="delegatedadminservicemanagementdetail-resource-type"></a>Тип ресурса delegatedAdminServiceManagementDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения об управлении службой в клиенте клиента, управляемом делегированным администрированием.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление delegatedAdminServiceManagementDetails](../api/delegatedadmincustomer-list-servicemanagementdetails.md)|[delegatedAdminServiceManagementDetail](delegatedadminservicemanagementdetail.md)|Получение списка объектов **delegatedAdminServiceManagementDetail** и их свойств.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор управляемой службы. Только для чтения.|
|serviceName|String|Имя управляемой службы. Только для чтения.|
|serviceManagementUrl|String|URL-адрес портала управления для управляемой службы. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminServiceManagementDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminServiceManagementDetail",
  "id": "String (identifier)",
  "serviceName": "String",
  "serviceManagementUrl": "String"
}
```

---
title: тип ресурса delegatedAdminServiceManagementDetail
description: Содержит сведения об управлении службой в клиенте-клиенте, управляемом делегированной администрацией.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 837a7377031b7b2b913cf9346f8ca151da0267e1
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589794"
---
# <a name="delegatedadminservicemanagementdetail-resource-type"></a>тип ресурса delegatedAdminServiceManagementDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения об управлении службой в клиенте-клиенте, управляемом делегированной администрацией.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список делегированAdminServiceManagementDetails](../api/delegatedadmincustomer-list-servicemanagementdetails.md)|[delegatedAdminServiceManagementDetail](delegatedadminservicemanagementdetail.md)|Получите список делегирования **объектовAdminServiceManagementDetail** и их свойств.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор управляемой службы. Только для чтения.|
|serviceName|Строка|Имя управляемой службы. Только для чтения.|
|serviceManagementUrl|Строка|URL-адрес портала управления для управляемой службы. Только для чтения.|

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

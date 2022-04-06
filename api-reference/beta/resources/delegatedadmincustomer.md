---
title: тип ресурса delegatedAdminCustomer
description: Представляет клиента, у которого есть делегированная связь администратора с партнером Майкрософт.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b7ac3c580ab566565d99f7c7c542e2bee0f0bcc3
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589990"
---
# <a name="delegatedadmincustomer-resource-type"></a>тип ресурса delegatedAdminCustomer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет организацию Azure AD, которая является клиентом партнера Майкрософт и имеет делегированную связь администратора с партнером Майкрософт. Этот объект автоматически создается системой, когда между партнером и клиентом существует по крайней мере одна делегированная связь администратора и удаляется, если более активных отношений не существует.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список делегированAdminCustomers](../api/tenantrelationship-list-delegatedadmincustomers.md)|[delegatedAdminCustomer](delegatedadmincustomer.md) collection|Получите список делегирования **объектовAdminCustomer** и их свойств.|
|[ДелегированиеAdminCustomer](../api/delegatedadmincustomer-get.md)|[delegatedAdminCustomer](delegatedadmincustomer.md)|Ознакомьтесь с свойствами и отношениями объекта **делегированияAdminCustomer** .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя клиента клиента отображает имя Azure AD. Только для чтения. Поддерживает `$orderBy`. |
|id|String|Уникальный идентификатор клиента, назначенного Azure AD. Только для чтения. Наследуется от [сущности](../resources/entity.md).|
|tenantId|String|ID клиента, назначенного Azure AD. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|serviceManagementDetails|[delegatedAdminServiceManagementDetail](delegatedadminservicemanagementdetail.md) collection|Содержит сведения об управлении службой в клиенте-клиенте, управляемом делегированной администрацией.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminCustomer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminCustomer",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String"
}
```

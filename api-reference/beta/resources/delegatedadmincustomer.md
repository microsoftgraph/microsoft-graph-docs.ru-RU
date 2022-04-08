---
title: Тип ресурса delegatedAdminCustomer
description: Представляет клиента, который имеет делегированные отношения администратора с партнером Майкрософт.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 4d86eb070a72102aee490321bc854ea319467fab
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704219"
---
# <a name="delegatedadmincustomer-resource-type"></a>Тип ресурса delegatedAdminCustomer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет организацию Azure AD, которая является клиентом партнера Майкрософт и имеет делегированные отношения администратора с партнером Майкрософт. Этот объект автоматически создается системой, если между партнером и клиентом существует хотя бы одна делегированная связь администратора, и удаляется, если активных связей больше нет.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление delegatedAdminCustomers](../api/tenantrelationship-list-delegatedadmincustomers.md)|[Коллекция delegatedAdminCustomer](delegatedadmincustomer.md)|Получение списка объектов **delegatedAdminCustomer** и их свойств.|
|[Получение delegatedAdminCustomer](../api/delegatedadmincustomer-get.md)|[delegatedAdminCustomer](delegatedadmincustomer.md)|Чтение свойств и связей объекта **delegatedAdminCustomer** .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя клиента Клиента Azure AD. Только для чтения. Поддерживает `$orderBy`. |
|id|String|Уникальный идентификатор клиента, назначаемого Azure AD. Только для чтения. Наследуется от [сущности](../resources/entity.md).|
|tenantId|String|Идентификатор клиента, назначаемого Azure AD. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|serviceManagementDetails|[Коллекция delegatedAdminServiceManagementDetail](delegatedadminservicemanagementdetail.md)|Содержит сведения об управлении службой в клиенте клиента, управляемом делегированным администрированием.|

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

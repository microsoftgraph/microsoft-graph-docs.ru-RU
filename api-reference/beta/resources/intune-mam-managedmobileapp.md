---
title: Тип ресурса managedMobileApp
description: Идентификатор для развертывания приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1aee8113116bd831b94c74bbf7f3310820197706
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266734"
---
# <a name="managedmobileapp-resource-type"></a>Тип ресурса managedMobileApp

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Идентификатор для развертывания приложения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов managedMobileApp](../api/intune-mam-managedmobileapp-list.md)|Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Список свойств и связей объектов [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|
|[Получение объекта managedMobileApp](../api/intune-mam-managedmobileapp-get.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Чтение свойств и связей объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|
|[Создание объекта managedMobileApp](../api/intune-mam-managedmobileapp-create.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Создание объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|
|[Удаление объекта managedMobileApp](../api/intune-mam-managedmobileapp-delete.md)|Нет|Удаляет объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|
|[Обновление объекта managedMobileApp](../api/intune-mam-managedmobileapp-update.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Обновление свойств объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Идентификатор приложения с типом его операционной системы.|
|id|String|Ключ объекта.|
|version|String|Версия объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```





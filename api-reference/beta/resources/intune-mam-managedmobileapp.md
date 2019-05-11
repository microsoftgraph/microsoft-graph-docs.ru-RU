---
title: Тип ресурса managedMobileApp
description: Идентификатор для развертывания приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8e6daa53e5985b0c91d51945db58da6ab2d9482
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940675"
---
# <a name="managedmobileapp-resource-type"></a>Тип ресурса managedMobileApp

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|Строка|Ключ объекта.|
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
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




